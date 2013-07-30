Plone Buildout Example
======================

This repository contains an example buildout for Plone, with development,
staging and production setups.

The easiest way to use it is to click the "Download ZIP" link that should be
on the frontpage of the Github repository, and expand that. Create a
buildout.cfg pointing to the buildout you want (typically development.cfg at
this stage)::

    [buildout]
    extends = development.cfg

and run normally::

    $ python2.7 bootstrap.py
    $ bin/buildout

Before using the buildout seriously you should change the 'latest' links in
versions.cfg to the specific Plone version you want, ie change this::

    extends = 
        http://dist.plone.org/release/4.3-latest/versions.cfg
    
    find-links = 
        http://dist.plone.org/release/4.3-latest
        http://dist.plone.org/thirdparty


To this::

    extends = 
        http://dist.plone.org/release/4.3.1/versions.cfg
    
    find-links = 
        http://dist.plone.org/release/4.3.1
        http://dist.plone.org/thirdparty


Author
------

Lennart Regebro <regebro@gmail.com>

