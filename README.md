# Modern-Time-Series-Forecasting-with-Python-2E

## What is this book about?

This book covers the following exciting features:

* Find out how to manipulate and visualize time series data like a pro
* Set strong baselines with popular models such as ARIMA
* Discover how time series forecasting can be cast as regression
* Engineer features for machine learning models for forecasting
* Explore the exciting world of ensembling and stacking models
* Get to grips with the global forecasting paradigm
* Understand and apply state-of-the-art DL models such as N-BEATS and Autoformer
* Explore multi-step forecasting and cross-validation strategies

This repo is forked from [Modern Time Series Forecasting with Python](https://www.packtpub.com/en-us/product/modern-time-series-forecasting-with-python-9781835883181), published by Packt.

Clone this forked repo use link above.

## Download the Data

You are going to be using a single dataset throughout the book. The book uses London Smart Meters Dataset from Kaggle for this purpose (which is an energy dataset). Many of the notebooks from early chapters are dependencies for some of the later chapters.  As such, to remove this dependency if you want to run the notebooks out of order, we have included a data.zip file with all of the required datasets.
To setup, follow these steps:

1. Download the data from AWS: <https://packt-modern-time-series-py.s3.eu-west-1.amazonaws.com/data.zip>
2. Unzip the content
3. Copy over the data folder to the Modern-Time-Series-Forecasting-with-Python-2E folder you pull from github.

## Use the right version of Python

I use pyenv - you can install this

```bash
brew update
brew install pyenv
brew install cmake
```

Then add pyenv to shell

```bash
echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.zshrc && echo 'command -v pyenv >/dev/null || export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.zshrc && echo 'eval "$(pyenv init -)"' >> ~/.zshrc
```

Restart shell

```bash
source ~/.zshrc
```

Check if pyenv works

```bash
pyenv --version
```

Install the specific version for this repo

```bash
pyenv install 3.10.13
pyenv local 3.10.13
```

Check the Python version

```bash
python --version
```

## Setup the environment

Clone the repo and then download the data

## Using Pip based environment

Create the virtual environment and activate it if Python version above 3.10

```bash
python -m venv venv
source venv/bin/activate
pip install --upgrade pip setuptools
pip install -r requirements_new.txt
```

Then test the installation

```bash
python test_installation.py
```

## Blocks vs RAM

Number of blocks to select from the dataset is dependent on how much RAM you have in your machine. Although, these are not rules, but rough guidelines on how much blocks to choose based on your RAM is given below. If you still face problems, please experiment with lowering the number of blocks to make it work better for you.

* 1 or <1 Block for 4GB RAM
* 1 or 2 Blocks for 8GB RAM
* 3 Blocks for 16GB RAM
* 5 Blocks for 32GB RAM
