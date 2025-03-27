# Tic-Tac-Toe React Game

A modern, interactive implementation of the classic Tic-Tac-Toe game built with React. This project was created following Maximilian Schwarzmüller's Udemy React course.

## Features

- **Interactive Game Board**: Clickable 3x3 grid for placing X and O marks
- **Player Management**: Editable player names with visual indicators for the active player
- **Game State Tracking**: Real-time tracking of game progress with a log of all moves
- **Win Detection**: Automatic detection of winning combinations and game draws
- **Responsive Design**: Beautiful UI with animations that works on different screen sizes

## Project Structure

- `App.jsx`: Main component managing game state and logic
- `components/`:
  - `Player.jsx`: Handles player information and name editing
  - `GameBoard.jsx`: Renders the 3x3 game grid with interactive squares
  - `Log.jsx`: Displays a history of all moves made during the game
  - `GameOver.jsx`: Shows the end game screen with winner announcement and restart option
  - `winningCombinations.js`: Defines all possible winning patterns

## How It Works

### Game Logic

The game uses several key React concepts:

1. **State Management**: Uses React's `useState` hook to track:
   - Player names
   - Game turns
   - Active player
   - Game board status

2. **Derived State**: Instead of storing everything in state, some values are derived:
   - Active player is calculated from the current turns
   - Game board configuration is derived from the history of moves
   - Winner is determined by checking current board against winning combinations

3. **Component Communication**: Uses props to pass data and callbacks between components

### Playing the Game

1. Players can edit their names by clicking the "Edit" button
2. The active player is highlighted
3. Players take turns clicking on empty squares to place their symbol (X or O)
4. A log displays all moves made during the game
5. When a player completes a winning combination, or all squares are filled, the game ends
6. Players can start a rematch by clicking the "Restart" button

## Technologies Used

- **React**: For building the user interface components
- **JavaScript ES6+**: Modern JavaScript syntax for clean, maintainable code
- **CSS**: Custom styling with animations for an engaging user experience

## Getting Started

### Prerequisites

- Node.js (v14 or later)
- npm or yarn

### Installation

1. Clone the repository:
   ```
   git clone https://github.com/yourusername/Udemy_Tic_Tac_Toe.git
   cd Udemy_Tic_Tac_Toe
   ```

2. Install dependencies:
   ```
   npm install
   ```

3. Start the development server:
   ```
   npm run dev
   ```

4. Open your browser and navigate to `http://localhost:5173`

## Learning Points

This project demonstrates several important React concepts:

- Component-based architecture
- State management with hooks
- Lifting state up
- Derived state calculations
- Conditional rendering
- Event handling
- CSS animations and styling in React applications

## Acknowledgements

- This project was created as part of [Maximilian Schwarzmüller's React course on Udemy](https://www.udemy.com/course/react-the-complete-guide-incl-redux/)
- React logo and documentation from [React](https://reactjs.org/)
