# Conway's Game of Life Simulation

## Overview

The objective of this project is to implement a simulation of Conway's Game of Life, a well-known cellular automaton (CA). This simulation will demonstrate the behavior of cells based on a set of rules, where each cell is either "alive" or "dead" and evolves in discrete time steps.

The project will use at least one simple data structure (dynamic matrix) encapsulated within a C++ class to represent the grid of cells and handle the simulation.

## Conway's Game of Life Rules

1. **Cell Survival**: A live cell with two or three live neighbors remains alive in the next generation. 
2. **Cell Death**: A live cell with fewer than two live neighbors dies due to underpopulation, and with more than three live neighbors, it dies due to overpopulation.
3. **Cell Birth**: A dead cell with exactly three live neighbors becomes alive in the next generation.

## Requirements

- **Programming Language**: C++
- **Data Structure**: Dynamic matrix (to represent the grid of cells)
- **Input/Output**: The program should take an initial state (a grid configuration) as input and output the grid after each iteration or generation.

## Features

- Dynamic grid creation and manipulation
- Display of grid state after each generation
- Basic interactive controls (optional) to set initial configuration or number of generations

## Getting Started

### Prerequisites

Ensure that you have a C++ compiler installed. If you don't have one, you can install a popular option like **GCC** (Linux/macOS) or **MinGW** (Windows).

### Installation

1. Clone this repository:

   ```bash
   git clone https://github.com/your-username/game-of-life.git
   ```

2. Navigate to the project directory:

   ```bash
   cd game-of-life
   ```

3. Compile the program:

   ```bash
   g++ -o game_of_life main.cpp
   ```

4. Run the simulation:

   ```bash
   ./game_of_life
   ```

### Usage

- The program will display the grid of cells at each iteration.
- You can customize the grid size and initial configuration as needed (modify the `main.cpp` file).

## Example

**Initial Configuration:**

```cpp
0 0 0 0 0
0 1 1 0 0
0 0 1 0 0
0 0 0 0 0
```

**After one iteration:**

```cpp
0 1 1 0 0
0 1 1 0 0
0 0 1 0 0
0 0 0 0 0
```

## Contributions

Feel free to fork this project, report bugs, or submit pull requests.

## License

This project is open source and available under the MIT License.
