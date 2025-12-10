# The Ultimate Stat Chart (RPG Style)

A lightweight, interactive **Radar Chart (Spider Graph)** built to visualize personal stats, skills, or RPG attributes. This project uses pure HTML, CSS, and SVG to render a dynamic graph that updates in real-time as you input data.

![Project Status](https://img.shields.io/badge/status-active-brightgreen)
![Tech](https://img.shields.io/badge/tech-HTML%20%7C%20CSS%20%7C%20JS-blue)

## 📋 Overview

This tool allows users to input values (0-10) across 6 distinct categories to generate a visual "stat polygon." It is designed with a flat, modern UI and is fully self-contained in a single file—no frameworks, libraries, or build steps required.

**Live Demo:** [Insert your GitHub Pages Link Here]

## ✨ Features

* **Real-Time Visualization:** The SVG graph updates instantly as you type numbers.
* **Custom Categories:** Replaces standard "Appearance" stats with a **"Technical"** category (Engineering, Crafting, Tech) to better suit makers and developers.
* **Dynamic Scaling:** The graph axis scales automatically based on the input (0 to 10).
* **Color-Coded Groups:** Visual distinction between Physical, Mental, Social, and Technical attributes.
* **Zero Dependencies:** Built with Vanilla JavaScript and native SVG.

## 📊 The Stat Categories

The chart tracks 18 distinct attributes across 6 main groups:

1.  **Physical (Pink):** Health, Strength, Stamina
2.  **Technical (Orange):** Engineering, Crafting, Tech
3.  **Mental (Yellow):** Intelligence, Perception, Creativity
4.  **Personality (Green):** Humor, Passion, Empathy
5.  **Social (Blue):** Charisma, Social Skills, Confidence
6.  **Metaphysical (Purple):** Spirituality, Discipline, Luck

## 🚀 Quick Start

### Option 1: Run Locally
1.  Clone the repository:
    ```bash
    git clone [https://github.com/yourusername/stat-chart.git](https://github.com/yourusername/stat-chart.git)
    ```
2.  Open `index.html` in any web browser.

### Option 2: Host on GitHub Pages
1.  Go to your repository **Settings**.
2.  Navigate to **Pages**.
3.  Set the source branch to `main` (or `master`) and save.
4.  Your chart will be live at `https://yourusername.github.io/stat-chart/`.

## ⚙️ Customization

You can easily modify the categories by editing the `groups` array in the `<script>` section of `index.html`:

```javascript
const groups = [
  { 
    name: "My Custom Category", 
    class: "theme-red",
    stats: ["Stat A", "Stat B", "Stat C"] 
  },
  // ...
];
