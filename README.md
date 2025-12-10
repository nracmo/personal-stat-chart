# The Ultimate Stat Chart (Web + 3D Printable)

An interactive, browser-based tool that visualizes personal stats in an RPG-style radar chart. 

Beyond just visualization, this tool features a built-in **Slicer/Mesh Generator** that can instantly compile your stats into a **3D Printable STL Medallion**, complete with raised data spikes and engraved text labels—all within a single HTML file.

![Project Status](https://img.shields.io/badge/status-active-brightgreen)
![Tech](https://img.shields.io/badge/tech-Vanilla%20JS%20%7C%20SVG%20%7C%20STL%20Generation-orange)

## ✨ Features

### 🌐 Web Visualization
* **Interactive Graph:** Real-time updates as you input stats (0-10).
* **Custom Categories:** Tailored for Makers/Engineers:
    * **Technical:** Engineering, Crafting, Tech
    * **Physical:** Health, Strength, Stamina
    * **Mental:** Intelligence, Perception, Creativity
    * **Personality:** Humor, Passion, Empathy
    * **Social:** Charisma, Social Skills, Confidence
    * **Metaphysical:** Spirituality, Discipline, Luck
* **PNG Export:** Download high-resolution images of your chart.

### 🧊 3D Print Generator (STL)
* **Browser-Based Slicing:** Generates binary STL files locally in your browser using pure JavaScript.
* **Customizable Size:** Set your desired diameter (default 2 inches / 50.8mm).
* **Voxel Text Engine:** Automatically converts stat names to abbreviations (e.g., `Strength` -> `STR`) and generates 3D pixel-art text on the medallion ring without needing external font files.
* **Optimized Geometry:** Creates a flat base, a raised label ring, and data spikes designed for easy FDM printing.

## 🚀 How to Use

### Running the App
1.  Clone the repo or download `index.html`.
2.  Open the file in any modern web browser.
3.  Enter your stats in the input fields.

### Generating a 3D Print
1.  Set the **Diameter** (default is 50.8mm).
2.  Click **"Download STL"**.
3.  The browser will generate the 3D geometry (this may take 1-2 seconds) and download the file.

## 🖨️ 3D Printing Guide

The generated STL is optimized for simple filament swapping to make the text pop.

* **Layer Height:** 0.2mm recommended.
* **Infill:** 15-20%.
* **Color Swapping (Filament Change):**
    * **0mm - 3.6mm:** Base Color (The coin and label ring).
    * **3.6mm - Top:** Accent Color (The data spikes and text).
    * *Tip: Add an `M600` command or a "Pause at Height" in your slicer at **layer 18** (if using 0.2mm layers).*

## 🛠️ Tech Stack

* **HTML5/CSS3:** Flexbox layout and UI.
* **SVG:** 2D Vector graph rendering.
* **Vanilla JavaScript:** * Radial math for the polygon generation.
    * Canvas pixel-scanning for voxel text generation.
    * Raw binary STL mesh construction.

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
