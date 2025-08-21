# GAPDH Enzyme Kinetics Analysis

Biochemical analysis of GAPDH (Glyceraldehyde-3-phosphate dehydrogenase) through equilibrium constant determination and FBP concentration measurement.

## Requirements

- R version 4.5.0+
- Required packages (managed via renv):
  - tidyverse
  - janitor
  - knitr

## Setup

1. Clone/download the project
2. Open R in the project directory
3. Restore the R environment:
   ```r
   renv::restore()
   ```

## Data

- `data/GAPDH_1.csv`: Experiment 1 - Sequential phosphate buffer additions (174 measurements)
- `data/GAPDH_2.csv`: Experiment 2 - TIM enzyme assay (66 measurements)

## Analysis

Run the Jupyter notebook:
```r
# Open auswertung.ipynb in RStudio or Jupyter
```

### Experiment 1: Equilibrium Constant
- Measures extinction changes after phosphate buffer additions
- Calculates K' = 0.0671 ± 0.0260
- Determines ΔG'° = 6.70 kJ/mol

### Experiment 2: FBP Concentration
- NADH-coupled enzyme assay
- Determines [FBP] = 0.85 mM in original sample

## Output

- `figures/erste_kurve.png`: Experiment 1 kinetics plot
- `figures/zweite_kurve.png`: Experiment 2 kinetics plot

## Reproducibility

The `renv.lock` file ensures exact package versions. All calculations use explicit constants and formulas documented in the notebook.

## Licence 
MIT