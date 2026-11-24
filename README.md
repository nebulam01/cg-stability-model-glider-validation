# CG Position Stability Model & Safe Glider Validation

An interactive **Google Colab** engineering tool built with `ipywidgets`, `NumPy`, `Pandas`, and `Matplotlib` to model how **center-of-gravity (CG) position** affects longitudinal stability and validate the model against a **safe glider test**[cite: 4].

## Overview

Moving the center of gravity forward or aft relative to the neutral point changes static margin, pitch restoring stiffness, and damping behavior[cite: 4]. This notebook lets you adjust CG position (`% MAC`), test against a simulated safe glider launch or enter a manual test peak angle, inspect a 2D glider layout alongside a model-vs.-test response plot, and read a cause-and-effect explanation of why the result occurred[cite: 4].

### Stability & Validation Modes
- **CG Position (`% MAC`):** Shifts CG relative to a `35% MAC` neutral point reference to inspect positive static margin (stable), low margin (marginally stable), and aft CG (unstable/oscillatory) regimes[cite: 4].
- **Validation Source:** Compare the stability model against a **Simulated Safe Glider Test** or a **Manual Glider Test Peak `[deg]`** input[cite: 4].

## Key Features

- **Interactive English UI (`ipywidgets`):** Adjust `CG Position [% MAC]`, `Validation Source`, and `Manual Test Peak [deg]` sliders, updating live or via **Run CG Validation**.
- **2D Glider Layout & Validation Chart:** Displays a 2D side-view glider layout marking `CG` and `Neutral Point` alongside the `Stability Model Pitch` vs. `Safe Glider Test Pitch` graph[cite: 4].
- **Stability Verdict & Cause-and-Effect Explanation:** Reports `Stability Verdict`, `Static Margin`, and `Validation RMSE`, paired with a clear explanation of why the behavior happened[cite: 4].

## How to Run in Google Colab

1. Open a new notebook in [Google Colab](https://colab.research.google.com/).
2. Paste the CG stability & glider validation code into a code cell and run it[cite: 4].
3. Adjust CG location and validation inputs to observe stability changes and model-to-test agreement[cite: 4].

## Engineering Notes

- Real glider pitch stability also depends on wing/tail aspect ratios, airspeed, trim settings, and hand-launch release conditions; use this tool to build stability intuition and cross-check safe low-energy glider tests[cite: 4].
