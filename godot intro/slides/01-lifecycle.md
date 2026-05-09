# Node Lifecycle

The most common entry points for logic:

```gdscript
extends Node

# Called once when the node and its children enter the scene tree.
func _ready():
    # Setup and initialization
    pass

# Called every frame. 'delta' is the time elapsed since the previous frame.
func _process(delta):
    # Update logic (UI, non-physics movement, etc.)
    pass

# Called at a fixed rate (60 FPS by default). Used for physics logic.
func _physics_process(delta):
    # Physics calculations and movement
    pass

# Called when an input event (mouse, keyboard, etc.) occurs.
func _input(event):
    # Handle discrete events (e.g., button press)
    pass
```
