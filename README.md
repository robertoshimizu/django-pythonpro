# Django-PythonPro

App deployed to Heroku at https://pythonprodjangors.herokuapp.com/ 

[![Build Status](https://travis-ci.org/robertoshimizu/django-pythonpro.svg?branch=master)](https://travis-ci.org/robertoshimizu/django-pythonpro)
[![Updates](https://pyup.io/repos/github/robertoshimizu/django-pythonpro/shield.svg)](https://pyup.io/repos/github/robertoshimizu/django-pythonpro/)
[![Python 3](https://pyup.io/repos/github/robertoshimizu/django-pythonpro/python-3-shield.svg)](https://pyup.io/repos/github/robertoshimizu/django-pythonpro/)
[![codecov](https://codecov.io/gh/robertoshimizu/django-pythonpro/branch/master/graph/badge.svg)](https://codecov.io/gh/robertoshimizu/django-pythonpro)

Django App development following [PythonPro](https://www.python.pro.br/) Course

### Instruction for use

1. Check the python version and define a global interpreter using pyenv:
```bash
pyenv which python
pyenv global
```
2. Install pipenv
```bash
pip install pipenv
```
3. Check if pipenv create a .venv folder inside project directory. Edit .bash_profile or .bashrc and add:
```bash
export PIPENV_VENV_IN_PROJECT=1
```

#### Install the dependencies using Pipenv

```bash
pipenv install
```
#### Activate Virtualenv

```bash
source .venv/bin/activate
```
Alternatively:
```bash
pipenv shell
```

### Remarks

1. This command `python manage.py runserver` spins a Django server. In the course, it is used an alias for it, which is:
``` 
alias mng='python $VIRTUAL_ENV/../manage.py'
```
which has been registerd in the .bash_profile (mac)

2. Heroku CLI, do not forget to inform the proper app. Examples:
``` 
heroku apps:info --app=pythonprodjangors
heroku apps:open --app=pythonprodjangors
```