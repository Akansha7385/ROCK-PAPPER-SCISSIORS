# Rock, Paper, Scissors Game

This project is a simple web-based implementation of the classic **Rock, Paper, Scissors** game. Users can play against the computer, with scores tracked throughout the game.

## Features

- Players choose between Rock, Paper, or Scissors by clicking on the corresponding image.
- The computer randomly selects one of the three options: Rock, Paper, or Scissors.
- The winner is determined according to the traditional rules of the game:
  - Rock beats Scissors.
  - Paper beats Rock.
  - Scissors beat Paper.
- The game declares a win, loss, or draw after each round and updates the score accordingly.
- The game includes simple styling and feedback through colors and messages.

## Project Structure

- **HTML Structure**: 
  The game elements are represented as clickable buttons with images. The score and result message are also displayed on the webpage.

- **CSS Styling**:
  Basic styling is applied for the layout and appearance of the game elements, including hover effects, centering, and responsive visuals. The styling also updates based on whether the player wins, loses, or the round is a draw.

- **JavaScript Logic**:
  The game logic is handled in JavaScript, which:
  - Tracks the player and computer's scores.
  - Randomly generates the computer's choice.
  - Compares the player and computer's choices to determine the outcome.
  - Updates the score and displays appropriate messages for each round.

## Code Breakdown

- **Game Variables**:
  - `userScore` and `compScore`: Keeps track of the user's and computer's scores.
  - `choices`: HTML elements representing the user's options (Rock, Paper, or Scissors).
  - `msg`, `userScorePara`, `compScorePara`: DOM elements used to update the game status, scores, and messages on the UI.

- **Functions**:
  - `genCompChoice()`: Randomly generates the computer's choice of Rock, Paper, or Scissors.
  - `drawGame()`: Displays the message for a draw round.
  - `showWinner(userWin, userChoice, compChoice)`: Displays the winner of the round and updates the score and message based on whether the player won or lost.
  - `playGame(userChoice)`: Runs the game logic for each round, comparing the player's choice to the computer's choice and updating the game status.

- **Event Listeners**:
  Each `.choice` element (representing Rock, Paper, or Scissors) has an event listener. When clicked, it calls `playGame(userChoice)` to play a round of the game with the user's choice.

