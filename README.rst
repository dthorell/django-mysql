============
Django-MySQL
============

.. image:: https://img.shields.io/readthedocs/django-mysql?style=for-the-badge
   :target: https://django-mysql.readthedocs.io/en/latest/

.. image:: https://img.shields.io/github/actions/workflow/status/adamchainz/django-mysql/main.yml?branch=main&style=for-the-badge
   :target: https://github.com/adamchainz/django-mysql/actions?workflow=CI

.. image:: https://img.shields.io/badge/Coverage-100%25-success?style=for-the-badge
   :target: https://github.com/adamchainz/django-mysql/actions?workflow=CI

.. image:: https://img.shields.io/pypi/v/django-mysql.svg?style=for-the-badge
   :target: https://pypi.org/project/django-mysql/

.. image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge
   :target: https://github.com/psf/black

.. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=for-the-badge
   :target: https://github.com/pre-commit/pre-commit
   :alt: pre-commit

.. figure:: https://raw.github.com/adamchainz/django-mysql/main/docs/images/dolphin-pony.png
   :alt: The dolphin-pony - proof that cute + cute = double cute.

..

    | The dolphin-pony - proof that cute + cute = double cute.


Django-MySQL extends Django's built-in MySQL and MariaDB support their specific
features not available on other databases.


What kind of features?
----------------------

Includes:

* ``QuerySet`` extensions:

  * 'Smart' iteration - chunked pagination across a large queryset
  * ``approx_count`` for quick estimates of ``count()``
  * Query hints
  * Quick ``pt-visual-explain`` of the underlying query

* Model fields:

  * MariaDB Dynamic Columns for storing dictionaries
  * Comma-separated fields for storing lists and sets
  * 'Missing' fields: differently sized ``BinaryField``/``TextField`` classes,
    ``BooleanField``\s represented by BIT(1)

* ORM expressions for over 20 MySQL-specific functions
* A new cache backend that makes use of MySQL's upsert statement and does
  compression
* Status variable inspection and utility methods
* Named locks for easy locking of e.g. external resources
* Table lock manager for hard to pull off data migrations

To see them all, check out the exposition at
https://django-mysql.readthedocs.io/en/latest/exposition.html .

Requirements and Installation
-----------------------------

Please see
https://django-mysql.readthedocs.io/en/latest/installation.html .

Documentation
-------------

Every detail documented on
`Read The Docs <https://django-mysql.readthedocs.io/en/latest/>`_.
