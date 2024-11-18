# Pong Game 🏓

## Description

This is a classic Pong game built using Python's `turtle` graphics module. The objective of the game is to control paddles and try to bounce the ball past the opponent's paddle to score a point. The game keeps track of the score for both players, and the first player to reach a certain score wins.

This project demonstrates **object-oriented programming (OOP)** principles by organizing the game into classes for the ball, paddles, and scoreboard.

## Features

- **Two-Player Gameplay**: One player controls the right paddle using the Up and Down arrow keys, while the other controls the left paddle using the "W" (up) and "S" (down) keys.
- **Ball Movement**: The ball bounces off the top and bottom edges and is affected by the paddles.
- **Score Tracking**: The score is displayed at the top of the screen, with points awarded when the ball passes a player's paddle.
- **Game Reset**: The ball resets to the center after scoring, and the game continues.

## Requirements

- Python 3.x
- `turtle` graphics module (pre-installed with Python)

## How to Play

1. **Start the Game**:
   - Run the `game.py` script to start playing.

2. **Control the Paddles**:
   - **Right Paddle**: Use the Up and Down arrow keys.
   - **Left Paddle**: Use the "W" (up) and "S" (down) keys.

3. **Score Points**:
   - When the ball passes one of the paddles, the opponent scores a point.
   - The game continues until a predefined score is reached (you can modify this in the code).

4. **Game Over**:
   - The game does not end automatically. Players can choose to reset or close the game after each round.

## Code Structure

### Files Breakdown

Here is a breakdown of each file and its purpose in the game:

---

### `game.py`

- **Purpose**: This is the main file that runs the game. It sets up the screen, initializes the game objects (paddles, ball, scoreboard), and controls the flow of the game.
- **Key Functionality**:
  - Controls the movement of the ball and paddles.
  - Handles ball bounce logic (when it hits the top/bottom or the paddles).
  - Checks for scoring conditions and updates the scoreboard.

---

### `scoreboard.py`

- **Purpose**: This file defines the `Scoreboard` class, which tracks and displays the scores for both players.
- **Key Functions**:
  - `update_scoreboard()`: Displays the current scores for the left and right players.
  - `l_point()`: Increases the score of the left player by one and updates the scoreboard.
  - `r_point()`: Increases the score of the right player by one and updates the scoreboard.

---

### `paddle.py`

- **Purpose**: This file defines the `Paddle` class, which is responsible for creating and controlling the paddles for both players.
- **Key Functions**:
  - `go_up()`: Moves the paddle up by 20 units.
  - `go_down()`: Moves the paddle down by 20 units.
  - The paddles are positioned on the left and right sides of the screen, and their size is adjustable using `shapesize()`.

---

### `ball.py`

- **Purpose**: This file defines the `Ball` class, which controls the ball's movement and behavior in the game.
- **Key Functions**:
  - `move()`: Moves the ball according to its speed and direction.
  - `bounce_y()`: Reverses the vertical direction of the ball when it hits the top or bottom edges of the screen.
  - `bounce_x()`: Reverses the horizontal direction of the ball when it hits one of the paddles.
  - `reset_position()`: Resets the ball's position to the center of the screen when a point is scored.

---

## How to Run

1. Clone or download the project files.
2. Make sure Python 3.x is installed on your computer.
3. Open a terminal or command prompt and navigate to the project directory.
4. Run the following command to start the game:

```bash
python game.py
```

## Future Improvements

- **Sound Effects**: Add sound effects for events like scoring a point or hitting a paddle.
- **Increasing Difficulty**: Increase the speed of the ball as the game progresses to make it more challenging.
- **Graphical User Interface (GUI)**: Implement a more complex interface with features like a game menu, options for player vs AI, or settings to change the game's difficulty.
- **Leaderboard**: Save high scores and display a leaderboard.

## Credits

This project was created as an exercise to demonstrate object-oriented programming (OOP) principles and basic game development using Python's `turtle` graphics module.

