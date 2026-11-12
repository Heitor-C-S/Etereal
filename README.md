*Read this in other languages: [English](README.md), [Português](README.pt.md).*

# Etereal

> Transforming movement into music through computer vision.

**Etereal** is an experimental project that uses computer vision to track hand gestures and body movements, converting them into real-time musical and sonic parameters. Inspired by the Theremin, the project allows music to be played entirely "in the air," with no physical contact required.

## 🗺️ Development Roadmap & Proof of Concept

The project is structured in phases to ensure reliable audio synthesis before scaling interface complexity:

### Phase 1: MVP - Linear Gestural Synth (Current Focus)
The "Hello World" of this PoC focuses on generating basic chords (e.g., C Major triad in the 3rd octave: C3, E3, G3) with independent hand tracking:
* **Primary Hand (Root/Degree):** Selects the scale degree (e.g., 2nd, 3rd, 4th) relative to a base scale using linear spatial zones.
* **Secondary Hand (Modifier):** Acts as a chord quality modifier, altering the base triad into a minor, major 7th, minor 7th, or dominant 7th chord based on specific hand gestures.
* **Audio Engine:** Reliable real-time audio synthesis (3-voice polyphony for triads) without buffer underruns.

### Phase 2: Dynamic Radial Interface
An evolution of the spatial UI to allow cleaner transitions and deeper expression:
* **Radial Interface (Right Hand):** The screen is divided into a 7-slice circle (A through G) with a central "deadzone".
  * **Root Selection:** The hand's angle relative to the center (polar coordinates) selects the root note.
  * **Deadzone:** Returning the hand to the center acts as a rest state, silencing the audio to allow clean transitions between non-adjacent chords.
  * **Modifiers (Gestures):** Finger gestures on the same hand (e.g., pinching the thumb and other fingers) alter the chord quality in real-time.
* **Continuous Expression (Left Hand):** Operates on the vertical axis (Y) for dynamic volume control, simulating the classic behavior of a Theremin.

## 🛠️ Technology Stack

* **Language:** Python (with a potential fallback to TypeScript)
* **Computer Vision:** MediaPipe / OpenCV
* **Sound Generation:** Algorithmic real-time synthesis via code (e.g., `pyo`, `numpy` + `sounddevice`)

## ⚙️ Installation & Usage

*(Instructions for cloning, installing dependencies, and running the project will be added as development progresses).*

## 📄 License

This project is licensed under the [PolyForm Noncommercial License 1.0.0](https://polyformproject.org/licenses/noncommercial/1.0.0/). Use, modification, and distribution are permitted exclusively for non-commercial purposes.
