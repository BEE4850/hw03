# Homework 3: Bayesian Statistics and Monte Carlo Simulation

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

This is the repository for Homework 3 for [BEE 4850](https://viveks.me/simulation-data-analysis), taught at [Cornell University](https://cornell.edu) in Spring 2025 by [Vivek Srikrishnan](https://viveks.me).

If enrolled in the class, a PDF of the completed assignment, **with all cells evaluated if a notebook**, should be submitted to Gradescope *no later* than Friday, March 14, 2025, at 9:00pm. The assignment will be penalized 50% if it is submitted up to 24 hours late.

## Learning Objectives

After completing this lab, students will be able to:

* Approximate posterior distributions using grid approximations;
* Sample from (low-dimensional) distributions using rejection sampling;
* Use Monte Carlo simulation to compute expected values of non-linear functions;
* Solve optimization problems using Monte Carlo approximations of the objective functions.

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

1. [Install Julia](https://julialang.org/downloads/) before beginning this lab. This notebook was developed with version 1.11.2, but any 1.11.x should work (there could be some issues with other versions, depending on what's changed).
2. If necessary, [install git](https://happygitwithr.com/install-git.html) and [create a GitHub account](https://github.com). 
3. [Clone the repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository). I recommend doing this in a dedicated `BEE4850/` folder, which can also house homework assignment repositories and lecture notes. You can clone directly into the `BEE4850/` folder.   For Windows (or from another graphical interface), just create a `BEE4850` folder, then a `hw` folder inside of that, then clone into that folder. Or to clone into a `BEE4850/hw` folder, from a command prompt:
    ```bash
    cd BEE4850/
    mkdir hw
    cd hw/
    git clone https://github.com/BEE4850/hw03.git
    ```

 