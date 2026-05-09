# Scenes as Instantiable Modules

### Scenes = Classes
* A Scene is a saved branch of the tree.
* Acts as a **Blueprint** or **Class**.

### Encapsulation
* A "Level" scene instances "Player" and "Enemy" scenes.
* **Recursive Design**: You can run any scene independently for unit testing and debugging.

<div class="mt-8 flex justify-center items-center gap-8">
  <div class="border p-4 rounded bg-gray-800">Player.tscn</div>
  <div class="text-2xl">→</div>
  <div class="border p-4 rounded bg-gray-800">Main.tscn</div>
</div>
