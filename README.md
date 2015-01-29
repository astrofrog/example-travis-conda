About
=====

[Travis CI](https://travis-ci.org) is a Continuous Integration service that
will run tests for your project anytime someone makes a change or opens a pull
request. However, every time a build starts on Travis, all the dependencies are
installed from scratch in a clean environment. Travis does include Python, but
if you try and install for example Numpy, Scipy, and Matplotlib from source,
the installation could take a while (over 20 minutes) for each build.

This repository contains a simple ``.travis.yml`` file to get you started with
testing your Python project on [Travis CI](https://travis-ci.org) using
[conda](http://conda.pydata.org/) to speed up the installation of dependencies.
Setting up a build with for example Python, Numpy, Scipy, Matplotlib, and
Astropy takes **only a minute**! This is possible because
[conda](http://conda.pydata.org/) installs pre-compiled binary packages.

Getting started
===============

To get started, copy over the ``.travis.yml`` file here to your repository, and
add/remove dependencies or builds in the matrix if needed. Then go to the
[Travis CI](https://travis-ci.org) website, sign in with your GitHub account,
then go to **Accounts** and turn on Travis for the repository you want to test.
Next time you push a change or open a pull request on your repository, Travis
will run the tests!

Note that in the example ``.travis.yml`` file, the command to run the tests is
currently set to ``py.test`` (in the ``script`` section) but you can change
this to anything you like.

More
====

You can find out more information about using conda on Travis in
[this official conda blog post](http://conda.pydata.org/docs/travis.html) blog
post - their example ``.travis.yml`` file is a little different, but both will
do the job. The one in this repository is a little simpler overall and includes
more inline comments.

Build status
============

[![Build Status](https://travis-ci.org/astrofrog/example-travis-conda.svg?branch=master)](https://travis-ci.org/astrofrog/example-travis-conda)
