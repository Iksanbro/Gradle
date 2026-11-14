# Wire Mod

**Visible redstone wires for Create and Create Aeronautics.** Connect any block face to any other block face — no connector blocks. Hang wires or lay them along blocks, copy them with Create schematics, fly them on Sable ships, run them from the ground to a ship on a rope — and control everything with a **keyboard, mouse or gamepad**.

---

## ✨ Features

### 🔌 Wires from face to face
- **Right click** a block face with a Signal Wire to pick the source, then right click the target faces. One source can feed many targets.
- **Any block receives the signal**: lamps, pistons, doors, Create machines — no connector block needed.
- The **signal strength 0–15 is kept**. Several wires into one face take the maximum. Wires can be chained.
- Plugs are colored by role: copper — source, blue — target, purple — both. A powered wire is brighter.
- **Dye** a source plug to recolor its wires.

### 〰️ Two ways to lay a wire
- **Hanging:** the wire sags between its ends and goes through blocks.
- **Along blocks:** the wire is laid on surfaces in straight lines and finds its own way around walls, like Create: Power Grid cables.
- **Waypoints:** Sneak + right click a block while a source is selected — the wire will go through that point.
- The preview shows the route before you connect.

### 📐 Create schematics
- Wires are saved with **Schematic and Quill**, rotated and mirrored with the schematic.
- The **Schematicannon prints them**, using 1 wire per connection.

### 🛩️ Sable and Create Aeronautics ships
- Wires inside one ship keep working through **assembly, flight, rotation and disassembly**.
- Ground ↔ ship and ship ↔ ship links need the **Signal Cable**: tie a rope (Rope Coupling) between two holders, then right click both holders with the cable. The cable winds around the rope.
- Cut the rope — the cable drops as an item. An ordinary wire that ends up between the ground and a ship breaks and is refunded.
- **Lasers** (laser pointer, laser and optical sensors) pass through wire plugs.

### ⌨️ Signal Typewriter
- **Every key is a channel.** Right click the typewriter with a wire, press a key — the wire carries that key.
- Mouse support: **mouse buttons**, **wheel** (a short pulse per click) and **mouse movement** (an analog 0–15 signal by speed).
- Right click with an empty hand to start typing; **Esc** to stop. Only wired keys go to the wires — **the rest works as usual** (move, jump, inventory, hotbar).
- **Sneak + right click** opens the channel modes: **Button** (on while held) or **Lever** (one press on, the next off); for mouse movement — **Speed** or **Joystick** (holds the offset).
- The HUD shows the wired keys and what is pressed.

### 🎮 Gamepad Receiver
- A controller drives the wires: **buttons** work like keys, **sticks and triggers** give an analog **0–15 signal by deflection** (with a dead zone).
- Keyboard and mouse stay with the game while you use it.

### ⚡ Fast and safe
- Typewriter and gamepad signals reach the wires **at once**, not on the next tick.
- Settings, levers and the current typing session **survive ship assembly and disassembly**.
- 200+ active wires cost about 1 ms of mod code per tick.

---

## 🚀 Quick start
1. Craft **Signal Wire**.
2. Right click the face of a lever, then the face of a lamp. Flip the lever.
3. **Sneak + right click in the air** — reset the wire you are laying. **R** — switch hanging / along blocks.
4. **Left click** a plug to remove its wires (they are refunded).

For a typewriter: place it, right click it with a wire, press **W**, right click a lamp — then right click the typewriter with an empty hand and hold **W**.

---

## 🧰 Recipes
- **Signal Wire ×8:** copper ingot + redstone + dried kelp (shapeless).
- **Signal Cable:** 2 Signal Wires + string (shapeless, needs Create Aeronautics).
- **Signal Typewriter:** paper / 3 buttons / iron ingot, Signal Wire, iron ingot.
- **Gamepad Receiver:** lightning rod / button, Signal Wire, button / 3 iron ingots.

---

## 📦 Requirements
- Minecraft **1.21.1**, NeoForge **21.1.228+**
- **Create** 6.0.x

## 🔌 Optional
- **Sable** 2.x — wires on physics ships (sub-levels)
- **Create Aeronautics** 1.3.x — Signal Cable on ropes, lasers, Physics Assembler

## ⚙️ Config
`config/wiremod-common.toml`: `maxWireLength`, `strongPower`, `consumeWire`.
`config/wiremod-client.toml`: `wireSegments`, `sagFactor`, `wireThickness`.
The mode key (**R**) can be rebound in Controls → Wire Mod.

## ⚠️ Known issues
- Pistons and Create contraptions (not Sable ships) do not move wire plugs: the wire breaks.
- While typing, a wired key belongs to the typewriter: a wire on **W** or **E** stops it from moving you or opening the inventory.
- The Gamepad Receiver was tested with a virtual gamepad only. It uses the standard GLFW gamepad mappings (Xbox, PlayStation, Switch Pro and others).

---

## 🌐 Languages
English, Russian.

## 📄 License
MIT. Bundles the **Sable Companion** library (MIT, by RyanHCode) via jar-in-jar; no other mods are bundled.

---

*This mod was made 100% by AI.*
