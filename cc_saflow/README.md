SAflow (Sustained Attention and Flow)
==============================

This research project aims to investigate with MEG the neural correlates of attentional fluctuations during a modified version of a classical sustained attention task, namely the [GradCPT (Esterman et al., 2013)](https://academic.oup.com/cercor/article/23/11/2712/303412?login=true).
In this repository, you can find the experiment's source code, the related preprocessing and analysis scripts as well as the scripts generating the figures for the research article (WiP).

How to use :
- Download (and unzip) the repository.
- Create and activate a new Python environment if needed (via [venv](https://docs.python.org/3/library/venv.html) or [conda](https://uoa-eresearch.github.io/eresearch-cookbook/recipe/2014/11/20/conda/))
- Download the original data acquisition folder, store it in ./data, or anywhere else you'd like
- Open src/saflow_params.py and change the various paths to fit your file structure
-     python setup.py install


Project Organization
------------

    ├── LICENSE
    ├── Makefile           <- Makefile with commands like `make data` or `make train`
    ├── README.md          <- The top-level README for developers using this project.
    ├── data               <- Where the dataset will be installed
    ├── docs               <- A default Sphinx project; see sphinx-doc.org for details
    │
    ├── models             <- Trained and serialized models, model predictions, or model summaries
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-jqp-initial-data-exploration`.
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures        <- Generated graphics and figures to be used in reporting
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `pip freeze > requirements.txt`
    │
    ├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
    ├── src                <- Source code for use in this project.
    │   ├── __init__.py    <- Makes src a Python module
    │   │
    │   ├── data           <- Scripts to download or generate data
    │   │   └── generate_bids.py
    │   │   └── preprocessing.py
    │   │   └── segmentation.py    
    │   │
    │   ├── features       <- Scripts to turn raw data into features for modeling
    │   │   └── build_features.py
    │   │
    │   ├── models         <- Scripts to train models and then use trained models to make
    │   │   │                 predictions
    │   │   ├── predict_model.py
    │   │   └── train_model.py
    │   │
    │   └── visualization  <- Scripts to create exploratory and results oriented visualizations
    │       └── visualize.py
    │
    └── tox.ini            <- tox file with settings for running tox; see tox.testrun.org


--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
