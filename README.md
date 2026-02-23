# Homework 3: Time Series and Extreme Values

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

This is the repository for Homework 3 for [BEE 4850](https://viveks.me/simulation-data-analysis), taught at [Cornell University](https://cornell.edu) in Spring 2026 by [Vivek Srikrishnan](https://viveks.me).

If enrolled in the class, a PDF of the completed assignment, **with all cells evaluated if a notebook**, should be submitted to Gradescope *no later* than Friday, March 06, 2026, at 9:00pm. The assignment will be penalized 50% if it is submitted up to 24 hours late.

## Learning Objectives

After completing this lab, students will be able to:

* Diagnose autocorrelation in a time series and develop an AR(1) model.
* Use predictive distributions of test statistics to assess how well a model works.
* Calibrate a semi-empirical model using assumptions of both Gaussian i.i.d. and AR(1) residuals.
* Model block maxima and peaks over thresholds using extreme value theory.
* Calculate and compare return levels of extreme events.

## Repository Overview

The repository consists of the following files:

- `hw03.ipynb`: Jupyter Notebook for the homework assignment. Students should create code or Markdown blocks as necessary to answer questions. **This is the only file you should need to edit.**
- `Project.toml`, `Manifest.toml`: Julia environment files. These should just work, but feel free to add other packages as needed using the `Pkg` package manager. **This is the only other file that you might end up making changes to, though you should do this using `Pkg`, not directly.**
- `hw03.qmd`: Source file for Jupyter notebook generation. You shouldn't need to or want to touch this; everything is in the `.ipynb` file.
- `LICENSE`: This material is licensed using the MIT license. You can ignore this for working on the problem set.
- `README.md`: This file. You shouldn't need to touch this.
- `.gitignore`: This tells `git` what files to ignore. You shouldn't need to touch this.
- `.github/`: This folder contains workflow files which generate the notebook. Again, you shouldn't need to touch this.
- `data/`: This folder contains several .csvs and other data files to complete the projects.

## Prerequisites

### Julia

[Julia](https://julialang.org/downloads/): This notebook was developed with version 1.11.5, but any 1.11.x should work (there could be some issues with other versions, depending on what's changed). You can solve this assignment using other languages, but the provided notebook is based on Julia.

### Packages

These are provided in the project environment assuming the assignment will be solved in Julia; similar packages from other languages can be used instead.

1. `DataFrames.jl`: tabular data structure
2. `DataFramesMeta.jl`: macros to simplify DataFrames.jl commands
2. `CSV.jl`: reads/writes .csv files
3. `Distributions.jl`: interface to work with probability distributions
4. `Plots.jl`: plotting library
5. `StatsBase.jl`: statistical quantities like mean, median, etc
6. `StatsPlots.jl`: some additional statistical plotting tools
7. `Optim.jl`: optimization tools
8. `LaTeXStrings.jl`: latex formatting for plot strings
9. `Dates.jl`: API for time-date units.