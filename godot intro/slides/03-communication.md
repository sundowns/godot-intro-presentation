# Signals & Exports

### Decoupling Logic
* **Signals (Observer Pattern)**: Nodes emit events; others listen.
* **Rule of Thumb**: "Signal Up, Call Down".

### Configuration
* **Exports**: Expose variables to the Inspector.

```gdscript
@export var speed = 400
@export var rotation_speed = 1.5

signal health_depleted(final_value)

func take_damage(amount):
    health -= amount
    if health <= 0:
        health_depleted.emit(health)
```

<img src="/images/exports.png" class="h-40 mx-auto mb-8" />