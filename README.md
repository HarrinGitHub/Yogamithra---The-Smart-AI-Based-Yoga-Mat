# Yogamithra — The Smart AI-Based Yoga Mat

An AI-powered yoga mat that senses body position and weight distribution during practice and gives real-time feedback on posture, helping users correct their form without a live instructor in the room.

> **Heads up:** your repo currently only has a `LICENSE` file — no code has been pushed yet, so I can't pull real technical details from it. Below is a README *template* built around what "Yogamithra — Smart AI-Based Yoga Mat" implies. Swap in your actual sensors, model, and output method once the code is up, and this will read exactly like the Catalog & Order API example.

---

## What it does

Yogamithra uses an array of pressure sensors embedded in the mat surface to detect how weight is distributed across a user's pose. That sensor data is fed into a model that classifies the pose and checks it against the correct form, then gives feedback — fill in whether that's an app, LED indicators on the mat itself, audio cues, or some combination.

*(Replace this paragraph with what your build actually does — how many sensors, what poses it recognizes, and how it delivers feedback.)*

---

## What makes this more than a sensor mat

*(This is the section that makes a README interesting — the "hard part" you solved. A couple of options depending on what you built:)*

- **Pose classification under noisy sensor data** — pressure readings vary person to person (weight, foot size, flexibility), so the model needs to generalize rather than memorize one body type.
- **Real-time feedback loop** — if the mat gives corrections *while* the user holds a pose, latency and sensor-sampling rate become real engineering constraints, not just accuracy metrics.
- **Calibration** — every mat/user pairing may need a quick calibration step so the pressure baseline adapts to the person using it.

---

## Hardware

| Component | Role |
|---|---|
| Pressure sensor array (FSR or similar — confirm type) | Captures weight distribution across the mat |
| Microcontroller (Arduino / ESP32 — confirm) | Reads sensors, runs inference or forwards data |
| *(Feedback mechanism — LEDs / app / speaker?)* | Delivers corrections to the user |

---

## Tech stack

| Layer | Choice | Why |
|---|---|---|
| Sensing | *(fill in: FSR sensors, sensor count/layout)* | |
| Model | *(fill in: framework — TensorFlow Lite, scikit-learn, etc.)* | |
| Firmware | *(fill in: Arduino/ESP32 C++, MicroPython?)* | |
| App/UI | *(fill in, if applicable)* | |

---

## Getting started

*(Fill this in once code is pushed — should read like a checklist someone can follow start to finish, e.g.:)*

1. Flash the mat's firmware to the microcontroller.
2. Install the model dependencies (`pip install -r requirements.txt`).
3. Connect the mat and run the app/dashboard.
4. Step onto the mat and hold a pose to see live feedback.

---

## Roadmap

- [ ] Push the actual project code (firmware, model, app) to this repo
- [ ] Add a project description on the GitHub repo page
- [ ] Document the sensor layout and pose library supported
- [ ] Add a demo video or GIF of the mat giving live feedback
- [ ] Write up model accuracy / evaluation results

---

Built as an AI + hardware portfolio project.
