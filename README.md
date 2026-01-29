# HEA4HER
We use an interpretable machine-learning model with composition-based descriptors to rapidly screen and discover thermodynamically stable high-entropy alloys for hydrogen evolution catalysis.
HEA Discovery for HER — Code and Data


Title: Data-Efficient Discovery of Thermodynamically Stable High-Entropy Alloy Catalysts for Hydrogen Evolution Reaction
Author: Ziqi Tang
Track: AI4Mat @ LCLR 2026 (Tiny Papers)

The goal is to screen equimolar five-element HEA compositions for HER catalysis using
thermodynamic stability rules and lightweight machine learning models based only on composition-derived descriptors.

Folder Structure
data/        # datasets (raw and processed)
scripts/     # python scripts for descriptors, screening, ML
notebooks/   # analysis and figure generation
results/     # output tables and plots

Data

Includes:

Experimental HER performance data collected from literature

Elemental physical and chemical properties

Generated equimolar 5-element HEA composition space

Main targets:

Overpotential at 10 mA cm⁻² (mV)

Optional: Tafel slope

Descriptors

For each HEA composition, descriptors are calculated from elemental properties:

Mixing enthalpy (ΔHmix)

Configurational entropy (ΔSmix)

Atomic size mismatch (δ)

Ω stability parameter

Mean electronegativity

Mean ionization energy

Estimated hydrogen binding energy

Only composition-based features are used (no structural input).

Models

Supervised regression models:

Random Forest Regressor (main model)

Linear regression (baseline)

Used to rank thermodynamically stable HEA candidates for HER activity.


Notes

Predictions are intended for trend-based screening, not exact activity values.

Stability screening is based on empirical solid-solution criteria, not CALPHAD or DFT.



Contact

Ziqi Tang
PhD Candidate, Mechanical Engineering
University of Ottawa
