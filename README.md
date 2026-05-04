# Thesis Code: SIA and DDM Analysis

This repository contains Python code for Spatial Image autocorelation (SIA) and Differential Dynamic Microscopy (DDM) used in my thesis.

---

## Requirements

Before running the DDM scripts, install the PyDDM package:

👉 [https://github.com/rmcgorty/PyDDM/tree/main/docs](https://github.com/rmcgorty/PyDDM/tree/main/docs)

No additional dependencies are required beyond those bundled with PyDDM.

---

## SIA (Static Image Analysis)

**Script:** `SIA`

Run directly on a folder of `.tiff` files.

**Output:**
- A table of **g(r) vs r** (radial distribution function)

---

## DDM (Differential Dynamic Microscopy)

All DDM scripts use the **single exponential decay model**.

Run these scripts **after installing the PyDDM package** (see Requirements above).

### 1. `originalDDM-single-exponential` — Run on folder → individual tauvsq file

**Output:**
- **τ vs q** plot only

---

### 2. `DDM-alpha` / `alpharescaled` / `tauqsquared`

**Output:**
- **α** (alpha) values
- **α rescaled** (alpha squared) values
- **τ vs α²** (tau vs alpha squared) plot

---

### 3. `DDM-single-exponential` — Run on folder → individual tauvsq-ISF file

**Output:**
- **τ vs q** plot
- **τ vs ISF** plot

---

## Usage

1. Point the script at a folder containing your `.tiff` image files
2. Run the desired script
3. Output files will be saved in the same folder

---

## Contact

For questions about this code, please contact the author via this repository.
