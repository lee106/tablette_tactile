# tablette_tactile
Source code for tablette

Introduction

Tablette is a micro Python module to transform tabular data to nested lists of dicts.

Why

The purpose of the module is to make it easy to create JSON data starting from a database cursor. Yes. A database cursor, do you remember that? :)

How it works

As an example, consider this dataset:

columns = ['id', 'username', 'url_id', 'url', 'tag_id', 'tag']
data = [
        [ 1, 'albi', 1, 'http://python.org/', 1, 'programming language' ],
        [ 1, 'albi', 1, 'http://python.org/', 2, 'open source' ],
        [ 1, 'albi', 2, 'http://php.net/', 2, 'open source' ],
        [ 1, 'albi', 2, 'http://php.net/', 3, 'web' ],
        [ 2, 'karl', 3, 'http://reddit.com/', 4, 'lol' ],
        [ 2, 'karl', 3, 'http://reddit.com/', 5, 'wtf' ]
    ]

With this code, you will be able to know how to use a (tablette tactile)[https://www.besttech.fr] easily.
