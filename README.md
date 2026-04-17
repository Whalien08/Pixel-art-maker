# Pixel Art Maker 

A fully interactive, browser-based drawing tool for creating and exporting pixel art. This project focuses on mastering the **HTML5 Canvas API** and implementing fundamental computer science algorithms like **Flood Fill**.

##  Live Demo
[Check out the live app here!](https://whalien08.github.io/Pixel-art-maker/)

##  Features
- **Dynamic Grid:** Supports 16x16, 32x32, and 64x64 canvases with automatic cell scaling.
- **Toolbox:** Includes Pen, Eraser, and a "Paint Bucket" (Flood Fill) tool.
- **Color Management:** 16 preset palette colors plus a custom hex color picker.
- **High-Res Export:** Saves art as clean PNG files without grid lines, scaled up for clarity.
- **UI/UX:** Dark-themed interface with translucent hover previews and clear-canvas confirmation.

##  Technical Implementation

### 1. Data Structure: 2D Array Mapping
The application state is managed via a 2D JavaScript array. Every pixel's color is stored at a specific coordinate `grid[row][col]`. 

### 2. Algorithm: Stack-Based Flood Fill
The "Fill" tool utilizes an **iterative stack-based Flood Fill algorithm**. This approach was chosen over recursion to prevent "Maximum Call Stack Size Exceeded" errors, ensuring stability on larger grids.



### 3. Coordinate Mapping
The app translates mouse click coordinates $(x, y)$ into grid indices $(row, col)$ using the following logic:

$$col = \lfloor x / cellSize \rfloor$$
$$row = \lfloor y / cellSize \rfloor$$

## 📂 Project Structure
- `index.html`: UI components and layout.
- `style.css`: Responsive dark-themed styling.
- `script.js`: Canvas rendering, event listeners, and algorithm logic.

## 🤝 Credits
Built following the **Codédex** intermediate JavaScript tutorial.
- **Tutorial:** [Build a Pixel Art Maker](https://www.codedex.io/projects/build-a-pixel-art-maker-with-html-css-and-javascript)
- **Author:** Dharmarajsinh Jethva

---
Licensed under the [MIT License](LICENSE).
