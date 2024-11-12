# Run Bear Run

**Run Bear Run** is a JavaScript-based game created as part of my second-year coursework. In this game, players help a bear avoid a swarm of bees by navigating a board and keeping the sting count as low as possible.

## Game Description

This browser-based game allows players to control a bear character and avoid bees, which move randomly around the game board. The objective is to dodge the bees for as long as possible. The game tracks the number of stings (overlaps between the bear and bees) and records the best time duration between stings.

## Installation and Setup

1. Download the project files to your computer.
2. Open `index.html` in a web browser to start the game.

**File Structure:**
- `index.html`: Main HTML file for the game interface.
- `game.js`: Contains the core game logic and functions.
- `game.css`: Styles the game layout.
- `images/`: Folder for `bear.gif` and `bee.gif` images used in the game.

## How to Play

1. Open `index.html` in your browser.
2. Use the arrow keys (Left, Right, Up, Down) to move the bear.
3. Avoid the bees to keep the sting count (`Stings`) low.
4. The `Best duration` score displays the longest time between stings.
5. Adjust game settings as desired:
   - Increase the number of bees.
   - Modify the speed of bees and the bear.
   - Adjust the game’s refresh period.

## Customization

Several game settings can be adjusted in the HTML page:
- **Number of Bees**: Use the input and button in "Bear tries to avoid being stung by" to add more bees.
- **Bee Speed**: Enter a `px/ms` value in the Bee Speed input field.
- **Bear Speed**: Adjust the `px/ms` value in the Bear Speed input field.
- **Refresh Period**: Set the `ms` value in the "Refresh Period" input to change the game loop speed.

## Game Components

### HTML (index.html)
- Defines the game structure, including controls, score display, and game board.
- Uses an `<img>` element for the bear and bees, positioned dynamically on the board.

### JavaScript (game.js)
- Contains main game logic, including movement, bee creation, collision detection, and scorekeeping.
- Key functions:
  - `start()`: Initializes the bear and bees.
  - `moveBear()`: Handles bear movement based on keyboard input.
  - `updateBees()`: Moves bees and checks for collisions with the bear.
  - `isHit()`: Updates the score when a bee stings the bear.
  - `AddBee()`: Adds additional bees.

### CSS (game.css)
- Styles the game components, including the bear, bees, board, title, and score.
- Key styles:
  - `#board`: Defines the play area.
  - `#title` and `#scores`: Style the title and score sections.

The game assets include bear and bee images located in the `images` folder.

Enjoy the game and see how long you can keep the bear safe!
