# Convection–Diffusion IBVP

This repository contains a complete computational study and final report for the one-dimensional convection–diffusion initial-boundary-value problem (IBVP), comparing finite-difference (FDM) and finite-element (FEM) discretizations. Everything you need—code, figures, and write-up—is organized under a single folder.

## Repository Layout

```
Convection-Diffusion IBVP/
├── notebooks/                ← Jupyter notebook with all code + explanatory Markdown
│   └── convection_diffusion_analysis.ipynb
└── report/                   ← Final written report
    ├── convection_diffusion_report.pdf
    └── convection_diffusion_report.md
```

### notebooks/
- **convection_diffusion_analysis.ipynb**  
  Contains all Python code cells (FDM/FEM assembly, solvers, convergence tests, plots) interleaved with Markdown cells explaining theory, algorithms, and interpretation. Run sequentially to reproduce every figure and table.

### report/
- **convection_diffusion_report.pdf**  
  Polished, paginated project write-up including introduction, derivations, results, and conclusions.
- **convection_diffusion_report.md**  
  Markdown source of the above PDF for easy editing.

## Getting Started

### Prerequisites
- Git (to clone this repo)
- Python 3.7+
- Conda (recommended) or pip
- Jupyter Notebook or JupyterLab

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/Convection-Diffusion-IBVP.git
   cd Convection-Diffusion-IBVP
   ```

2. **Create and activate the environment**
   - Using Conda (preferred):
     ```bash
     conda create -n ibvp_env python=3.8 numpy scipy matplotlib pandas jupyter
     conda activate ibvp_env
     ```
   - Using pip + venv:
     ```bash
     python3 -m venv ibvp_env
     source ibvp_env/bin/activate       # macOS/Linux
     ibvp_env\Scripts\activate.bat    # Windows
     pip install numpy scipy matplotlib pandas jupyter
     ```

3. **Launch Jupyter**
   ```bash
   jupyter lab    # or jupyter notebook
   ```
   Navigate to the `notebooks/` folder and open `convection_diffusion_analysis.ipynb`.

## Usage

1. Open and run `notebooks/convection_diffusion_analysis.ipynb`:
   - Section 1: Problem statement and IBVP formulation.
   - Section 2: FDM & FEM derivations.
   - Section 3: Convergence studies.
   - Section 4: Results, plots, and interpretation.

2. View final report in `report/convection_diffusion_report.pdf`.

## Dependencies

- Python 3.7+
- numpy
- scipy
- matplotlib
- pandas
- jupyter

Install dependencies via:
```bash
conda install numpy scipy matplotlib pandas jupyter
```
or
```bash
pip install numpy scipy matplotlib pandas jupyter
```

## Troubleshooting

- **ModuleNotFoundError:** Ensure `ibvp_env` is activated.
- **Kernel issues:** Restart Jupyter after environment activation.
- **Plot overlaps:** Clear outputs and rerun cells.

---

By following this guide, you can reproduce all figures, tables, and analyses, even if you’re new to GitHub or Python. Happy exploring!
