# Is RWE on track for its 2030 coal exit?

Group project for **Climate Risks (IDSI 51003)**. Role: **sustainability consultant**.
Team: Victor Henz, Edgar Gusching, Marius Rang, Ylias Guetari.

## Question

Does RWE's wind + solar pipeline cover the coal capacity it has committed to close by 2030
(capacity-factor-adjusted **replacement ratio ≥ 1**), and does its past build rate make that pipeline credible?

## Repo structure

```
data/   GEM Global Integrated Power Tracker, September 2026 V2 (xlsx)
labs/   lab notebooks (lab5.ipynb) + figures for the paper (fig_uncertainty.png)
```

## How to run

```bash
pip install -r requirements.txt
jupyter notebook labs/lab5.ipynb      # then Kernel -> Restart & Run All (~1-2 min, the xlsx is big)
```

The notebook looks for the GEM file in `data/` (or next to the notebook), with spaces or underscores in the name.

## Main results so far (Lab 5)

* RWE wind + solar capacity in 2030 (equity share): median **23.9 GW**, 90% interval 19.3-28.5 GW (current pipeline).
* Replacement ratio vs the coal RWE committed to close: **1.10** (0.63-1.63), P(ratio ≥ 1) = 0.63.
* To reach a ratio of 1 RWE has to build **~2.05 GW/yr** in 2026-2030, vs 0.78-1.01 GW/yr in the past: 2 to 2.6x faster.

## Data and license

Global Energy Monitor, *Global Integrated Power Tracker*, September 2026 V2, licensed **CC BY 4.0**
(https://globalenergymonitor.org/projects/global-integrated-power-tracker/).
Known limits: parent company recorded for only 28% of RWE units, and GEM captures about 64% of the
wind + solar capacity RWE reports for end 2024 (see Part A of `labs/lab5.ipynb`).
