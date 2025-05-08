README



version 3 stable with updated shooting space (extended for more time to shoot)

Original file by Vukovic

version 6 progressed to sound with gun type either machine or laser gun                                                                                                
Q&A template is actually version 7, where the Q&A cells are found from original file's codes. 

Cells B2 to B19 contain text/formulae.  A2 to A19 contains the values (as funnctions in x, defined)
See file's Global JS last few lines
//////////////////////////////////////////////////////////////////////////////////////////////////

    //Line below sets cells A2 to A19 as functions in x, and set all values = 0
    ggbApplet.evalCommand('Execute(Sequence["A"+i+"(x) = 0", i, 2, 19)]');
    // Line below hides all the functions from A2 to A19 automatically plotted by previous command
    // in Graphics 1
    ggbApplet.evalCommand('Execute(Sequence["SetVisibleInView(A"+i+",1,false)", i, 2, 19)]');
    // Line below parses all the formulae (Text values) in cells B2 to B19 as values
    // in cells A2 to A19
    ggbApplet.evalCommand('Execute[Sequence("ParseToFunction[A"+i+",B"+i+"]",i,2,19)]');
    
////////////////////////////////////////////////////////////////////////////////////////////////////

Background noise added (files with bgs tag)
