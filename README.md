# L1 INFO - Introduction à la Sécurité (des données) - Projet 2024/2025

## Install
This project runs on a Jupyter server compatible with Python 3.8.
If you run the project on [colab](https://colab.research.google.com/),
the following installation is optional (unless you would like to run on
*colab* using local resources).

In order to run the notebooks without *colab*, first, you might create a
virtual environment (optional). Second, install the dependencies,
to do so install [poetry](https://python-poetry.org) a packaging and
dependency management tool. Third, clone the project sources. Finally,
run the *poetry* `install` command to setup the required dependencies.
The complete installation sequence is as follows (set the `PATH`
accordingly):

```bash
# create a virtual environment  
python3.8 -m venv ${PATH}/venv-a2r2
# activate the environment
source ${PATH}/venv-a2r2/bin/activate 
# install the dependency management tool
pip install poetry
# clone the project and enter to the repo dir
git clone https://github.com/tristan-allard/l1-ise-public.git iseperturb && cd $_
# install dependencies on the environment
poetry install
```

## Run
The project is organized in self-contained Jupyter notebooks. These are
located in the `notebooks` directory of the project. There are two ways
to run them:

- On [colab](https://colab.research.google.com/), click on the links of
  each notebook to copy the notebook to *colab*. You require your own
  Google credentials to execute it.
- On a local instance of a Jupyter server, after the dependencies
  installation, launch Jupyter (copy the link displayed in the terminal
  on a Web browser) and click on a notebook from the list.

  ```bash
  jupyter notebook
  ```

In fact, there is a hybrid way to execute the notebooks. On *colab* you
can choose "Connect to local runtime" from the `Connect` toolbar.
To ensure the connection to a local Jupyter server, you have to activate
the appropiate extension:

```bash
jupyter serverextension enable --py jupyter_http_over_ws
```
