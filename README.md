# leverage-vizualization
leverage vizualization for futures trading

# Quick start

```bash
source pyenv396/bin/activate
# then run the notebook in VSCode
```

# How to create and run Jupyter notebook in VSCode running on M1 chipset

```bash
# create venv that will use Python version 3.9 (instead of default)
python3.9 -m venv pyenv396
source pyenv396/bin/activate

# install and run ipykernel to be able to run Jupyter from VSCode
pip install ipykernel
ipython kernel install --user --name=pyenv396
# update pip
pip3 install -U pip setuptools
pip install jupyter
pip install pandas
# this is a thing to install to be able to run numpy on M1 chipset
pip install spacy
pip install seaborn
# install this to use UI in Jupyter
pip install ipywidgets

# to deactivate venv, just run thid in the tab where activate was run
deactivate
```