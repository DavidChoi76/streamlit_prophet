<div align="center">

![Streamlit Prophet](streamlit_prophet/references/logo.png)

Deploy a [Streamlit](https://streamlit.io/) app to train, evaluate and optimize a [Prophet](https://facebook.github.io/prophet/) forecasting model visually

## ⭐  Quick Start  ⭐

[Test the app online](https://davidchoi76-streamlit-prop-streamlit-prophetappdashboard-no33b5.streamlit.app/) with shared computing resources 


</div>


## 💻 Requirements

### Python version
* Main supported version : <strong>3.7</strong> <br>
* Other supported versions : <strong>3.8</strong> & <strong>3.9</strong>

Please make sure you have one of these versions installed to be able to run the app on your machine.

### Operating System
Windows users have to install [WSL2](https://docs.microsoft.com/en-us/windows/wsl/) to download the package. 
This is due to an incompatibility between Windows and Prophet's main dependency (pystan). 
Other operating systems should work fine.

## ⚙️ Installation


### Create a virtual environment (optional)
We strongly advise to create and activate a new virtual environment, to avoid any dependency issue.

For example with conda:
```bash
pip install conda; conda create -n streamlit_prophet python=3.7; conda activate streamlit_prophet
```

Or with virtualenv:
```bash
pip install virtualenv; python3.7 -m virtualenv streamlit_prophet --python=python3.7; source streamlit_prophet/bin/activate
```


### Install package
Install the package from PyPi (it should take a few minutes):
```bash
pip install -U streamlit_prophet
```

Or from the main branch of this repository:
```bash
pip install git+https://github.com/artefactory-global/streamlit_prophet.git@main
```


## 📈 Usage

Once installed, run the following command from CLI to open the app in your default web browser:

```bash
streamlit_prophet deploy dashboard
```

Now you can train, evaluate and optimize forecasting models in a few clicks.
All you have to do is to upload a time series dataset. 
This dataset should be a csv file that contains a date column, a target column and optionally some features, like on the example below:

![](streamlit_prophet/references/input_format.png)

Then, follow the guidelines in the sidebar to:

* <strong>Prepare data</strong>: Filter, aggregate, resample and/or clean your dataset.
* <strong>Choose model parameters</strong>: Default parameters are available but you can tune them.
Look at the tooltips to understand how each parameter is impacting forecasts.
* <strong>Select evaluation method</strong>: Define the evaluation process, the metrics and the granularity to
assess your model performance.
* <strong>Make a forecast</strong>: Make a forecast on future dates that are not included in your dataset,
with the model previously trained.

Once you are satisfied, click on "save experiment" to download all plots and data locally.