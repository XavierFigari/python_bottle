# Python project to experiment the Bottle web/database framework
This is a pretty cool framework to display web page templates (as in php/Laravel), and to access SQL databases.

Bottle is a fast, simple and lightweight WSGI micro web-framework for Python. It is distributed as a single file module and has no dependencies other than the Python Standard Library.

Install bottle with `pip install bottle`

For the "Hello world" demo that uses a simple Bottle route :

- run the application `python bottle1.py`
- access the web site with http://localhost:8080/hello/world (or http://localhost:8080/hello/xavier)

For the "Todo list" demo that makes use of Bottle routes and templates :

- create a database by running `python create_todolist_table.py`
- run the application `python todo.py`
- access the web site : http://localhost:8083/todo

The application executes `run(host='localhost', port=8083, reloader=True)`
The run() statement simply starts the web server included in Bottle.
Each @route statement then calls the corresponding Python function when the http address matches the route statement.

We will end up with an application with the following pages and functionality:

        start page http://localhost:8080/todo
        adding new items to the list: http://localhost:8080/new
        page for editing items: http://localhost:8080/edit/<no:int>
        catching errors


