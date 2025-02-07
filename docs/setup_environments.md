# Creating a Basic Python Environment
## Install PyENV
```sh
curl -fsSL https://pyenv.run | bash
```

## Configure PyENV
Edit your shell configuration file (e.g. ~/.bashrc or ~/.zshrc) and add the following lines:
```sh
export PYENV_ROOT="$HOME/.pyenv"
[[ -d $PYENV_ROOT/bin ]] && export PATH="$PYENV_ROOT/bin:$PATH"
eval "$(pyenv init -)"
eval "$(pyenv virtualenv-init -)"
export REQUESTS_CA_BUNDLE=/etc/ssl/certs/ca-certificates.crt
```

## Install Python
```sh
pyenv install 3.12.8
pyenv global 3.12.8
pip install --upgrade pip
```

## Install Poetry in the Base Python Environment
```sh
pip install poetry
```

## Configure Global Poetry Settings
```sh
poetry config virtualenvs.in-project true
```
