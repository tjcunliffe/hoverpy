[![PyPI version](https://badge.fury.io/py/hoverpy.svg)](https://testpypi.python.org/pypi/hoverpy) [![RTD badget](https://readthedocs.org/projects/hoverpy/badge/?version=latest)](http://hoverpy.readthedocs.io/en/latest/)[![Build Status](https://travis-ci.org/SpectoLabs/hoverpy.svg?branch=master)](https://travis-ci.org/SpectoLabs/hoverpy)

![](https://github.com/SpectoLabs/hoverpy/raw/master/docs/source/hoverpy_logo.png)

### Documentation

https://hoverpy.readthedocs.io/

### Source

https://github.com/SpectoLabs/hoverpy/

### Motivation

HoverPy speeds up and simplifies tests that depend on HTTP / HTTPS services. It does so by recording all HTTP traffic generated by your python application inside a database file. 

When you run your code again, it plays back the responses corresponding to your requests. This means during the simulate phase, no HTTP traffic gets generated whatsoever. This grants several benefits:

- Increased test speed
- Ability to work offline
- Ability to modify traffic
- Ability to simulate network latency
- Deterministic test environment

If/when the service you are testing against changes its API, then you can simply delete your db file, and capture the test results again. HoverPy uses a [very high performance proxy written in Go](http://hoverfly.io), for this reason it is rock solid in terms of speed and reliability.

### Support

HoverPy works great with the following HTTP clients:

- requests
- urllib2
- urllib3
- TBD

### License

HoverPy uses Apache License V2. See LICENSE.txt for more details.