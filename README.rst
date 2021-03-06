=============================
djangocms-admindocs-style
=============================

.. image:: https://badge.fury.io/py/djangocms-admindocs-style.png
    :target: https://badge.fury.io/py/djangocms-admindocs-style

.. image:: https://travis-ci.org/goldhand/djangocms-admindocs-style.png?branch=master
    :target: https://travis-ci.org/goldhand/djangocms-admindocs-style

Adds DjangoCMS Admin Styles to the admindocs.

Documentation
-------------

The full documentation is at https://djangocms-admindocs-style.readthedocs.org.

Quickstart
----------

Install djangocms-admindocs-style::

    pip install djangocms-admindocs-style

Then use it in a project by adding it to your installed apps before 'django.contrib.admin' and 'djangocms_admin_style'::

    INSTALLED_APPS = [
        ...
        'djangocms_admindocs_style',
        'djangocms_admin_style',
        'django.contrib.admin',
        'django.contrib.admindocs',
        ...
    ]

Features
--------

* Adds styles from `djangomcs_admin_style <https://github.com/divio/djangocms-admin-style>` to the ``django.contrib.admindocs`` app.
* Makes ``django.contrib.admindocs`` templates all inherit from a single base template that you can extend: ``admin/base_admin_docs.html``
* Adds a link to the DjangoCMS toolbar to a sidebar item

Running Tests
--------------

Does the code actually work?

::

    source <YOURVIRTUALENV>/bin/activate
    (myenv) $ pip install -r requirements-test.txt
    (myenv) $ python runtests.py

Compiling CSS
-------------

Make sure `sassc` is installed and run::

    npm run sass
