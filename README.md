### Render Border

A Blender Add-on to set the [Render Region](https://docs.blender.org/manual/en/latest/editors/3dview/navigate/regions.html#render-region) precisely.

<img width="800" alt="RBORDER" src="https://user-images.githubusercontent.com/512368/122653937-75415b00-d148-11eb-8903-ae9fefa7cd5e.png">


#### Usage

The Panel is accessible via *Camera > Properties > Data > Render Border*.

![intro](https://user-images.githubusercontent.com/512368/122652262-2b537780-d13e-11eb-8a09-2ee2f1eb8635.gif)

 - **X** - Pixel distance between the left edge of the camera border and the left side of the render border
 - **R** - Pixel distance between the right edge of the camera border and the right side of the render border
 - **Y** - Pixel distance between the bottom edge of the camera border and the bottom edge of the render border
 - **T** - Pixel distance between the top edge of the camera border and the top edge of the render border
 - **Center X** - Horizontal center of the render border
 - **Center Y** - Vertical center of the render border

#### Installation

 1. Download the [latest release](https://github.com/p2or/blender-renderborder/releases)
 2. In Blender open up *User Preferences > Addons*
 3. Click *Install from File*, select `render-border.py` and activate the Add-on

#### Gotchas

You can animate/keyframe the values as usual. However, in order to **render an animation** you would have to use [Loom](https://github.com/p2or/blender-loom) or write your own python script to render single frames of the animation since Blender updates some of the render attributes *only once per render execution* due to a [current limitation](https://developer.blender.org/T47530) so unfortunately you cannot use [default animation rendering](https://docs.blender.org/manual/en/dev/render/output/render_panel.html)).
 
![Animation](https://i.stack.imgur.com/tCoxp.gif)






