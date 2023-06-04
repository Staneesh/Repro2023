# Reproducing ARIMA Model Research

The scientific paper which results we chose to reproduce was _"Air Passengers Occupancy Prediction Using Arima Model"_ by Konda Himakireeti and Tammishetti Vishnu (2019). 

## Scientific Paper

The paper presents the process of tuning ARIMA model to predict air passengers occupancy over time. Code used to implement this statistical model was not attached to the paper, so we chose to re-implement relevant parts of the procedure described in detail in the scientific article.

## Our Workflow

Most important development tools used in the process are listed below:

* We used [Python](https://www.python.org/) as our language of choice.
* Analysis was performed in a [Jupyter Notebook](https://jupyter.org/). 

## Collaboration

In our work we relied heavily on Git:

* We used the [Issues](https://github.com/Staneesh/Repro2023/issues?q=is%3Aissue) tab to decide on a project topic and its scope.
* We used the `main` branch as the project master.
* The `main` branch was protected from direct pushes - approval from all team members was required for every pull request, which forced all team members to communicate and comment.  

## Features / Milestones

- [ ] Loading the data
- [ ] Importing Python packages relevant for data analysis
- [ ] Fitting the model using ARIMA
- [ ] Forecasting 
- [ ] Plotting forecast results
- [ ] Documenting code
- [ ] **Were the results replicated?**

## Running the Code

Please make sure you have all usual dependencies installed on your system. Most importantly `python`, `pip` and `ipykernel`. If you're using _Visual Studio Code_ for development, you should be prompted to install them automatically. Next, follow this process:

1. Create the virtual environment: `python -m venv venv`
2. Enter `venv`: `source venv/bin/activate` on Linux or `venv\Scripts\activate.bat` on Windows
3. Upgrade you `pip`: `pip install --upgrade pip`
4. Install dependencies from the requirements file: `pip install -r requirements.txt`
5. You're good to open the Jupyter Notebook IDE of your choice. Be sure to use select Python version from inside the `venv` you just created when prompted by `ipykernel` package.