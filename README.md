# 🌸 Seasons & You (2D Mobile & PC Platformer)

> **Cross-Platform Story-Driven Platformer Game**  
> *A 5-level mobile-first web platformer built with Kaplay.js, featuring responsive multi-touch controls, dynamic music transitions, and interactive typewriter UI systems.*

🎮 **[Live Demo / Oyunu Oyna](https://violetofnight.github.io/seasons-kaplay-mobile-pc-platformer/)**

---
![alt text](image.png)
---

## 📌 Project Overview

**Seasons & You** is a story-driven 2D platformer game that progresses through 5 unique seasonal levels. The project was engineered to deliver a fluid, high-performance web-based gaming experience across both mobile touchscreens and desktop keyboards.

---

## 🛠️ Technical Highlights & Engineering Challenges

* **Responsive Multi-Touch Architecture:** Replaced default DOM touch handlers with a custom `Map`-based multi-touch state management system. This eliminates touch lag and allows simultaneous movement and jump inputs on mobile devices.
* **Dynamic Typewriter & Sizing System:** Implemented a custom typewriter algorithm for dialogue and item pickup messages (`currentLevel.songName`). Text background panels dynamically recalculate their bounds and scale responsiveness based on active string length at `%25 opacity`.
* **Smooth Audio Tweening:** Music transitions between levels utilize linear interpolation (`tween`) for seamless fade-in/fade-out audio state management.
* **Strict Z-Index Hierarchy Layering:** Resolved UI component overlap conflicts (e.g., control buttons appearing over dialogues or level completion collages) by establishing a strict `z-index` structure:
  - `z(100)`: HUD & Mobile Controls
  - `z(500)`: End-level Collages
  - `z(1010)`: Dialogue Panels & Story Elements

---
![alt text](<Ekran görüntüsü 2026-07-28 012906.png>)
---

## 🚀 Tech Stack

* **Engine:** [Kaplay.js](https://kaplayjs.com/) (Kaboom.js ecosystem)
* **Language:** JavaScript (ES6+)
* **Rendering:** HTML5 Canvas
* **Hosting & CI/CD:** GitHub Pages

---

## 💡 AI-Driven Pair Programming

This project was developed using an **AI-Driven Pair Programming (Gemini)** approach. Complex edge cases—such as multi-touch input conflict resolution, UI layer ordering, and dynamic audio-visual synchronizations—were designed, debugged, and optimized through iterative prompt engineering and interactive code refinement.

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).