<div align="center">
  <img src="Resources/crosshair.ico" alt="VCross Logo" width="120" />
  <h1>VCross</h1>
  <p><strong>A professional, high-performance Windows crosshair overlay with native click-through support and a glowing 'Universe' aesthetic.</strong></p>
</div>

---

## 🚀 Features

- **Hardware-Accelerated Overlay**: Written in .NET 8 WPF, ensuring zero-latency, pixel-perfect rendering that stays on top of any borderless/windowed game.
- **True Click-Through**: Utilizes Win32 `WS_EX_TRANSPARENT` so your mouse never accidentally interacts with the overlay during frantic gameplay.
- **✨ Animation Engine**: The crosshair natively responds to your mouse inputs (via `WH_MOUSE_LL`).
  - **Fire Expand**: Replicates weapon recoil by expanding the crosshair instantly on Left-Click.
  - **Scope Collapse**: The bars glide smoothly to the center and fade out while holding Right-Click.
- **RGB Chroma Mode**: Syncs with `CompositionTarget.Rendering` for a smooth, hardware-vsync tied HSL-to-RGB color cycle.
- **Live Customization**: Instantly tweak Gap, Thickness, Length, Opacity, Rotation, Dot Size, Outline, and animation durations.
- **20 Vector Presets**: From the generic Classic Cross to specialized T-Shapes, Sniper Dots, and KovaaK layouts.
- **JSON Profiles**: Share your crosshairs easily with other players via import/export config `.json` files.

---

## 🎨 The "Universe" Theme
The Control Center UI features a stunning dark purple glassmorphism aesthetic (`#0A0A0B` / `#6A0DAD`), with neon-glowing sliders and hover micro-animations, designed to look like modern esports center control software.

---

## 🛠️ Coming Soon: "VCross Nexus"
We are currently working on **Phase 2**, which introduces the **VCross Nexus Discord Bot**. 
* **Visibility Lab**: The bot grades your crosshair code against challenging background snapshots (snow, shadows, grass).
* **Live Sharing**: Auto-generate beautiful preview cards of your crosshair in your Discord server.
* **Remote Control**: Switch presets directly from your phone while playing.

*(Read the full vision in [Roadmap.md](Roadmap.md))*

---

## 🖥️ Requirements
- Windows 10/11
- .NET 8.0 Desktop Runtime

## 🚀 How to Run
```powershell
# Clone the repository
git clone https://github.com/yourusername/VCross.git
cd VCross

# Run directly
dotnet run

# Or build a standalone single-file EXE for distribution
dotnet publish -c Release -r win-x64 --self-contained true -p:PublishSingleFile=true
```
