Contributions
-------------

Contributions are welcome in the form of pull requests.

Once the implementation of a piece of functionality is considered to be bug
free and properly documented (both API docs and an example script),
it can be incorporated into the master branch.

To help developing `hnn-core`, you will need a few adjustments to your
installation as shown below.

##### Running tests

To run the tests using `pytest`, you need to have the git cloned `hnn-core`
repository with an editable pip install:

    $ git clone https://github.com/hnnsolver/hnn-core --depth 1
    $ cd hnn-core
    $ python setup.py develop

Then, install the following python packages:

    $ pip install flake8 pytest pytest-cov

##### Building the documentation

The documentation can be built using sphinx. For that, please additionally
install the following:

    $ pip install matplotlib sphinx numpydoc sphinx-gallery sphinx_bootstrap_theme pillow

You can build the documentation locally using the command:

    $ cd doc/
    $ make html

You will also need to install mne to run all the examples and tests successfully. Please find
the installation instructions on the [MNE website](http://martinos.org/mne/).