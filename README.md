# Maze project

## Desciption

The goal of this project is to create a game in 3D using raycasting. Ray-casting is a techniques that transform a limited form of data (a very simplified map or floor plan) into a 3D projection by tracing rays from the view point into the viewing volume.

![maze using raycasting](/images/maze1.png)

## General Requirements

    * All your files will be compiled on Ubuntu 14.04 LTS, using gcc (Ubuntu 4.8.4-2ubuntu1~14.04) 4.8.4
    * We will use the gcc flags -Wall -Werror -Wextra and -pedantic
    * All your functions must be commented
    * Your functions should be maximum 40 lines long (one statement per line)
    * Your functions should be maximum 80 columns long
    * No more than 5 functions per file
    * Your entire repository will be checked using Betty

![door_open](/images/maze44.png)

## How the project works
   * the project first creates the window and initialize the game with some default value
   * It then displays the map and the game zone to the user
   * the user uses keys like (like w, a, s, d, e & arrow keyes) to move & rotate the player
   * the system continously checks the input key provided by the user
   * if an Escape key or Quit buttom is tapped or clicked, it quits the game and destroy the window

## System Usage

   * Download the source file from the githbub.com into your local machine
   * naviagete to the Maze folder
   * compile all source codes ending with .c extension using the following flag:
        gcc -Wall -Werror -Wextra -pedantic ./src/*.c -lm $(sdl2-config --cflags --libs) -lSDL2_ttf -lSDL2_image -o maze
   * launch the executable file like ./maze if you want to use the default map
   * launch the executable file by passing the name of the map file if you want to provide your own map like "./maze map"  here map is the name of your file
   * the system then displays the map & the game zone on the screen
   * Press up arrow key or w key to move the player to upper positon
   * press down arrow key or s key to move the player to down postion
   * press left arrow key or a key to rotate the player in counter clockwise direction
   * press right arrow key or d key to rotate the player in clockwise direction
   * press e key to open the door
   * press Escape key or click Quit button to exit the game

![door_open](/images/maze33.png)

## content of the Maze project
| File name       | Description |
---               | ---    |
main.c            | a c file which contains the main method and the display function
cast.c            | a c filw which defines main component of casting throug the methods ray_cast, horizontal collision , vertical collistion
drow.c            | a c file which contains methods used to draw a map, player, wall, roof & floor
map.c             | a c file which defines a map coordinates and method to access them
texture           | a c file which defines a texture value and method to access them
window            | a c file which contains method used to define the window and input keyboards

---


## Author
Raheem Salifu Kasim(https://github.com/devrsk)
