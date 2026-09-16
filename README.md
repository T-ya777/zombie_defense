# Zombie Defense

Zombie Defense is a tower defense game I built in Python as my final project for Carnegie Mellon's Fundamentals of Programming and Computer Science course (15-112).

The project was ranked **Top 8 among 400+ course submissions**.

## Overview

The game combines tower defense mechanics with interactive puzzles and a grid-based zombie trapping minigame. Players defend against waves of zombies, earn resources, purchase upgrades, and complete challenges with increasing difficulty.

I built the project using Python and CMU Graphics, with the game logic organized around six custom classes for enemies, bullets, soldiers, shop items, bonus items, and puzzle pieces.

## Features

- Multi-screen tower defense gameplay
- Enemy waves and dynamic difficulty progression
- Upgrade and economy systems
- Interactive draggable puzzle pieces
- Collision detection and combat mechanics
- Grid-based zombie trapping minigame
- Multiple pathfinding strategies based on difficulty

## Pathfinding

One of my favorite parts of the project was implementing different approaches to pathfinding for the zombie trapping minigame.

### Easy
Uses recursive backtracking to find a valid route through the grid.

### Medium
Uses recursive search with pruning to find a shorter path while avoiding unnecessary exploration.

### Hard
Uses Breadth-First Search (BFS) with a queue and visited set to find a shortest path through the grid.

Working on these different approaches gave me an early introduction to graph search and pathfinding. I later studied BFS and related data structures more formally in CMU's Principles of Imperative Computation (15-122).

## Interactive Puzzle System

The game also includes draggable polygon-based puzzle pieces. I implemented point-in-polygon detection using ray casting to determine whether the player's mouse is inside an irregularly shaped piece, along with dragging and snapping behavior.

## Tech

- Python
- CMU Graphics
- Object-Oriented Programming
- Breadth-First Search
- Recursive Backtracking
- Collision Detection
- Ray Casting

## Running the Project

1. Install Python 3.
2. Install the required CMU Graphics dependencies.
3. Clone this repository.
4. Run the main Python file.

## Acknowledgments

This project was created as a final project for CMU 15-112: Fundamentals of Programming and Computer Science.

Some visual and audio assets used in the game were created with or sourced from external tools and resources. Attribution for these assets is included in the source code.
