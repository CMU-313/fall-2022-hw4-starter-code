# HW4 Starter Code and Instructions

Please consult the [homework assignment](https://cmu-313.github.io//assignments/hw4) for additional context and instructions for this code.

## pipenv

[pipenv](https://pipenv.pypa.io/en/latest/) is a packaging tool for Python that solves some common problems associated with the typical workflow using pip, virtualenv, and the good old requirements.txt.

### Installation

#### Prereqs

- We recommend Python version > 3.7 be installed
- pip package manager is updated to latest version

#### Mac OS

Run
`sudo -H pip install -U pipenv`
In the command line

#### Windows OS

Adhere to [this](https://www.pythontutorial.net/python-basics/install-pipenv-windows/)

### Usage

#### Downloading Packages

The repository contains `Pipfile` that declares which packages are necessary to run the `model_build.ipnyb`. To install packages declared by the Pipfile, run `pipenv install` in the command line from the root directory.

You might want to use additional packages throughout the assignment.
To do so, run `pipenv install [PACKAGE_NAME]`, as you would install python packages using pip.
This should also update `Pipfile` and add the downloaded package under `[packages]`.

#### Virtual Environment

Working in teams can be a hassle since different team members might be using different versions of Python. To avoid this issue, you can create a python virtual environment, so you and your team will be working with the same version of Python and PyPi packages.
Run `pipenv shell` in your command line to activate this project's virtual environment.
To learn more about virtual environments, read [this article](https://docs.python-guide.org/dev/virtualenvs/#using-installed-packages).
You can also specify which version of python you and your team should use under `[requires]` in `Pipfile`.

## Jupyter Notebook

You should run your notebook in the virtual environment from pipenv.
To do so, in the pipenv virtual environment, run `jupyter notebook`.

## API Endpoints

To start your Flask API server, run `python apps/app.py`.
You can alter the port number in `app.run(host="0.0.0.0", debug=True, port=80)`.
