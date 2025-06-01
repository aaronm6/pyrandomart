# pyrandomart
Python library to produce randomart text from a bytes object

This module contains a function to turn a bytes object into a randomart
string.
see: [http://www.dirk-loss.de/sshvis/drunken_bishop.pdf](http://www.dirk-loss.de/sshvis/drunken_bishop.pdf)
for a description of randomart

Only function in this file that is useful to import is 
the last one, 'randomart'. So the recommended usage is:
from pyrandomart import randomart
