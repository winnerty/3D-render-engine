# Simple 3D renderer in pure Java

This project is a small educational **software 3D renderer** implemented in pure Java, without OpenGL or external libraries. It demonstrates how basic 3D graphics work under the hood.

## Features
- Rotation of the 3D object via two sliders:
    - **Heading** (Y-axis)
    - **Pitch** (X-axis)
- Manual implementation of:
    - 3×3 rotation matrices
    - Vertex transformation
    - Triangle normals (cross product)
    - Basic lighting
    - Barycentric rasterization
    - Z-buffer depth testing

## Project Structure
- **DemoViewer.java** - UI and rendering loop
- **Matrix3.java** - matrix math
- **Vertex.java** - 3D vector
- **Triangle.java** - colored triangle

## How It Works
1. Vertices are rotated using custom matrices.
2. Triangle normal and light intensity are computed.
3. Pixels are filled using barycentric coordinates.
4. Z-buffer resolves depth.
5. Final image is drawn to a `BufferedImage`.

## Run
1. Open the project in any Java IDE.
2. Run `DemoViewer.main()` (Java 8+).