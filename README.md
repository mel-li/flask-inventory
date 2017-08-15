# flask-inventory

In this file, I will document how to setup flask-inventory. All commands you need to run in the terminal are prefixed by `$`.

First begin by cloning flask-inventory:

```
$ git clone https://github.com/mel-li/flask-inventory.git
```

You should have a new folder called `flask-inventory/`. Head into that directory:

```
$ cd flask-invetory/
```

Now, let's create bantam's virtual environment:

```
$ virtualenv flask
$ flask/bin/pip install -r requirements.txt
```

In the `flask-inventory/` directory run:

```
$ ./run.py --debug
```

This is the command that start's flask-inventory's Flask webserver. Now, open up your web browser and head to `localhost:5000`. You should see the home page.

If you want to run on an alternate port, enter the port number as another argument. This is useful anytime the default Flask port (5000) is in use.

```
$ ./run.py --debug 5001
```

To deploy to the flask-inventory fleet (`fleetctl` must be installed):

```
$ ./deploy.py
```
