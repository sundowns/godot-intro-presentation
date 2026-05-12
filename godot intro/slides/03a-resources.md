# Resources: Data-Driven Design

### What are Resources?
* Dedicated data containers (`.tres` files).
* Shared across multiple instances (Flyweight pattern).
* Examples: textures, scripts, curves, custom data.

Or.... *custom* resources:
```gdscript
# stats_resource.gd
extends Resource
class_name MonsterStats

@export var health: int = 100
@export var speed: float = 200.0
```

```gdscript
# monster.gd
extends CharacterBody2D

@export var stats: MonsterStats # Swap 'Goblin.tres' for 'Dragon.tres'
```
