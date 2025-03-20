# 3D Object Rendering with Curves

This project is an interactive web-based application for creating and visualizing 3D surfaces of revolution using different types of curves (Bezier, B-Spline, and Hermite). It allows users to manipulate control points and generate 3D objects by rotating curves around an axis.

## Features

- **Multiple Curve Types:**
  - Bezier curves
  - B-Spline curves
  - Hermite curves
  - Interactive control point manipulation

- **Surface Generation:**
  - Real-time surface of revolution generation
  - Adjustable rotation axis
  - Customizable number of segments and rotation samples
  - Toggle between wireframe and solid rendering
  - Switch between flat and smooth shading

- **Interactive Controls:**
  - Add control points with CTRL+Click (or ALT+Click, COMMAND+Click)
  - Delete control points with SHIFT+Click
  - Move rotation axis with arrow keys
  - Load preset control points (keys 1-5)
  - Toggle control lines visibility
  - Auto-mesh updating option

## Keyboard Controls

- `z`: Draw Bezier curve
- `b`: Draw BSpline curve
- `m`: Draw Hermite curve
- `=`: Increase number of segments
- `-`: Decrease number of segments
- `e`: Erase all control points
- `l`: Show/hide control lines
- `c`: Toggle closed/open curve (BSpline and Hermite only)
- `a`: Toggle rotation axis visibility
- `s`: Generate or update surface (spacebar also works)
- `w`: Toggle wireframe/solid rendering
- `f`: Toggle flat/smooth shading

## Dependencies

- Three.js - 3D graphics library
- dat.GUI - Control panel interface
- FileSaver.js - File saving functionality
- OBJExporter.js - 3D model export capability

## Getting Started

1. Clone the repository
2. Open `index.html` in a modern web browser
3. Use the keyboard controls and mouse to create and manipulate curves
4. Generate surfaces of revolution using the 's' key or spacebar

## Technical Details

The application uses HTML5 Canvas for 2D curve visualization and Three.js for 3D surface rendering. It implements:
- Bezier curve computation
- B-Spline curve algorithms
- Hermite curve interpolation
- Surface of revolution generation
- Real-time 3D rendering with customizable parameters

## File Structure

- `index.html` - Main application page
- `curves.js` - Core curve computation and interaction logic
- `three.min.js` - Three.js library
- `dat.gui.min.js` - GUI control library
- `OBJExporter.js` - 3D model export functionality
- `FileSaver.js` - File saving utilities
- `preset.js` - Preset curve configurations 