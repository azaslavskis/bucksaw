Bucksaw Desktop
Fork of Bucksaw with Material UI and desktop app integration

Tool for analyzing flight logs from drones using Cleanflight-family firmwares like Betaflight and INAV. Designed to help assess vibration patterns and PID tuning performance. This fork replaces the web-based UI with a modern Material UI-based desktop application, offering a more integrated and responsive experience on your local machine.

✨ Key Differences from Original:
Fully packaged desktop application using Material UI.

No need to run a web browser — everything runs as a native GUI app.

Improved user experience with a sleek, responsive Material Design interface.

Built on the same Rust backend for fast, local FFT and analysis processing.

🔧 Setup Instructions
1. Rust Backend
Ensure Rust is installed:

bash
Copy
Edit
https://rustup.rs/
Build and run the backend in debug mode:

bash
Copy
Edit
cargo run
Install the backend binary if needed:

bash
Copy
Edit
cargo install --path .
2. Frontend (Material UI + App Framework)
This fork uses a React + Material UI frontend. To develop:

bash
Copy
Edit
cd frontend
npm install
npm run dev  # or use your chosen app framework's dev command
3. Packaging as Desktop App
Depending on your app wrapper:

With Tauri (recommended for Rust projects)
bash
Copy
Edit
npm run tauri dev       # Live-reload for development
npm run tauri build     # Create a native build (Windows/macOS/Linux)
With Electron
bash
Copy
Edit
npm run electron-dev    # Development mode
npm run electron-build  # Package for distribution
🚀 Features
View detailed FFT data for vibration analysis.

Compare PID tuning across multiple flights.

Works entirely offline – your log files never leave your device.

Efficient and smooth performance with native hardware acceleration.

Compatible with .bfl and .csv log files.

📸 Screenshot


📝 Credits
Original project by @KoffeinFlummi.
This fork adds Material UI integration and desktop packaging for a standalone user experience.

Let me know if you'd like a full folder structure or sample tauri.conf.json and package.json for a complete starter repo.




You said:
not tauri. using egui + material theme

ChatGPT said:
Thanks! Since you're building a native desktop app using Rust + egui (with a Material Design theme), here's a rewritten version of the Bucksaw project description tailored for your fork:

Bucksaw Desktop (egui + Material Theme)
Native desktop tool for analyzing drone flight logs, rebuilt with a modern, Material Design-inspired UI using egui.

This fork of Bucksaw is focused on delivering a fully native experience — no browser, no WebAssembly. It leverages Rust's speed for log processing and presents the data through a responsive, clean Material-themed interface via egui.

✨ Highlights
🖥 True native desktop app — no browser or Electron

🎨 Material Design theme built on top of egui

📈 Fast local analysis of Betaflight and INAV logs

🧠 Focus on vibration analysis and tune performance

🗂 Works offline, all data stays on your device

🛠 Setup
1. Install Rust
Get Rust at https://rustup.rs

2. Build & Run
Clone the repository and run:

bash
Copy
Edit
cargo run --release
To install the app system-wide:

bash
Copy
Edit
cargo install --path .
This will build a native binary for your system.

📂 Features
Load and analyze .bfl or .csv blackbox logs

Fast, local FFT processing

Visualize gyro noise, PID loops, and filter performance

Scrollable, zoomable timeline view

Material-style UI elements for a consistent look

💻 Screenshots
(Update this section with screenshots of the new egui-based interface)

🎨 UI & Design
The UI is built using egui with a custom theme that mimics Material Design components — buttons, sliders, tab views, dialogs, and typography are styled accordingly for clarity and comfort.

📜 License & Credits
Original Bucksaw by @KoffeinFlummi

This fork: native Rust + egui + Material Design theme

Let me know if you want help building out the egui layout, theming your components to match Material Design (e.g., color palettes, elevation, shadows), or adding packaging with cargo-bundle or similar tools.




You said:
markdown 

ChatGPT said:
Certainly! Here's the Markdown version of the rewritten project description for your fork of Bucksaw using egui + Material Design theme:

markdown
Copy
Edit
# Bucksaw Desktop (egui + Material Theme)

**Native desktop tool for analyzing drone flight logs**, rebuilt with a modern, Material Design-inspired UI using [egui](https://github.com/emilk/egui).

This fork of [Bucksaw](https://github.com/KoffeinFlummi/bucksaw) focuses on delivering a completely native experience — no browser, no WebAssembly. It uses Rust for high-performance log analysis and presents the data through a responsive, clean Material-themed interface powered by `egui`.

---

## ✨ Highlights

- 🖥 **True native desktop application** — no browser required
- 🎨 **Material Design-style UI** built with `egui`
- 📈 Fast, local analysis of Betaflight and INAV flight logs
- 🧠 Optimized for analyzing vibrations and PID tuning
- 🔐 Works 100% offline — your data never leaves your device

---

## 🛠 Setup

### 1. Install Rust

Install Rust from: [https://rustup.rs](https://rustup.rs)

### 2. Build & Run

Clone the repository and run:

```bash
cargo run --release
To install the app system-wide:

bash
Copy
Edit
cargo install --path .
This builds a native executable on your platform (Linux, macOS, Windows).

📂 Features
Supports .bfl and .csv blackbox logs

On-device FFT and filter analysis

Timeline views for gyro data and control loops

Interactive UI with zoom, pan, and customizable views

Material-styled UI for visual clarity and modern UX

💻 Screenshots
Insert updated screenshots here after UI customization



🎨 UI & Design
The UI is built entirely with egui, customized to emulate Material Design:

Color palette & typography inspired by Material 3

Consistent padding, spacing, and elevation

Styled components: buttons, tabs, sliders, toolbars

📜 License & Credits
Original project: Bucksaw by @KoffeinFlummi

This fork: Native egui-based UI with Material theme and desktop-first UX

🔧 Roadmap (Optional)
 Log comparison view

 Custom filter overlays

 Export plots as images or CSV

 PID tuning recommendation engine

css
Copy
Edit

Let me know if you want a matching `Cargo.toml`, a theming setup for egui, or an embedded icon/logo for app packaging.



