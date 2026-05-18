# drive_wam

World Action Models for autonomous driving.

## Overview

`drive_wam` explores world action models — models that jointly learn world dynamics and driving policy — for autonomous driving. The goal is to predict future scene state conditioned on candidate actions and use this for planning.

## Structure

```
drive_wam/
├── README.md
├── TODO.md
└── third_party/
    └── drivelaw/        # reference: DriveLaW (action + video baselines)
```

## Getting started

TBD — environment setup, data preparation, and training scripts will be added as the project takes shape.

## References

- `third_party/drivelaw` — DriveLaW reference implementation (action and video variants).
