*Read this in other languages: [English](README.md), [Português](README.pt.md).*

# Etereal

> Transforming movement into music through computer vision.

**Etereal** is an experimental project that uses computer vision to track hand gestures and convert them into a real-time musical synthesizer. Inspired by instruments like the Theremin, the project allows music to be played entirely "in the air," with no physical contact required.

## 🎯 Proof of Concept (PoC)
The initial prototype functions as a gestural chord synthesizer with independent hand tracking. The "Hello World" of this PoC focuses on generating a basic C Major triad in the 3rd octave (C3, E3, G3).
* **Primary Hand (Root/Degree):** Selects the scale degree (2nd, 3rd, 4th, etc.) relative to a base C Major scale.
* **Secondary Hand (Modifier):** Acts as a chord quality modifier, altering the base triad into a minor, major 7th, minor 7th, or dominant 7th chord based on specific hand gestures.

## 🛠️ Technology Stack
* **Language:** Python (with a potential fallback to TypeScript)
* **Computer Vision:** MediaPipe / OpenCV
* **Sound Generation:** Algorithmic real-time synthesis via code (e.g., `pyo` or `sounddevice`)

## ⚙️ Installation & Usage
* **Work in progress...**

## 🗺️ Development Roadmap

* **Phase 1: MVP - Linear Gestural Synth (Current Focus)**
  * Basic independent hand tracking.
  * Primary Hand: Linear/zone-based selection of scale degrees (e.g., C, D, E).
  * Secondary Hand: Gesture-based chord quality modifiers (Major, Minor, 7th).
  * Reliable real-time audio synthesis (3-voice polyphony for triads).

* **Phase 2: Dynamic Radial Interface**
  * Implementation of a circular spatial UI with a central "deadzone" for clean chord transitions.
  * Continuous dynamic expression (e.g., Y-axis for volume control, similar to a Theremin).
  * Advanced modifiers via single-hand finger pinching gestures.

*(Instructions for cloning, installing dependencies, and running the project will be added as development progresses).*

## 📄 License

This project is licensed under the [PolyForm Noncommercial License 1.0.0](https://polyformproject.org/licenses/noncommercial/1.0.0/). Use, modification, and distribution are permitted exclusively for non-commercial purposes.
