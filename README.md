# Python Graphics Library

The **Python Graphics Library** is a simple, object-oriented library for creating 2D graphics in Python. Originally developed by **John Zelle**, this library has been enhanced over the years by various contributors to include additional features, improved functionality, and support for modern Python versions.

---

## Features

- **Graphical Window (`GraphWin`)**: Create and manage graphical windows for drawing.
- **Basic Shapes**: Draw points, lines, circles, rectangles, polygons, and more.
- **Rotatable Shapes**: Support for rotatable polygons and ovals.
- **Text and Input**: Add text and input fields to your graphics.
- **Images**: Load, display, and manipulate images with support for the Pillow library.
- **Mouse and Keyboard Interaction**: Handle mouse clicks, right-clicks, and key presses.
- **Coordinate Transformation**: Easily map between world and screen coordinates.
- **Animations**: Move and update graphical objects for animations.
- **Collision Detection**: Built-in methods for detecting collisions between shapes, points, and images.

---

## Installation

Place the `graphics.py` file in the same directory as your current project that is using the library. To use the classes of the library, best practice is to import it into your current project by typing:

```python
from graphics import *
```

This will give you access to the graphics module in your current Python file and any file that imports from it.

---

## Getting Started

Here is a simple example to create a graphical window and draw a circle:

```python
from graphics import *

def main():
    # Create a graphical window
    win = GraphWin("My Circle", 300, 300)

    # Draw a circle
    circle = Circle(Point(150, 150), 50)
    circle.setFill("blue")
    circle.draw(win)

    # Wait for a mouse click before closing
    win.getMouse()
    win.close()

main()
```

---

## Documentation

### Classes and Objects

The library provides the following key classes:

- **GraphWin**: The main window for displaying graphics.
- **Point**: Represents a point in 2D space.
- **Line**: Represents a line segment between two points.
- **Circle**: Represents a circle with a center and radius.
- **Rectangle**: Represents a rectangle defined by two opposite corners.
- **Polygon**: Represents a polygon with multiple vertices.
- **RotatablePolygon**: A polygon that can be rotated.
- **RotatableOval**: An oval that can be rotated.
- **Text**: Displays text at a specified location.
- **Entry**: Provides a text input field.
- **Image**: Displays and manipulates images.

For detailed documentation, refer to the [Wiki](https://github.com/snissley-edu/python_graphics/wiki).

---

## Contributors

The library was originally developed by **John Zelle** and has been enhanced by the following contributors:

- **Scott Nissley**: Current maintainer, added features such as rotatable graphics objects, right-click support, and collision detection methods.
- **Brandon Brzuszkiewicz**: Contributed active fill support and enhancements to graphical objects like `Polygon` and `RoundedRectangle`.
- **DJ Carroll**: Added image manipulation features using the Pillow library, including resizing, rotation, and collision detection for images.

---

## License

This library is open-source software released under the terms of the [GPL License](http://www.gnu.org/licenses/gpl.html).

---

## Support

If you encounter any issues or have feature requests, feel free to open an issue in the [GitHub repository](https://github.com/snissley-edu/python_graphics/issues).

---

Start creating amazing graphics with Python today!
