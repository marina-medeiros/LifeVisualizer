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

Clone this repository:

   ```bash
   git clone https://github.com/your-username/game-of-life.git
   ```

### Compiling and Runnig

To compile and run the game, follow these steps:

1. Ensure you have CMake installed on your system.
2. Clone the repository to your local machine.
3. Navigate to the project directory in your terminal.
4. Go into the source file: `cd source`
4. Create a build directory: `mkdir build && cd build`.
5. Generate the build files with CMake: `cmake ..`.
6. Compile the project: `cmake --build .`.
7. Run the compiled executable: `./glife`. followed by the path of the config file (e.g. './glife ../config/glife.ini').

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
