# NFL Player Frame Data Visualization

**Tools:** Python, Pandas, Matplotlib  
**Skills:** Tracking data visualization, movement analysis

---

## Overview

Visualizes player movement patterns across NFL plays using frame-level tracking data. The goal is to surface spatial context, speed changes, and positioning that inform more advanced performance metric development — specifically as a precursor to the NFL Big Data Bowl in-stride analysis.

Each frame captures 22 players' (x, y) coordinates, speed, acceleration, direction, and orientation throughout a play, enabling granular animation and static snapshot visualizations.

---

## Key Findings

- Frame-level data reveals clear positional clustering by role (coverage defenders, receivers, backfield players) that is invisible in aggregate statistics
- Speed and acceleration profiles differ sharply between pre-snap motion and post-snap routes, which can serve as features for downstream modeling
- Visualization confirms that spatial context — not just distance — drives route difficulty and coverage assignments

---

## File Structure

```
nfl-player-frame-viz/
├── data/
│   └── frame_test_input.csv             # NFL frame-level tracking sample
├── visualizing_nfl_player_frame_data.ipynb  # Visualization notebook
└── README.md
```

---

## How to Run

This notebook is designed to run in **Google Colab**. To use the local data file:

1. Open `visualizing_nfl_player_frame_data.ipynb` in Colab or Jupyter
2. Replace the Google Drive path with: `data/frame_test_input.csv`
3. Run all cells

The sample dataset (`frame_test_input.csv`) contains tracking data for select plays and is sufficient to reproduce all visualizations in the notebook.
