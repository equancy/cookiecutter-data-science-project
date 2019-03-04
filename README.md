# Equancy Cookiecutter Data Science Project

_Flexible data science project structure for doing data science use case._


### Requirements to use the cookiecutter template:
-----------
 - Python 2.7 or 3.x
 - [Cookiecutter Python package](http://cookiecutter.readthedocs.org/en/latest/installation.html) >= 1.4.0: This can be installed with pip by or conda depending on how you manage your Python packages:

``` bash
$ pip install cookiecutter
```

or

``` bash
$ conda config --add channels conda-forge
$ conda install cookiecutter
```


### To start a new project, run:
------------

    cookiecutter http://git.equancy.cloud/tools/cookiecutter-data-science-project


### The resulting directory structure
------------

The directory structure of your new project looks like this:

```
├── LICENSE            <- Equancy all rights reserved.
├── Makefile           <- Makefile with commands like `make data` or `make train`.
├── README.md          <- The top-level README for developers using this project.
│
├── _can_be_deleted    <- Trash bin (!! git ignored)
│
├── confidential       <- Confidential documents, data, etc. (!! git ignored)
│
├── data               <- !! git ignored
│   ├── external       <- Data from third party sources.
│   ├── processed      <- The final, canonical data sets for modeling.
│   ├── raw            <- The original, immutable data dump.
│   └── working        <- Working, intermediate data that has been transformed.
│
├── docs               <- A default Sphinx project; see sphinx-doc.org for details
│
├── models             <- Trained and serialized models, model predictions, or model summaries
│                         Also includes sklearn & pyspark pipelines.
│
├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
│                         the creator's initials, and a short `-` delimited description, e.g.
│                         `1.0-rvm-initial-data-exploration`.
│
├── production
│   ├── config         <- YAML files with dependancies between tasks, data catalog and others.
│   ├── pipelines      <- sklearn & pyspark pipelines.
│   ├── tasks          <- Luigi tasks.
│   └── scripts        <- Functions used by Luigi tasks.
│
├── references         <- Data dictionaries, manuals, and all other explanatory materials.
│
├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
│   └── figures        <- Generated graphics and figures to be used in reporting
│
├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
│                         generated with `pip freeze > requirements.txt`
│
├── src                <- Source code for use in this project.
│   ├── __init__.py    <- Makes src a Python module
│   │
│   ├── data           <- Scripts to download or generate data
│   │   └── make_dataset.py
│   │
│   ├── features       <- Scripts to turn raw data into features for modeling
│   │   └── build_features.py
│   │
│   ├── models         <- Scripts to train models and then use trained models to make
│   │   │                 predictions
│   │   ├── predict_model.py
│   │   └── train_model.py
│   │
│   └── visualization  <- Scripts to create exploratory and results oriented visualizations
│       └── visualize.py
│
└── tox.ini            <- tox file with settings for running tox; see tox.testrun.org
```

### Installing development requirements
------------

    pip install -r requirements.txt

### Running the tests
------------

    py.test tests

## Inspiration

From [DrivenData](https://drivendata.github.io/cookiecutter-data-science).
