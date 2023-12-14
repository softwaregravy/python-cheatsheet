# venv workflow

```bash
# ~/.zshrc
alias ae='deactivate &> /dev/null; source ./venv/bin/activate'
alias de='deactivate'
```

```bash
$ cd project
$ ae
(venv) $ # Work on the project...
$ de
```

[source](https://realpython.com/lessons/my-virtual-environments-workflow/)

## Install Package

```bash
python -m pip install <package-name>
```

## Create and consume requirements.txt

```bash
$ python -m pip freeze > requirements.txt

$ deactivate
$ python3 -m venv new-venv
$ source new-venv/bin/activate
$ python -m pip install -r requirements.txt
```

[venv reference](https://realpython.com/python-virtual-environments-a-primer/#how-can-you-work-with-a-python-virtual-environment)

