# Installing

## Python

If `sudo easy_install couchapp` doesn't work for you, you can install from source.

    git clone git://github.com/jchris/couchapp.git
    cd couchapp
    sudo python setup.py install

You may need to satisfy some dependencies. We hope this will happen automatically but... you never know.

## Installing on OS X Leopard

You may encounter an error resembling this when installing on OS X Leopard:

    No eggs found in /tmp/easy_install-s_Hq0s/simplejson-2.0.4/egg-dist-tmp-LjhqW1

If so, there is a problem with your `setuptools` library (the version included with Python 2.5 on OS X is broken). To upgrade:

    sudo easy_install "http://pypi.python.org/packages/2.5/s/setuptools/setuptools-0.6c9-py2.5.egg#md5=fe67c3e5a17b12c0e7c541b7ea43a8e6"

(or download the `.egg` corresponding to your version of Python from [the setuptools page](http://pypi.python.org/pypi/setuptools) and `easy_install` that).

## Questions and Comments

If you can improve this documentation, please send pull requests using Github or hit the [CouchApp mailing list](http://groups.google.com/group/couchapp). 

We want the install experience to go smoothly for **everyone**, so please send feedback and let us help you make this documentation cover troubleshooting problems.
