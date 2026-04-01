# Supply and Demand Research

Structured research runs investigating supply and demand zone detection, validation, and trading strategies.

## Repo Structure

```
├── runs/                    # Each research run gets its own folder
│   ├── .template/           # Copy this to start a new run
│   │   ├── data/            # Raw and processed data for this run
│   │   ├── notebooks/       # Jupyter notebooks (analysis, exploration)
│   │   ├── results/         # Output files, metrics, logs
│   │   ├── figures/         # Charts, plots, visualizations
│   │   └── README.md        # Run description, hypothesis, conclusions
│   ├── 001-zone-detection/  # Example: first research run
│   ├── 002-zone-scoring/    # Example: second research run
│   └── ...
├── shared/                  # Reusable code across runs
│   ├── indicators/          # Zone detection, scoring functions
│   ├── utils/               # Data loading, plotting helpers
│   └── configs/             # Shared configuration files
├── docs/                    # Background reading, methodology notes
└── README.md
```

## Starting a New Run

```bash
cp -r runs/.template runs/NNN-short-name
```

Edit the run's `README.md` to document:
- **Hypothesis** — What you're testing
- **Data** — Instruments, timeframes, date ranges
- **Method** — Approach and parameters
- **Results** — Key findings
- **Conclusions** — What this means for the next run

## Run Naming Convention

`NNN-short-description` where NNN is a zero-padded sequence number.

| Run | Description |
|-----|-------------|
| 001 | *(first run)* |

## Principles

- Each run is self-contained and reproducible
- Document hypothesis before running experiments
- Record negative results — knowing what doesn't work is valuable
- Shared code lives in `shared/`, not duplicated across runs
