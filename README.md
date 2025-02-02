Snake Game
A simple implementation of the classic Snake game using HTML5 Canvas and JavaScript.

Overview
This project recreates the classic Snake game where the player controls a snake that grows longer each time it eats an apple. The game features:

Snake Movement: Control the snake with the arrow keys.
Apple Eating: When the snake's head touches an apple, the snake grows longer and a new apple appears at a random location.
Screen Wrapping: The snake reappears on the opposite side of the canvas when it goes off one edge.
Score Display: The score is updated based on the number of apples eaten (i.e., the snake’s length minus one).
Getting Started
Prerequisites
A modern web browser (e.g., Chrome, Firefox, Edge, Safari).
Installation
Clone the Repository:

bash
Kopyala
git clone https://github.com/yourusername/snake-game.git
Navigate to the Project Directory:

bash
Kopyala
cd snake-game
Open the index.html File:

You can open the index.html file directly in your browser. Alternatively, you can serve the project using a local web server.

Using Python (if installed):

bash
Kopyala
# For Python 3.x:
python -m http.server 8000
Then, open your browser and go to: http://localhost:8000

How to Play
Controls:

Left Arrow: Move left.
Right Arrow: Move right.
Up Arrow: Move up.
Down Arrow: Move down.
Objective:

Guide the snake to eat the red apples.
Each apple eaten increases the length of the snake and your score.
Avoid running into the walls; instead, the snake will wrap around the canvas.
File Structure
index.html: Contains the HTML structure and the canvas element where the game is rendered.
game.js: Contains all the game logic, including:
Game loop setup
Snake movement and tail update
Apple generation and collision detection
Drawing functions to render the game elements
README.md: This file, which explains the project details and how to run it.
Code Overview
Game Loop:
The game uses setInterval to call the show function at a rate of 20 frames per second, which updates the game state and redraws the canvas.

Snake Movement:
The snake’s head is updated based on the current direction set by the arrow keys. The tail is managed by shifting the first element and pushing a new head position.

Apple Eating:
When the snake’s head coordinates match the apple’s coordinates, the snake grows, and a new apple is created at a random position that does not overlap with the snake.

Wall Collision:
Instead of ending the game when the snake hits a wall, the snake wraps around to the opposite side of the canvas.

License
This project is open source and available under the MIT License.

Acknowledgments
Inspired by the classic Snake game.
Developed as a fun project to learn more about HTML5 Canvas and JavaScript game development.
