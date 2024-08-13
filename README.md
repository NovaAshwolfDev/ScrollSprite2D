# ScrollSprite2D for Godot 4.2/4.3

## Overview

`ScrollSprite2D` is a GDExtension for Godot Engine versions 4.2 and 4.3. It introduces a custom [node](https://docs.godotengine.org/en/stable/classes/class_node.html)  that allows for advanced scrolling and tiling of textures in 2D scenes. This extension is particularly useful for developers who need to create infinite scrolling backgrounds, parallax effects, or tiled textures in their games or applications.

## Features

- **Customizable Scrolling:** Adjust the scroll speed in both the X and Y directions to create smooth scrolling effects.
- **Tiling Support (Not Fully Working Yet):** Specify the number of tiles to render, allowing for dynamic and infinite scrolling backgrounds.
- **Zoom Support:** Adjust the zoom level of the texture for different effects.

## Installation

To install the `ScrollSprite2D` GDExtension:

1. Clone the repository into your Godot project directory.
    ```bash
    git clone https://github.com/NovaTheFurryDev/ScrollSprite2D.git
    ```
2. Open your Godot project and navigate to the `Project Settings` to enable the `ScrollSprite2D` extension.
3. Add the `ScrollSprite2D` node to your scene from the node tree.

## Usage

Once installed, the `ScrollSprite2D` node can be added to your scene like any other Godot node. Here's how you can use it:

1. **Adding to the Scene:**
   - In the scene tree, right-click and select `Add Node`.
   - Search for `ScrollSprite2D` and add it to your scene.

2. **Configuring Scroll Settings:**
   - Adjust the `ScrollSpeedX` and `ScrollSpeedY` properties to control the speed of the texture scrolling.
   - Set the `Amount` property to determine the number of tiles to render.

3. **Adjusting Zoom:**
   - Use the `Zoom` property to change the scale of the texture, creating different visual effects.

4. **Example:**
   ```gdscript
   var scroll_sprite = ScrollSprite2D.new()
   scroll_sprite.ScrollSpeedX = 2.0
   scroll_sprite.ScrollSpeedY = 1.5
   scroll_sprite.Amount = 3
   add_child(scroll_sprite)
# Still WIP 
