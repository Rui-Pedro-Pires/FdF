# FDF Project - "Bringing 3D Landscapes to Life"

## Project Overview
This project involves creating a **3D wireframe model** of a landscape from a grid of points using the **MiniLibX** graphical library. The goal was to render a 3D landscape in **isometric projection** based on data provided in a `.fdf` file, which contains a matrix of altitude points.

---

<img src="https://github.com/Rui-Pedro-Pires/FdF/blob/main/Screenshot%20from%202024-09-25%2011-40-15.png">

---
## Design and Development
### 1. **File Parsing**
The input is an `.fdf` file with a matrix of numbers representing the height of each point in the landscape. I implemented file reading using `get_next_line`, and parsed the numbers into a 2D array using `ft_split`.

### 2. **Isometric Projection**
I used isometric projection to convert 3D points (x, y, z) into 2D coordinates for rendering. The projection gives the illusion of depth, making the 3D wireframe appear in a 2D window.

### 3. **Rendering with MiniLibX**
Each point in the 3D model is connected by lines to its neighbors, forming a grid-like wireframe. I used **MiniLibX** to open a window and draw the lines between points.

### 4. **Window Management**
The program opens a window where the landscape is displayed. I added event handling to:
- Close the window when the **ESC** key is pressed.
- Ensure the window closes properly when the user clicks the close button.

## Key Challenges
- **File Parsing**: Ensuring that the input file is read correctly and handling any formatting issues.
- **Memory Management**: Preventing memory leaks by freeing all dynamically allocated memory.
- **Projection and Rendering**: Properly mapping 3D coordinates to a 2D plane for smooth rendering.

## Bonus Part
For the bonus, I added:
- **Zoom**: Allowing the user to zoom in and out of the 3D model.
- **Translation**: Enabling the user to move the model within the window.

## How to Compile and Run

### Compilation
To compile the project:
```bash
make
```

### Running the Program
To run the program:
```bash
./fdf [file.fdf]
```

Example:
```bash
./fdf example.fdf
```

This runs the program using a `.fdf` file, rendering the 3D landscape in an isometric view.
