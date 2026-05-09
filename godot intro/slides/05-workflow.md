# The Engineering Workflow

### Tools & Integration
* **Git Friendly**: `.tscn` and `.tres` are human-readable text files (TOML-like).
* **Small Footprint**: Single ~100MB executable; no complex installation.

### Language Ecosystem
* **GDScript**: Python-like, optimized for the engine.
* **C#**: First-class support via .NET 8.
* **GDExtension**: High-performance C++, Rust, or Swift bindings.

<div class="mt-8 flex justify-between gap-4">
  <div class="w-1/2 border p-2 text-xs font-mono">
    [node name="Player" type="CharacterBody3D"]
    transform = Transform3D(1, 0, 0, ...)
    script = ExtResource("1_abc")
  </div>
  <div class="w-1/2 flex items-center justify-center border bg-gray-900 rounded">
    Godot Editor UI
  </div>
</div>
