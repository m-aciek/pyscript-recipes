# Running Python Turtle Graphics in the Browser Using PyScript

## Prerequisites
- Basic knowledge of Python
- Familiarity with HTML and JavaScript
- PyScript installed

## Directory/File Layout
```
.
├── index.html
├── main.py
├── pyscript.toml
├── svg.py
└── turtle.py
```

## `index.html` Example
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Turtle Graphics with PyScript</title>
    <script type="mpy" src="./main.py" config="./pyscript.toml"></script>
</head>
<body>
    <h1>Python Turtle Graphics in the Browser</h1>
</body>
</html>
```

## `pyscript.toml` Snippet Listing Files
```toml
[[files]]
path = "./svg.py"
[[files]]
path = "./turtle.py"
```

## `main.py` Example
```python
from turtle import *

# Draw something simple
forward(100)
right(90)
forward(100)
done()  # Ensure to call done() to finish rendering
```

## Notes About Output
- The output will be rendered as SVG graphics.
- Use `mode('logo')` to set the turtle graphics in logo mode for easier control.

## Optional Tip for Targeting a Container
You can target a specific HTML container by passing it to the `done()` function:
```python
done(target="container_id")  # Replace "container_id" with the actual id of your container
```

## Full Source Code for `svg.py`
```python
# Full implementation of svg.py if needed
class SVG:
    pass  # Add actual SVG implementation here
```

## Full Source Code for `turtle.py`
```python
# Full implementation of turtle.py if needed
class Turtle:
    pass  # Add actual Turtle implementation here
```
