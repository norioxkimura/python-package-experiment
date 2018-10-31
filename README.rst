====
acme
====

.. image:: https://travis-ci.org/norioxkimura/python-package-experiment.svg?branch=master
    :target: https://travis-ci.org/norioxkimura/python-package-experiment

Sample Session
--------------

Ubuntu:

.. code-block:: shell-session

    $ sudo apt-get install -y python-minimal virtualenv
    $ virtualenv /tmp/test
    $ . /tmp/test/bin/activate
    $ pip install -U pip setuptools wheel
    $ pip list
    Package       Version
    ------------- -------
    pip           18.1
    setuptools    40.5.0
    wheel         0.32.2
    
    $ git clone https://github.com/norioxkimura/python-package-experiment.git
    $ cd python-package-experiment
    $ pip install -e .
    $ hello
    I am acme.core.hello()
    $ which hello
    /tmp/test/bin/hello
    
    $ pip install -e .[dev]
    $ pytest
    ...
    $ tox
    ...

License
-------
