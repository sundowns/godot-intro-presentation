# Signals: The Observer Pattern

* Nodes emit events; others listen.
* **Rule of Thumb**: "Signal Up, Call Down".

```gdscript
# Monster.gd
signal health_depleted(final_value)

func take_damage(amount):
    health -= amount
    if health <= 0:
        health_depleted.emit(health)
```

```gdscript
# Level.gd (Parent)
func _ready():
    # Connect the signal via code or the Editor UI
    $Monster.health_depleted.connect(_on_monster_dead)

func _on_monster_dead(value):
    print("Game Over!")
```
