# Regression: y = a x (Through Origin)

Interactive web app that fits a line through the origin (y = a x) using the same single-file layout and styling as your previous app, but with a slope-only model.

## Features
- Slider for `a` (slope) with live updates
- Left plot: data and line `y = a x` with residuals
- Right plot: convex `MSE(a)` curve with current `a` and optimum `a*`
- Practice section with random datasets and revealable equation

## Quick Start
Serve the static file from the repo root using any HTTP server.

```bash
python3 -m http.server 8000
```

Open `http://localhost:8000` in your browser.

## Model & Gradient
- Model: `y = a x`
- Loss: `MSE = (1/n) Σ (a x_i − y_i)^2`
- Gradient: `∂/∂a = (2/n) Σ x_i (a x_i − y_i)`

Enjoy experimenting!