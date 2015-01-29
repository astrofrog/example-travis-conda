About
=====

This repository contains a simple ``.travis.yml`` file to get you started with
testing your Python project, and uses [conda](http://conda.pydata.org/) to
speed up the installation of dependencies. Setting up a build with for example
Python, Numpy, Scipy, Matplotlib, and Astropy takes only a minute!

To get started, copy over the ``.travis.yml`` file here to your repository, and
add/remove dependencies or builds in the matrix if needed. Then go to the
[Travis CI](https://travis-ci.org) website, sign in with your GitHub account,
then go to **Accounts** and turn on Travis for the repository you want to test.
Next time you push a change or open a pull request on your repository, Travis
will run the tests!

Note that in the example ``.travis.yml`` file, the command to run the tests is
currently set to ``py.test`` (in the ``script`` section) but you can change
this to anything you like.
