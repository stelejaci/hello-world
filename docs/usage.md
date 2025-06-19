# Usage

##Overview

To use RaTrace, follow these instructions:

1. Define the scene in a Python script by creating geometric objects and specifying their properties such as position, size, material, and lighting.
2. Use the `render` function provided by RaTrace to render the scene.
3. Optionally, adjust rendering parameters such as image resolution, anti-aliasing level, and maximum recursion depth.
4. Run the Python script containing the scene definition and rendering commands.
5. RaTrace will generate an image file (e.g., PNG) containing the rendered scene based on the specified parameters.

Example Python script (`render_scene.py`):

```python
from RaTrace import Scene, Sphere, Plane, PointLight, render

# Create a scene
scene = Scene()

# Add objects to the scene
scene.add_object(Sphere(center=(0, 0, -5), radius=1, color=(255, 0, 0), reflection=0.5))
scene.add_object(Plane(normal=(0, 1, 0), distance=-1, color=(0, 255, 0)))

# Add lights to the scene
scene.add_light(PointLight(position=(5, 5, -10), intensity=0.8))

# Render the scene
render(scene, width=800, height=600, anti_aliasing=True, max_depth=5, output_file="output.png")
```