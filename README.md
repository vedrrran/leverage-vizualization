# leverage-vizualization
Leverage vizualization for futures trading.

The package was tested only on Apple M1 chipset.

# How to use the package

The best way to use the repo would be by running it in venv and executing in VSCode.

```bash
# clone the repo and make a venv from it
git clone https://github.com/vedrrran/leverage-vizualization.git
python3.9 -m venv leverage-vizualization

# go to repo and start venv
cd leverage-vizualization
source bin/activate

# install requirements
pip install -r requirements.txt

# start kernel that will be used by VSCode
ipython kernel install --user --name=leverage-vizualization

# then deactvate and activate venv - I had to do this step to have kernel listed in VSCode :)
deactivate
source bin/activate

# Run the cell with code in VSCode
# choose 'leverage-vizualization':venv as a kernel
```

# Quick start

```bash
source leverage-vizualization/bin/activate
# then run the notebook in VSCode
```

# Extra: How to create and run Jupyter notebook in VSCode running on M1 chipset

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