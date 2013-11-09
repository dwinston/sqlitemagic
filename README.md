sqlitemagic
===========

A magic for the IPython Notebook for interacting with SQLite
databases.  The database filename goes on the first line; the query is
all following lines (so that long queries can be formatted nicely).

Usage:

    %%sqlite filename.db
    select personal, family from person;

    Alan|Turing
    Grace|Hopper

Every query is processed independently: the magic makes a new database
connection, creates a cursor, sends the query, and displays all the
results.

This magic was inspired by https://github.com/tkf/ipython-sqlitemagic.
