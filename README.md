Features
========

This fork has the following features:

* Corrected support for multiple SOAP ports/bindings
* Support for both `import` and `include` stanzas in WSDL
* Support for a WSDL base directory to deal with relative pathnames in import/include stanzas
* Somewhat saner traceing/logging (traces now go to log.debug(), which you can handle per module)
* Somewhat more readable logic (by removing a bunch of helpers to a separate file)


Testing
=======

Using Python 2.7+:

    python -m unittest discover

Using older Python versions:

    python -m unittest tests/suite.py
  
Code coverage:

    sudo pip install coverage
    coverage run tests/suite.py
    coverage report -m 
    coverage html
    
    
Changes
=======

 * Includes Issue 152: Invalid WSDL params parsing WSDL with imported schema   (https://code.google.com/p/pysimplesoap/issues/detail?id=152)
 * Includes Issue 148: WSDL not reachable behind a Basic Authentication	Includes (https://code.google.com/p/pysimplesoap/issues/detail?id=148)

