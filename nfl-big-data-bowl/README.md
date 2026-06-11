# NFL Big Data Bowl: In-Stride Passing & Receiver Disruption

**Tools:** R, tidyverse, Kaggle  
**Skills:** Feature engineering, spatiotemporal analysis, custom metrics

---

## Overview

Developed as part of the **NFL Big Data Bowl** competition. This project creates a custom "in-stride" metric that quantifies how quarterback ball placement affects receiver acceleration and route disruption around the catch point.

Using frame-level player tracking data, the analysis connects receiver speed-up and slow-down to passing efficiency and play outcomes and attempts to surface a dimension of QB accuracy that traditional completion percentage ignores.

---

## Key Findings

- Receivers forced to adjust their routes (decelerate, redirect) to catch the ball show measurably worse yards-after-catch outcomes
- Ball placement relative to a receiver's projected path is a stronger predictor of route disruption than pass distance alone
- The in-stride metric differentiates elite QBs from average QBs in situations where completion percentage alone does not

---

## File Structure

```
nfl-big-data-bowl/
├── hit-em-in-stride.ipynb   # Full analysis notebook (R kernel)
└── README.md
```

> Tracking data is sourced from the Kaggle NFL Big Data Bowl competition and is not included in this repository.

---

## How to Run

1. Download the NFL Big Data Bowl tracking data from [Kaggle](https://www.kaggle.com/competitions/nfl-big-data-bowl-2025/data)
2. Open `hit-em-in-stride.ipynb` in Jupyter with an R kernel, or in Google Colab with R runtime
3. Update the data path at the top of the notebook and run all cells
