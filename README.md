
# FDF

## Description
FDF is a project I worked on to represent a landscape as a wireframe 3D model. The main goal is to display a 3D object where all surfaces are outlined in lines, giving a dynamic, graphical representation of terrain or landscape data using points and lines. This project helped me understand basic graphics programming using the MiniLibX library and how to manipulate points in space, connect them, and visualize the scene from various angles.

## Features
- Wireframe model rendering of a landscape from a .fdf file.
- Isometric projection to give a pseudo-3D view of the landscape.
- Dynamic rendering of points in space based on x, y, and z coordinates.
- Handling basic events like window resizing and exiting via ESC or window close button.

### Map Format
- The .fdf file represents a grid of points:
  - Horizontal and vertical positions correspond to x and y coordinates.
  - The numbers represent the altitude (z) at each point, creating a 3D effect.

- Here’s an example of a simple map:
  ```
  0 0 0 0 0 0 0 0 0 0 0 0 0
  0 0 0 0 0 0 0 0 0 0 0 0 0
  0 0 10 10 0 0 10 10 0 0 10 10 0
  ...
  ```

## Bonus Features
I also added the following bonuses:
- Additional projections like parallel or conic projection.
- Zooming in and out of the model.
- Translating and rotating the model.
- Any extra features that could enhance the wireframe model visualization.

## Installation
To install and run the project, follow these steps:

1. Clone my repository:
   ```bash
   git clone https://github.com/your-username/cub3D.git
   ```
2. Move to the project directory:
   ```bash
   cd FDF
   ```
3. Compile the project with the provided `Makefile`:
   ```bash
   make
   ```

## Usage
To render the 3D model, run the following command with a `.fdf` file:
```bash
./fdf path/to/map.fdf
```

### Controls:
- Mouse and keyboard inputs can be added to control zoom, rotation, and translation.
- Press `ESC` to close the window and exit.

## Requirements
- C programming language.
- MiniLibX library for graphics rendering.

## External Functions
I used the following external functions:
- System calls like `open`, `close`, `read`, `write`, `malloc`, `free`, `exit`.
- Functions from the math library (`-lm`).
- Functions from the MiniLibX library.

## License
This project is licensed under the MIT License.

