# Reproducing ARIMA Model Research

The scientific paper which results we chose to reproduce was _"Air Passengers Occupancy Prediction Using Arima Model"_ by Konda Himakireeti and Tammishetti Vishnu (2019). 

## Scientific Paper

The paper presents the process of tuning ARIMA model to predict air passengers occupancy over time. Code used to implement this statistical model was not attached to the paper, so we chose to re-implement relevant parts of the procedure described in detail in the scientific article.

## Our Workflow

Most important development tools used in the process are listed below:

* We used [Python](https://www.python.org/) as our language of choice.
* Analysis was performed in a [Jupyter Notebook](https://jupyter.org/). 

## Reproducibility

We set up a custom GitHub action that runs on every pull request to the `main` branch. It runs the sequence of operations described in section `Running the Code` of this `README`. Using this action we were sure, that no dependencies may be missing from the `requirements` set, and that the notebook produces a valid `html` file correctly and without errors on the latest Ubuntu linux release. 

[![notebook](https://github.com/Staneesh/Repro2023/actions/workflows/notebook.yml/badge.svg?branch=main)](https://github.com/Staneesh/Repro2023/actions/workflows/notebook.yml)

## Collaboration

In our work we relied heavily on Git:

* We used the [Issues](https://github.com/Staneesh/Repro2023/issues?q=is%3Aissue) tab to decide on a project topic and its scope.
* We used the `main` branch as the project master.
* The `main` branch was protected from direct pushes - approval from all team members was required for every pull request, which forced all team members to communicate and comment. Please see our list of [Pull Requests here](https://github.com/Staneesh/Repro2023/pulls?q=is%3Apr+).

## Features / Milestones

The main list of tasks that we wanted to accomplish is outlined below. Two main questions that we wanted to answer are marked in **bold**.

- [X] Loading the data
- [X] Importing Python packages relevant for data analysis
- [X] Fitting the model using ARIMA
- [X] Forecasting 
- [X] Plotting forecast results
- [X] Documenting code
- [X] **Were the results replicated?**
- [X] Alternative model implementation + comparisons
- [X] **Were we able to improve the model from the paper?**

## Running the Code

Please make sure you have all usual dependencies installed on your system. Most importantly `python`, `pip` and `ipykernel`. If you're using _Visual Studio Code_ for development, you should be prompted to install them automatically. Next, follow this process:

1. Create the virtual environment: `python -m venv venv`
2. Enter `venv`: `source venv/bin/activate` on Linux or `venv\Scripts\activate.bat` on Windows
3. Upgrade you `pip`: `pip install --upgrade pip`
4. Install dependencies from the requirements file: `pip install -r requirements.txt`
5. You're good to open the Jupyter Notebook IDE of your choice. Be sure to use select Python version from inside the `venv` you just created when prompted by `ipykernel` package.

## Quarto Report

Whilst viewing `main.ipynb` is an acceptable way of viewing the reproduced output, note that an enhanced and visually appealing report has been created using Quarto and is saved as `main.html`. The initial raw block embedded in `main.ipynb` contains the YAML details for report processing.

A separate `main_quarto.qmd` file replicating `main.ipynb` report processing has been saved for reference and `main_quarto.html` has been rendered on the back of this. There is no practical difference between the html reports.

Running the Quarto reports requires _Quarto CLI_ installed. Running `quarto render main.ipynb` in terminal generates the report. Copying `main.ipynb` to `main_quarto.ipynb` and then running `quarto convert main_quarto.ipynb` and `quarter render main_quarto.qmd` generates the qmd-based report for reference.
