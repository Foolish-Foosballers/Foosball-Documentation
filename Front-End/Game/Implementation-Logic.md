# Implementation Logic

General implementation logic of a user starting, playing, and ending a game.

## Step 1 - Pregame
1. If a game is not in progress, the user should be directed into the 'lobby' page. If a game is in progress, the user should be directed into the current 'scoreboard' page and continue with Step 2.
2. The 'lobby' page will have the following components:
   
   1. A welcome message
   2. A form with the following components:
     
      1. 'Type of game' dropdown (individual or series)
      2. 'Number of players' dropdown ( 2 or 4).
      3. 'Email' text fields (2 or 4, depending on the answer to the 'number of players dropdown).
      4. 'Pin' text fields (2 or 4, depending on the answer to the 'number of players' dropdown).
      5. 'Start Game' button.
      
    3. 'Create New Player' button.
3. The user should fill out the information in the form.
4. If the form's data is valid enable the 'start game' button. If the form's data is invalid disable the 'start game' button.
5. If the data is valid and the 'start game' button was selected, start the game and direct the user into the 'scoreboard'.

   1. If the user selects 'start game' with invalid form data, present the user with an error message and do not let them start the game until the data is corrected.
   2. Do not allow any instance of the application to go to the 'lobby' again until the current game has been completed.

## Step 2 - Gameplay

## Step 3 - Postgame
