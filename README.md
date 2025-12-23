
# Golden Gradient

Golden Gradient is a **heuristic optimizer** that replaces adaptive magnitude scaling with **directional gating**.

## What it does
It preserves the raw gradient and simply refuses to move when the direction is inconsistent with recent history.

## Why it matters
Adam and RMSProp fail on oscillatory / rotating-curvature landscapes due to variance amplification.
Golden Gradient accumulates monotonic gains instead.

## Status
- Deterministic
- One extra dot product
- Explicitly heuristic (no convergence claims)

## Demo
https://amiddlebrook.github.io/GoldenGradient/
