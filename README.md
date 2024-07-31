# Some of my Java mini-projects

## Blob Game

<p align="center">
  <img src="https://github.com/user-attachments/assets/01eed8c0-f463-4803-bdd0-26fc4c18af77" width="300" />
</p>


Welcome to **Blob Game**, an exciting and interactive Java project where you control a growing Blob in a world full of evil Blobs. Your mission: eat the smaller blobs to grow bigger while avoiding the larger ones!

### Table of Contents
- [Introduction](#introduction)
- [Gameplay](#gameplay)
- [Features](#features)
- [How to Play](#how-to-play)
- [Code Overview](#code-overview)
- [Getting Started](#getting-started)

### Introduction

Blob Game is a simple yet engaging game built using Java. The game starts with a player-controlled blob, which can move in all directions. The goal is to eat smaller blobs to increase in size while avoiding larger blobs that can end the game.

### Gameplay

- **Control your Blob:** Move your blob using the 'W', 'A', 'S', and 'D' keys.
- **Eat to Grow:** Consume smaller blobs to increase your size.
- **Avoid Bigger Blobs:** Stay away from blobs larger than yourself to avoid the game ending.
- **Win Condition:** Reach a blob radius of 115 to win the game.

### Features

- **Interactive Controls:** Use keyboard inputs to navigate your blob around the game field.
- **Dynamic Difficulty:** As your blob grows, the game gets more challenging with more evil blobs appearing.
- **Visual Feedback:** The color of your blob changes as it grows, giving a visual representation of your progress.
- **Collision Detection:** Advanced collision detection ensures a fair and challenging gameplay experience.

### How to Play

1. **Start the Game:** Launch the game and control your blob using the 'W', 'A', 'S', and 'D' keys.
2. **Move and Eat:** Navigate the game field to find and consume smaller blobs.
3. **Avoid Dangers:** Stay clear of larger blobs to avoid being eaten.
4. **Grow and Win:** Continue eating smaller blobs until your blob's radius reaches 115 to win the game.

### Code Overview

The Blob Game is built with two main classes: `Blob` and `BlobGame`.

#### Blob Class

- **Properties:**
  - `int radius`: Size of the blob.
  - `Color theColor`: Color of the blob.
  - `int x, y`: Coordinates of the blob.
  - `int deltaX, deltaY`: Velocity of the blob.

- **Methods:**
  - `getX()`, `getY()`, `getRadius()`: Getters for blob properties.
  - `eat()`: Increase the size of the blob.
  - `move()`, `moveRight()`, `moveLeft()`, `moveUp()`, `moveDown()`: Control blob movement.
  - `draw(Graphics g)`: Render the blob.

#### BlobGame Class

- **Properties:**
  - `Blob playerBlob`: The player's blob.
  - `ArrayList<Blob> evilBlobs`: List of enemy blobs.
  - `int delay`: Delay for game loop.
  - `boolean gameOver`: Game over flag.

- **Methods:**
  - `keyPressed(KeyEvent e)`: Handle key press events.
  - `checkForCollision()`: Check and handle collisions between blobs.
  - `createEvilBlob()`: Create new enemy blobs.
  - `distance(int x1, int y1, int x2, int y2)`: Calculate distance between two points.
  - `paint(Graphics g)`: Render the game field.
  - `run()`: Main game loop.

### Getting Started

To get started with Blob Game, you'll need to have Java installed on your machine. Follow these steps:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/blob-game.git



### Java Graphics Drawings

<p align="center">
  <img src="https://github.com/user-attachments/assets/b254b4c2-8e32-4b00-8213-649556a4de8c" width="300" />
</p>


## Graphicstron

Welcome to **Graphicstron**, a Java-based graphical design program that allows users to create various patterns and designs. This application features a range of buttons, each triggering a unique graphical design.

### Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [User Interface](#user-interface)
- [How to Use](#how-to-use)
- [Code Overview](#code-overview)
- [Getting Started](#getting-started)

### Introduction

Graphicstron is a graphical design application developed in Java. It utilizes a series of buttons to select different design patterns, which are then drawn on the screen using custom painting methods.

### Features

- **Interactive User Interface:** Easy-to-use buttons for selecting different design patterns.
- **Multiple Designs:** Includes patterns such as Box Grid, Multiplication Table, Brick Wall, ZigZag, Wall Paper 70s, and more.
- **Custom Painter Class:** A dedicated class for handling the drawing of various patterns.

### User Interface

The user interface consists of a series of buttons placed on the right side of the screen. Each button corresponds to a different design pattern. Clicking a button triggers the drawing of the selected pattern.

### How to Use

1. **Launch the Application:** Start the application to open the main window.
2. **Select a Pattern:** Click on any of the buttons to select a design pattern.
3. **View the Pattern:** The selected pattern will be drawn on the screen.

### Code Overview

The project consists of two main classes: `Graphicstron` and `Painter`.

#### Graphicstron Class

The `Graphicstron` class is the main class that extends `JPanel` and implements `ActionListener`.

- **Properties:**
  - `ArrayList<Button> buttons`: List of buttons for selecting patterns.
  - `String choice`: The current selected pattern.
  - `Painter thePainter`: Instance of the `Painter` class.
  - `int command`: Command identifier.

- **Methods:**
  - `Graphicstron()`: Constructor to initialize the UI and buttons.
  - `actionPerformed(ActionEvent event)`: Handles button click events.
  - `paint(Graphics g)`: Draws the selected pattern on the screen.
  - `main(String[] arg)`: Main method to launch the application.

#### Painter Class

The `Painter` class contains methods to draw each design pattern.

- **Methods:**
  - `paintBoxGrid(Graphics g)`: Draws a grid of boxes.
  - `paintMultiplicationTable(Graphics g)`: Draws a multiplication table.
  - `paintBrickWall(Graphics g)`: Draws a brick wall pattern.
  - `paintZigZag(Graphics g)`: Draws a zigzag pattern.
  - `paintWallPaper70s(Graphics g)`: Draws a 70s style wallpaper.
  - `paintGridAndLines(Graphics g)`: Draws a grid and lines pattern.
  - `paintTubularTwo(Graphics g)`: Draws a tubular pattern.
  - `paintPatchworkMax(Graphics g)`: Draws a patchwork pattern.
  - `paintTiledFloor(Graphics g)`: Draws a tiled floor pattern.
  - `paintPatchWork(Graphics g)`: Draws a patchwork pattern.
  - `paintRainbowFade(Graphics g)`: (Placeholder) Method to draw a rainbow fade.
  - `paintDiscoDown(Graphics g)`: (Placeholder) Method to draw a disco pattern.

## Getting Started

To get started with Graphicstron, ensure you have Java installed on your machine. Follow these steps:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/graphicstron.git


### Myrtle Mazes

<p align="center">
  <img src="https://github.com/user-attachments/assets/8c9ca1de-da35-4a9b-ba15-1d5dda65c95a" width="300" />
</p>

# Myrtle Maze

## Overview

The Myrtle Maze project is a Java-based application where a turtle, named Myrtle, navigates a grid or maze to perform tasks such as picking and placing various fruits. This project involves object-oriented programming concepts, GUI elements using Swing, and game-like mechanics.

## Features

- **Myrtle Navigation**: Myrtle can move around the grid or maze in specified directions.
- **Fruit Picking and Placing**: Myrtle can pick and place apples, oranges, and lemons based on its location and the task at hand.
- **Row and Grid Operations**: Myrtle can perform operations across rows and grids, such as picking all fruits in a row or filling the grid with fruits.
- **Harvesting and Depositing**: Myrtle can harvest fruits from a specified area and deposit them at a designated location.
- **Search and Movement Algorithms**: Myrtle can search for fruits and navigate through the maze using defined movement algorithms.

## Classes and Methods

### Myrtle Class

The `Myrtle` class extends the `Turtle` class and provides additional methods for fruit-related tasks and navigation.

#### Constructor

```java
public Myrtle(JPanel world, Block[][] map, char direction, int row, int col, int appleCount, int orangeCount, int lemonCount)
