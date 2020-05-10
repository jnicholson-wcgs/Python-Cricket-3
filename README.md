# Python-Cricket-3
Third task in the Python Cricket Saga

The third quest in the Python cricket saga, is to add:
1) A main menu
2) Some file handling

Task One
--------

Add a main menu to your program, with at least three user options:
1: Play the match
2: Pick the team
3: Load the team file

Option 1 (Play the match) should call your match() routine to run the scoring for the match
Options 2 and 3 get implemented below

Task Two
--------

Write a new routine loadfile() which takes the name of file to load.
loadfile() should return the number of players from the team file or -1 if the file did not load.
From the main menu option 3, call loadfile() with the filename, for example, 

teamfile = "WCGS-Team.tex"
nplayers = loadfile (teamfile)
if (nplayers == -1) :
  print ("Error: team file not found", teamfile
  
Load up the WCGS-Team.txt file into your program:
1) Open the file WCGS-Team.txt
2) Add it a global data structure called WCGS-Team. This can be a list (or another data structure)
3) Close the WCGS-Team.txt file

The file has a comma separated list of three items:
- Player name (this can be spaces in it)
- Player position: bowler, batsman, all-rounder or wicketkeeper

Ensure that you have correct error handling for your code, e.g., your program should not fail if the file does not exist
Also check that the player position values are correct. Ignore players where position is not from the four valid positions (bowler, batsman, all-rounder or wicketkeeper)

Task Three
----------

The team is loaded via Option 3.

Implement the pickteam() subroutine called from Option 2.

pickteam() is used to pick the WCGS team:
- Show the user the wicketkeepers in the team, and get the user to select exactly 1 wicketkeeper;
- Show the user the all-rounders, and prompt them to pick a maximum of 1;
- Show the user the bowlers and prompt for bowlers. There must be a minimum of 4 bowlers, including the all-rounders;
- Calculate the remaining players to pick, so that the total team selected is 11, and
- Show the batsmen and prompt for batsmen until the 11 players are picked.

Ensure your progrgram is fully tested, for example:
- No wicketkeeper selected
- All the all-rounders and no specialist bowlers
- No all-rounders and only specialist bowlers


Task Four
---------

Show the user the team selected in pickteam() and prompt them to select the batting order (the order in which each batsmen play)

Update the validateball() routine to accept 'o' or 'O' for the batsmen being out.
Keep track of the number of batsmen out. The innings finishes when there are ten players out.



