**Tic-Tac-Toe using React.js**

## Overview
-This project is a React-based Tic-Tac-Toe game where two players can play against each other. 
-The game manages turns, checks for winning combinations, and declares a winner or a draw at the end. 
-Players can restart the game or change their names at any time, enhancing the interactive experience.

## Code Structure

### `App.js`

The `App.js` file is the main component of the application. It manages the state of the game, including the players, game turns, and game board. 
Here is an overview of its main functions and components:

- **State Management:**
  - `players`: An object holding player names.
  - `gameTurns`: An array holding the history of game turns.

- **Helper Functions:**
  - `derivedActivePlayer(gameTurns)`: Determines the current active player based on the number of game turns.
  - `deriveGameBoard(gameTurns)`: Creates a game board from the game turns.
  - `deriveWinner(gameBoard, players)`: Checks the game board for any winning combination and returns the winner if found.

- **Main Functions:**
  - `handleSelectSquare(rowIndex, colIndex)`: Updates the game turns when a square is selected.
  - `handleRestart()`: Resets the game turns to start a new game.
  - `handlePlayerNameChange(symbol, newName)`: Updates a player's name.

- **Rendering:**
  - Renders the `Player` components to display player names and the active player.
  - Renders the `GameBoard` component to display the game board.
  - Renders the `Log` component to display the history of game turns.
  - Renders the `GameOver` component when the game ends in a win or a draw.
 
