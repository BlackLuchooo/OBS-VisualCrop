# VisualCrop.html (v1.2 Stable)

A specialized tool for OBS Studio that provides a visual, interactive interface for cropping and scaling sources. Designed to be used as a **Custom Browser Dock** directly inside OBS.

---

## 🚀 Overview
**VisualCrop** eliminates the need to manually enter pixel values in the "Edit Transform" window. It provides a real-time "WYSIWYG" (What You See Is What You Get) monitor where you can drag a selection box to crop your sources instantly.

---

## 🛠 Setup as OBS Custom Dock (Recommended)
For the best experience, integrate **VisualCrop.html** directly into your OBS interface:

1.  **Open OBS Studio.**
2.  Go to the top menu: `Docks` -> `Custom Browser Docks...`.
3.  **Dock Name:** `Visual Crop`.
4.  **URL:** Click the `...` button to browse and select your `VisualCrop.html` file, or paste the local path (e.g., `C:/Users/Name/Documents/VisualCrop.html`).
5.  Click **Apply**.
6.  **Dock it:** Drag the new window and snap it anywhere in your OBS layout (e.g., next to your Sources or Mixer).



---

## ✨ Key Features
* **Visual Interaction:** Drag the green selection box to reposition your crop.
* **Smart Zoom:** A dedicated slider that zooms in/out while maintaining the aspect ratio and automatically adjusting OBS scale.
* **Live Preview:** Periodic screenshots of the active source displayed directly in the dock.
* **Auto-Reconnect:** Remembers your WebSocket IP and Password for seamless sessions.
* **Vertical Resize:** The preview area adjusts its height to fit your custom dock size.

---

## 📖 How to Use
1.  **Connect:** Open the settings (⚙️) inside the dock, enter your WebSocket password, and connect.
2.  **Select:** Click on any source in your OBS **Sources list**. The tool will automatically sync.
3.  **Adjust:**
    * **Drag** the rectangle to move the visible area.
    * **Zoom Slider:** Use "Smart Zoom" to enlarge the crop without losing your canvas scale.
    * **H/V Sliders:** Fine-tune the horizontal and vertical offsets.

---

## ⚙️ Requirements
* **OBS Studio 28.0+** (WebSocket v5 is built-in).
* **WebSocket Enabled:** `Tools` -> `WebSocket Server Settings` -> `Enable WebSocket Server`.

## ⚠️ Known Limitations
* **Groups:** Currently optimized for top-level sources. Support for nested sources inside groups is limited due to OBS WebSocket event reporting.

---
**Developed by BlackLuchooo**
*Optimized for OBS Studio Workflow*
