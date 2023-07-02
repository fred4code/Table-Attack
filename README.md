# Table Attack

## Overview
Table Attack is built using pure JavaScript without reliance on third-party libraries or game engines. It employs DOM manipulation to create a dynamic and interactive game experience. The game characters, including the player and the enemies, are all represented as HTML table elements. Each cell of the table can be manipulated to create different shapes and colors, effectively making them the "pixels" of our game's 2D sprite graphics.

## Gameplay
The player can move their sprite up, down, left, or right within the game scene. The aim is to avoid enemies that spawn randomly at the top of the screen and move downwards, while also shooting at these enemies. If an enemy collides with the player, the game ends.

## How to Play
Click "Start Game" with the mouse to start playing. <br/>
Use the arrow keys on your keyboard to move your character around the game scene and the space bar to shot.

## Technical Details
The game runs on a continuous loop that updates every definite amount of milliseconds.
In each iteration, the game checks for user inputs (movement and shooting), moves enemies and projectiles, and checks for collisions.

HTML tables are used to create the game graphics. The player, enemies, and projectiles are all instances of a TableSprite class, which generates an HTML table element and allows for manipulating the cells' styles to create different shapes and colors.

The player and enemy movements are controlled by changing the CSS properties of their respective table elements. Collisions are detected using the getBoundingClientRect method, which provides the size and position of an element. This information is used to check if the rectangles of different elements overlap, signifying a collision.

This game offers a unique approach to 2D game development (as far as I have found). Instead of using canvas or WebGL for graphics, it explores the possibility that HTML tables can also provide a flexible and simple way to create game sprites and handle collisions, bringing a retro, pixel-art style to the web browser.

## Future Improvements
Future updates of Table Attack may include power-ups, different types of enemies, and a scoring system to make gameplay more exciting and engaging.

# Credits

## Sounds
blaster-2-81267.mp3 - is taken from here: https://pixabay.com/sound-effects/search/laser/<br/> 
Thanks to the author: Pixabay!

## Background music
Enigma-Long-Version-Complete-Version.mp3 is taken from here: https://www.chosic.com/download-audio/32067/<br/> 
Mention the artist of Enigma-Long-Version-Complete-Version.mp3:<br/> 
Aggressive Computer Gaming | ENIGMA by Alex-Productions | https://onsound.eu/<br/> 
Music promoted by https://www.chosic.com/free-music/all/<br/> 
Creative Commons CC BY 3.0<br/> 
https://creativecommons.org/licenses/by/3.0/<br/> 

Note: the playback speed of the music is increased by 50%