# How to create-activate-deactivate venv env in python
```
# Create
python3 -m venv my_env

# Activate
source venv/bin/activate

# Deactivate
deactivate

```

# For poetry

```
pyenv install 3.12.0 o quello che vogliamo

poetry new test_ipynb
cd test_ipynb

poetry env use *Specific version of python* or poetry env use /usr/bin/python3.12

poetry env info

poetry add ipykernel and other libraries

poetry run pip list

poetry install

poetry run pip list

poetry lock

poetry install

poetry run python -m ipykernel install --user --name=transformer_poetry --display-name "New Display Name"

In the top right, click on the Select Kernel.

And select the environment you got from the env info command.
```

# Create new env
```
pyenv install <VERSION>
poetry env use /full/path/to/python (find into user)
poetry install
```

# Other guide:
```
poetry new <Name Poetry>

cd <Nome Poetry>

poetry config virtualenvs.in-project true --local

# Create a virtual environment
poetry shell

poetry add ipykernel and other libraries

poetry run python -m ipykernel install --user --name=transformer_poetry --display-name "New Display Name"

# If we want to update something we use:
poetry update

# if we want to remove a package we use:
poetry remove <package name>

# if we want to install a specific version of a package we use:
poetry add <package name>@<version>

# If we want to install the latest version of a package we use:
poetry add <package name>@latest

# If we want to start the venv we use:
poetry shell

# For the first time we have to install the dependencies:
poetry install
```