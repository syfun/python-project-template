# Python Project Simple Template

## pakcage requirement

```
├── requirements
│   ├── base.txt       # project base pakcage
│   ├── local.txt      # project develop pakcage
│   └── production.txt # production package
└── requirements.txt   # production package
```


## private packages

`packages` folder save private packages. You can use like this in requirement.txt

```
django==3.0.1
# ...

./packages/example.tgz
```

## environment recommaned

Use [pyenv](https://github.com/pyenv/pyenv) to manage python environment.

exmaple:

```
$ pyenv virtualenv example 3.8.2
$ pyenv local example
$ pyenv shell example
$ pip install -r requirements/local.txt
```

## commit hook

Use [pre-commit](https://pre-commit.com/) hook.

Contains hooks:

- isort
- black
- flake8
