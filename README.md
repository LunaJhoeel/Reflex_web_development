# Commands

Install local pyenv
```bash
pyenv local 3.11
```

Check local pyenv
```bash
pyenv versions
pyenv local
```

Install pipx with pyenv 3.11
```bash
sudo apt update
python -m pip install --user pipx
python -m pipx ensurepath
source ~/.bashrc
echo 'export PIP_PYTHON_PATH="$(pyenv which python)"' >> ~/.bashrc
source ~/.bashrc
```

Check pipx version with pycowsay
```bash
pipx list
pipx install cowsay
pipx run pycowsay mooooo
pipx uninstall cowsay
```

Install poetry
```bash
pipx install poetry
pipx list
pipx upgrade poetry
poetry completions bash >> ~/.bash_completion
```
restart

Create Poetry environment
```bash
poetry init
```
(enter, enter, enter; etc)

Remove Poetry environment
```bash
poetry env remove 3.11.8
```

Activate Poetry virtual environment
```bash
poetry shell
```

Deactivate Poetry virtual environment
```bash
exit
deactivate
```

Add/remove dependencies examples
```bash
poetry add reflex
poetry remove reflex

poetry show --all

poetry add pytest --group test
```

Initialize project
```bash
reflex init
```

Run project
```bash
reflex run
```

Dev
```bash
poetry install
```

Prod
```bash
poetry install --without test
```

Local run
```bash
poetry run python app.py
poetry run pytest tests
```

