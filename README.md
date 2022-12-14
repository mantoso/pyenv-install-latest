# pyenv-install-latest

This [pyenv](https://github.com/yyuu/pyenv) plugin to install the latest version of Python.

## Usage

```shell
pyenv install-latest [--print] [<`pyenv install` options>] [<version-prefix>]
```

## Installation

```shell
git clone https://github.com/mantoso/pyenv-install-latest.git ${HOME}/.pyenv/plugins/pyenv-install-latest
```

Or, if your `pyenv` is not installed in your home directory

```shell
git clone https://github.com/mantoso/pyenv-install-latest.git "$(pyenv root)"/plugins/pyenv-install-latest
```

## Usage example

Install the latest version of Python.

```shell
$ pyenv install-latest
Install 3.5.2...
Downloading Python-3.5.2.tar.xz...
-> https://www.python.org/ftp/python/3.5.2/Python-3.5.2.tar.xz
Installing Python-3.5.2...
patching file Lib/venv/scripts/posix/activate.fish
Installed Python-3.5.2 to /home/username/.pyenv/versions/3.5.2
```

Install 2.7-based version of Python.

```shell
$ pyenv install-latest 2.7
Install 2.7.12...
Downloading Python-2.7.12.tar.xz...
-> https://www.python.org/ftp/python/2.7.12/Python-2.7.12.tar.xz
Installing Python-2.7.12...
Installed Python-2.7.12 to /home/username/.pyenv/versions/2.7.12
```

Print, but not install the latest 2.7-based version of Python

    $ pyenv install-latest --print 2.7
    2.7.15
