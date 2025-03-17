![Banner](https://i.imgur.com/qyWHmxW.png)

Gizmo3D encapsulates the Godot Engines 3D move/scale/rotation gizmos into a customizable node for use at runtime. The major differences are that you can edit all transformations at the same time, and customization options have been added. The selection box and axes can be toggled, colors changed, snapping intervals changed, and more. Transformation methods can be easily overriden to customize the default behavior. It is available in both C# and GDScript.

### Installation
Copy either Gizmo3DScript or Gizmo3DSharp from the addons folder into the addons folder of your project. Read more about installing and enabling addons [here](https://docs.godotengine.org/en/stable/tutorials/plugins/editor/installing_plugins.html). 

Once installed, you can add a Gizmo3D node to your project. For usage, it's recommended to take a look at the demo project - note that to use the demo you will have to **git clone** the repo, since the artifact is setup for use with the Godot Asset Library.

### Usage

| Signal            | C#                 | GDScript            |
|-------------------|--------------------|---------------------|
| Transform Begin   | `TransformBegin`   | `transform_begin`   |
| Transform Changed | `TransformChanged` | `transform_changed` |
| Transform End     | `TransformEnd`     | `transform_end`     |

| Overridable Transformation | C#                | GDScript            |
|----------------------------|-------------------|---------------------|
| Translation                | `EditTranslate()` | `_edit_translate()` |
| Scale                      | `EditScale()`     | `_edit_scale()`     |
| Rotation                   | `EditRotate()`    | `_edit_rotate()`      |

### Licensing
Gizmo3D is largely a port of C++ code from the Godot Engine source. Gizmo3D is licensed under MIT, while the license for the Godot Engine can be found [here](https://godotengine.org/license/). The demo project uses assets from Kenney's CC0 licensed [Mini Dungeon](https://kenney.nl/assets/mini-dungeon) asset pack. The banner logo uses the [Dimbo](https://www.dafont.com/dimbo.font) font.
