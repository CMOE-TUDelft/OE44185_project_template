# OE44185 Project Report Template

LaTeX template for **OE44185: Numerical Methods for Offshore and Dredging Engineering**.

The template is tailored to the course project on modelling a floating offshore wind turbine (OC3 Phase-IV spar-buoy) and focuses on the numerical modelling workflow.

## Deliverables Covered by This Template

- Report (maximum **15 pages** excluding appendices)
- Executable script or notebook for reproducibility

## Repository Structure

- `main.tex`: main report entry point
- `style.tex`: formatting and reusable placeholder commands
- `chapters/01_model_definition.tex`
- `chapters/02_numerical_methods.tex`
- `chapters/03_numerical_schemes.tex`
- `chapters/04_results_analysis.tex`

## Build

```bash
latexmk -pdf main.tex
```

Clean auxiliary files:

```bash
latexmk -c
```

## Report Logic

1. Model Definition
2. Numerical Discretization
3. Numerical Schemes and Implementation
4. Numerical Verification and Results Interpretation

## Core + Choice Architecture

- Core Model (mandatory): 2D FOWT representation, baseline loading, FEM/FVM discretization, and dynamic response assessment.
- Choice Packages (pick at least two): nonlinear mooring, irregular waves, time-dependent thrust/current, circular-cylinder CFD extension, local mesh refinement, or reduced-order/modal extension.

## Section Boundary Rules

- Section 1: assumptions, scope limits, and continuous model definition.
- Section 2: discrete formulation and discretization choices only.
- Section 3: implementation and algorithmic design choices.
- Section 4: verification first (convergence/stability/modal), then interpreted engineering results.

## Suggested Milestones

1. Week 1-2: One-page scope proposal (Core + selected Choice Packages).
2. Week 3: Model definition freeze (assumptions and equations).
3. Week 4-5: Discretization and implementation checkpoint.
4. Week 6: Verification checkpoint (convergence and stability evidence).
5. Final week: Results interpretation and report consolidation.

## Notes

- Replace all instructional placeholders before submission.
- Keep derivation details and long code excerpts in appendices.
- Provide explicit validation, convergence checks, and literature comparison.
- If AI is used, complete the in-depth acknowledgement in main.tex.
