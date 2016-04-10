# pydumper

*A clean wrapper for dumping and loading objects from disk.*

With this dumb little library, now you can dump and load objects without having to deal with those annoying file objects! You know what? You can even ignore those stupid file extensions and duplicate checking and let this package deal that for you!

## Installation

    pip install pydumper

## Examples

    >>> from dumper import dump, load
    >>> import random

    >>> dump([random.random() for i in range(1000)], "test") #"test.dat" is created in current working directory
    
    >>> obj = load("test") #"test.dat" is loaded
