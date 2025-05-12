# PhStats — Probability & Statistics Coursework

<p align="center">
  <img src="https://img.shields.io/badge/Status-In_Progress-blue?style=flat-square" alt="status badge" />
  <img src="https://img.shields.io/badge/Python-3.9+-yellow?style=flat-square" alt="python badge" />
  <img src="https://img.shields.io/github/last-commit/MakVlad2003/PhStats?style=flat-square" alt="last commit badge" />
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square" alt="license badge" />
</p>

> **Goal:** Consolidate lectures, seminars, and homework for the *Probability & Statistics* (PhStats) module at MIPT (spring–summer 2025).

---

## Table of Contents

1. [Overview](#overview)
2. [Repository Layout](#repository-layout)
3. [Running the Notebooks](#running-the-notebooks)
4. [Course Road‑map](#course-road-map)
5. [Contributing](#contributing)
6. [License](#license)

---

## Overview

This repository stores two major content streams:

* **`SEM/` — Seminars** Interactive Jupyter notebooks used during live coding sessions. Each notebook focuses on one topic (e.g. *Bayesian Inference*, *Maximum‑Likelihood Estimation*, *Markov Chains*).
* **`HW/` — Home‑works** Problem‑set notebooks with embedded theory blocks and autograded tasks.

All material is written in Python 3.9 using *NumPy*, *SciPy*, *pandas*, *matplotlib*, and *seaborn*; more advanced topics leverage *statsmodels* and *scikit‑learn*.

---

## Repository Layout

```
PhStats/
├── SEM/
│   ├── 01_intro_prob.ipynb        # Axioms, combinatorics, PMFs/CDFs
│   ├── 02_random_vars.ipynb       # Expectation, variance, law of total prob.
│   ├── 03_limit_theorems.ipynb    # LLN, CLT demos via Monte‑Carlo
│   └── …
├── HW/
│   ├── hw1_basic_prob.ipynb       # Dice & cards simulations
│   ├── hw2_estimation.ipynb       # MLE vs. Method‑of‑Moments
│   ├── hw3_hypothesis_testing.ipynb
│   └── …
├── environment.yml                # Conda spec for full reproducibility
├── requirements.txt               # pip‑friendly export
├── .gitignore                     # ignores checkpoints, data imports, outputs
└── .gitattributes                 # enables rich diff for notebooks
```

> Notebook names follow the same numbering as the course syllabus for quick navigation.

---

## Running the Notebooks

1. **Clone the repo**

   ```bash
   git clone https://github.com/MakVlad2003/PhStats.git && cd PhStats
   ```
2. **Create an environment** (conda recommended):

   ```bash
   conda env create -f environment.yml
   conda activate phstats
   ```
3. **Launch JupyterLab**

   ```bash
   jupyter lab SEM/01_intro_prob.ipynb
   ```

GPU is *not* required; all computations finish on a typical laptop within seconds.

---

## Course Road‑map

| Week | Topic                                     | Key notebook                      |
| ---- | ----------------------------------------- | --------------------------------- |
| 1    | Probability axioms & combinatorics        | `SEM/01_intro_prob.ipynb`         |
| 2    | Discrete & continuous distributions       | `SEM/02_random_vars.ipynb`        |
| 3    | Laws of large numbers, CLT                | `SEM/03_limit_theorems.ipynb`     |
| 4    | Parameter estimation                      | `HW/hw2_estimation.ipynb`         |
| 5    | Confidence intervals & hypothesis testing | `HW/hw3_hypothesis_testing.ipynb` |
| 6    | Linear regression & ANOVA                 | `SEM/linear_models.ipynb`         |
| 7    | Bayesian inference                        | `SEM/bayesian_intro.ipynb`        |
| 8    | Markov chains & Monte‑Carlo               | `SEM/markov_mc.ipynb`             |
| 9    | Final project guidelines                  | `SEM/final_project.ipynb`         |

> 📌 **Checkpoint submissions** are due each Sunday 23:59 UTC‑3.

---

## Contributing

Have a typo fix or an idea for an extra‑credit exercise? Feel free to open a pull request:

1. Fork the repo and create a branch
2. Commit with clear messages (`feat:`, `fix:`, `docs:` prefixes)
3. Open a PR — please follow *PEP 8* and keep cells under 80 chars wide.

See `CONTRIBUTING.md` for full guidelines.

---

## License

This work is distributed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

---

<p align="center">Made with 📊 + 🍀 by <a href="https://github.com/MakVlad2003">Vladislav Makarov</a></p>
