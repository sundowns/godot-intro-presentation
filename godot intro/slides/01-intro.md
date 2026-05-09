# The Node-Tree Architecture

### Everything is a Node
* Godot uses a **Scene Tree**.
* **Composition over Inheritance**: Build complex entities by nesting specialized nodes.

<div class="mt-16">
<p class="text-sm opacity-60 mb-2">Example: "Monster" Scene Tree</p>

```text
Monster
├── Sprite2D
├── CollisionShape2D
└── Hand (Node2D)
    └── Sword (Scene)
```
</div>

