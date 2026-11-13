# LuxShot

**LuxShot** is a fast, lightweight, and modern X11 region-screenshot utility written in Rust. Designed specifically with lightweight window managers like Fluxbox (and MX Linux) in mind, it provides smooth click-hold-release region selection, instant clipboard integration, and automatic shortcut configuration.

---

## Features

- **Intuitive Region Selection:** Click-hold and drag with live visual feedback to capture precisely the area you want.
- **Automatic Keybind Setup:** Instantly integrates with Fluxbox (`Mod4 s` / `Super + s`) on first run.
- **Dual Output:** Automatically saves high-resolution PNGs to your `~/Pictures` directory *and* copies the image data straight to your system clipboard.
- **Native Notifications:** Triggers a desktop notification confirming where your screenshot was saved.
- **Escape to Abort:** Press `Escape` at any time during capture to cancel cleanly.
- **Lightweight & Fast:** Built in Rust using `eframe`/`egui` and `xcap` for blazing-fast performance with minimal resource overhead.

---

## Installation & Building

To build and install LuxShot from source on an X11 Linux system, make sure you have Rust and `cargo-deb` installed.

### Prerequisites
Ensure you have the necessary X11 development libraries installed (standard on most distros):
```bash
sudo apt install build-essential libxcb-render0-dev libxcb-shape0-dev libxcb-xfixes0-dev libx11-dev
