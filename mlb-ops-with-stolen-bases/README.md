# MLB: Extending OPS with Stolen Base Value

**Tools:** Python, Pandas, Google Colab  
**Skills:** Metric design, exploratory analysis, baseball analytics

---

## Overview

On-base Plus Slugging (OPS) is one of the most widely used batting efficiency metrics in baseball, but it ignores baserunning entirely. This project introduces a modified metric — OPS+SB — that incorporates stolen base value using a run expectancy framework, then measures how player rankings shift as a result.

The analysis uses 2024 MLB season data and treats stolen bases as a positive and caught stealing as a negative.

---

## Key Findings

- A meaningful subset of players see significant ranking changes when baserunning is incorporated, particularly speedsters who profile as below-average sluggers
- OPS systematically undervalues players whose game is built around on-base ability and stolen bases
- The metric delta (OPS+SB − OPS) surfaces a clear tier of baserunning specialists whose value is obscured by traditional slash-line metrics

---

## File Structure

```
mlb-ops-with-stolen-bases/
├── data/
│   └── adding_stolen_bases_to_ops.csv   # 2024 MLB season statistics
├── adding_stolen_bases_to_ops.ipynb     # Full analysis notebook
└── README.md
```

---

## How to Run

This notebook is designed to run in **Google Colab**. To use the local data file instead of Google Drive:

1. Open `adding_stolen_bases_to_ops.ipynb` in Colab or Jupyter
2. Replace the Google Drive path with: `data/adding_stolen_bases_to_ops.csv`
3. Run all cells
