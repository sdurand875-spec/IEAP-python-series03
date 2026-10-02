# IEAP – Python Series 03: Remarkable points in a signal

Group assignment for the IEAP Python course: find and plot the **remarkable points** of a signal (zero crossings, local maxima and minima), use them to compute the **frequency** of a known signal, then redo the analysis on a **noisy signal** with a low-pass filter.

## Group

| Member | Part | Notebook |
|---|---|---|
| Sarah DURAND | Part 2 – Functions to find and plot remarkable points | [`Section/part2_functions.ipynb`](Section/part2_functions.ipynb) |
| Zoé SAUGE | Part 3 – Analysis of a known signal | [`Section/part3_clean_signal.ipynb`](Section/part3_clean_signal.ipynb) |
| Shunan YIN | Part 4 – Analysis of a noisy signal | [`Section/part4_noisy_signal.ipynb`](Section/part4_noisy_signal.ipynb) |

## Repository structure

```
IEAP-python-series03/
├── README.md                     ← this file
├── IEAP-python-series03.ipynb    ← main notebook gathering the three parts
└── Section/
    ├── part2_functions.ipynb     ← zero crossings, local extrema, plots, unit tests
    ├── part3_clean_signal.ipynb  ← known signal (two sine waves) + frequency computation
    └── part4_noisy_signal.ipynb  ← white noise + Butterworth low-pass filter
```

Parts 3 and 4 reuse the functions of part 2 with:

```python
%run part2_functions.ipynb
```

## Git workflow

- Each member works on **their own branch** and **their own notebook**, so no file is edited by two people and there are no merge conflicts.
- Branches: `part2-functions`, `part3-clean-signal`, `part4-noisy-signal`.
- When a part is finished, its author opens a **pull request** to `main`. Another member reviews it before it is merged.
- Function names and outputs were agreed on **before starting**, so that parts 3 and 4 could be written in parallel with part 2.
- The `main` branch always contains the latest validated version of the work.

## How to run

1. Clone the repository.
2. Install the required libraries: `numpy`, `matplotlib`, `scipy`.
3. Open the folder in VS Code (or Jupyter) and run `IEAP-python-series03.ipynb`, or run each notebook of `Section/` separately.
