This file justs goes through all of the edits made to Aritra Bal's original code

Edits by Louise Luker

//edit is added to all edited lines of code to be found easily

[61] Includes <cmath> into the code as was required when dealing with the vectors

[75][76] Loads libPhysics and libMathCore as required when running as kept getting errors

[81] Changed the name of the TTree that is gotten from the file as was named 'analysis' in the new converted PHYSLITE file

[84][86][87][88] Had to change the type of some of the variables as they are stored as different types in the new converted PHYSLITE root file

[111][119][120][121][122][124] Changed the name of some of the input branches as they are named differently in the new converted PHYSLITE root file

[123] The branch gathered here does not exist in the new converted PHYSLITE file and so was commented out

[130]-[136] Had to be commented out also as the 2012 data does not work with this, and also was not needed, and it kept giving errors that needed to be stopped

[361][362][363] Lines added whilst debugging, [361] prints the total number of events. The others are commented out now, but were used to see where things were struggling

[377][378][380][382][383] All are lines that were added for debugging. First begin a wtopwatch to time how long it takes to process each event, then prints the event number, then prints the number of leptons within that event

[410]-[414] Had to be commented out also as the 2012 data does not work with this, and also was not needed, and it kept giving errors that needed to be stopped

[424][456] Removed the MeV to GeV conversion as PHYSLITE ntuple already gives in GeV

[531] Added an if statement that skips the following loops if there are no leptons in the event, as without this line it would get stuck in an infinite loop. Required as old data was skimmed to removed any events with no leptons, but new PHYSLITE file is unskimmed

[646][647] End of timer from above, prints the time taken to process each event. Added for debugging, now commented out

[681] Line added to adapt my file, all lines below commented out as they were for the old files
