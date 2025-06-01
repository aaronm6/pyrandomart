# pyrandomart
Python library to produce randomart text from a bytes object

This module contains a function to turn a bytes object into a randomart
string.
see: [http://www.dirk-loss.de/sshvis/drunken_bishop.pdf](http://www.dirk-loss.de/sshvis/drunken_bishop.pdf)
for a description of randomart

## Installation
Try either:

```shell
pip install pyrandomart
```
or directly from github
```shell
pip install git+https://github.com/aaronm6/pyrandomart.git
```

## Usage
The only function in this package that is useful to import is the last one, 'randomart'. So the recommended usage is:
```shell
>>> from pyrandomart import randomart
```

For example, to turn a bytes object consisting of byte values 30 through 60 into randomart and print:
```shell
>>> bobj = bytes(range(30,60))
>>> print(randomart(bobj, header='30-60', footer='no hash'))
┏━━━━━[30-60]━━━━━┓
┃@===+o.          ┃
┃XO.*+...         ┃
┃= o o . .        ┃
┃Xo     . .       ┃
┃+Oo     S .      ┃
┃BE.    . o .     ┃
┃=o.     . .      ┃
┃o.               ┃
┃.o.              ┃
┗━━━━[no hash]━━━━┛
```
