## Overview

**PhStats** is a collection of Jupyter notebooks containing homework assignments (HW) and seminar exercises (SEM) for your statistics coursework. Each notebook covers a specific problem set or topic module, with solutions, visualizations, and commentary.

---

## Repository Structure

```
PhStats/
├── HW/              # Homework notebooks
│   ├── HW_1.ipynb
│   ├── HW_2.ipynb
│   ├── …
│   └── HW_12.ipynb
├── SEM/             # Seminar (lecture/practice) notebooks
│   ├── SEM_1.ipynb
│   ├── SEM_2.ipynb
│   ├── …
│   └── SEM_12_2.ipynb
├── .gitignore       # Specifies files and folders to ignore in Git
└── .gitattributes   # Normalizes line endings and notebook filtering
```

* **HW/**
  Contains 12 weekly homework notebooks (HW\_1 through HW\_12), each covering exercises aligned with the course’s syllabus.
* **SEM/**
  Contains seminar notebooks divided into two parts for certain weeks (e.g., SEM\_3\_1 and SEM\_3\_2), totaling 22 files that accompany lecture topics and in‑class activities.

---

## Prerequisites

1. **Python 3.8+**
2. **Jupyter Notebook or JupyterLab**
3. Key Python libraries typically used for statistical analyses, for example:

   * `numpy`
   * `pandas`
   * `matplotlib`
   * `scipy`
   * `statsmodels`

You can install them all via:

```bash
pip install numpy pandas matplotlib scipy statsmodels jupyter
```

---

## Getting Started

1. **Clone the repository**

   ```bash
   git clone https://github.com/MakVlad2003/PhStats.git
   cd PhStats
   ```

2. **Open Jupyter**

   ```bash
   jupyter lab   # or `jupyter notebook`
   ```

3. **Navigate** to the **HW/** or **SEM/** folder in the file browser and launch the notebook you want to review.

---

## Usage Tips

* **Clearing vs. Keeping Outputs**
  The repository uses a custom Git filter (`nbsoft`) configured in `.gitattributes` to strip certain metadata while preserving cell outputs. You generally don’t need to reconfigure this—just run and commit as usual.

* **Line Ending Warnings**
  When you see warnings like

  ```
  LF will be replaced by CRLF the next time Git touches it
  ```

  it means your system’s line endings differ from the repository’s. This is handled automatically by the `.gitattributes` settings; no action is required.

* **Version Control for Notebooks**

  * Run `nbstripout --install` in this repo to re-enable automatic cleaning of widget metadata on commit.
  * Use `git add --renormalize .` if you ever need to reapply the filter rules across all notebooks.

---

## Contributing

1. **Add or update assignments** in the appropriate folder (HW or SEM).

2. **Ensure notebook outputs are updated** by running all cells before committing.

3. **Follow existing naming conventions**:

   * Homework: `HW_<week>.ipynb`
   * Seminar: `SEM_<week>[_<part>].ipynb`

4. **Submit a pull request** — include a brief description of your changes.

---

## License

This repository is provided under the MIT License. Feel free to reuse and adapt these notebooks for your own coursework.
