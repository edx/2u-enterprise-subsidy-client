2u-enterprise-subsidy-client
#############################

|pypi-badge| |ci-badge| |codecov-badge| |doc-badge| |pyversions-badge|
|license-badge| |status-badge|

Purpose
*******

Client for interacting with the enterprise-subsidy service.

Getting Started
***************

Developing
==========

One Time Setup
--------------
.. code-block::

  # Clone the repository into your ``[DEVSTACK]/src/`` folder
  git clone git@github.com:edx/2u-enterprise-subsidy-client.git
  # Use a service container that would reasonably install this client, e.g.
  cd [DEVSTACK]/enterprise-subsidy && make app-shell
  cd /edx/src/2u-enterprise-subsidy-client

  # Set up a virtualenv in a ``venv/`` directory
  # You might need to install virtualenv first:
  # apt-get update
  # apt-get install -y virtualenv
  virtualenv venv/
  make requirements

  # Ensure things are looking ok by running tests
  make test

Every time you develop something in this repo
---------------------------------------------
.. code-block::

  # Grab the latest code
  git checkout main
  git pull

  # Use a service container that would reasonably install this client, e.g.
  cd [DEVSTACK]/enterprise-subsidy && make app-shell
  cd /edx/src/2u-enterprise-subsidy-client

  # Activate the virtualenv
  source venv/bin/activate

  # Install/update the dev requirements
  make requirements

  # Run the tests and quality checks (to verify the status before you make any changes)
  make validate

  # Make a new branch for your changes
  git checkout -b <your_github_username>/<short_description>

  # Using your favorite editor, edit the code to make your change.
  # Run your new tests
  pytest ./path/to/new/tests

  # Run all the tests and quality checks
  make validate

  # Commit all your changes
  git commit ...
  git push

  # Open a PR and ask for review.

License
*******

The code in this repository is licensed under the AGPL 3.0 unless
otherwise noted.

Please see `LICENSE.txt <LICENSE.txt>`_ for details.

Contributing
************

Contributions are very welcome.
Please read `How To Contribute <https://edx.org/r/how-to-contribute>`_ for details.

This project is currently accepting all types of contributions, bug fixes,
security fixes, maintenance work, or new features.  However, please make sure
to have a discussion about your new feature idea with the maintainers prior to
beginning development to maximize the chances of your change being accepted.
You can start a conversation by creating a new issue on this repo summarizing
your idea.

The Open edX Code of Conduct
****************************

All community members are expected to follow the `Open edX Code of Conduct`_.

.. _Open edX Code of Conduct: https://edx.org/code-of-conduct/


Reporting Security Issues
*************************

Please do not report security issues in public. Please email security@openedx.org.

.. |pypi-badge| image:: https://img.shields.io/pypi/v/2u-enterprise-subsidy-client.svg
    :target: https://pypi.python.org/pypi/2u-enterprise-subsidy-client/
    :alt: PyPI

.. |ci-badge| image:: https://github.com/edx/2u-enterprise-subsidy-client/workflows/Python%20CI/badge.svg?branch=main
    :target: https://github.com/edx/2u-enterprise-subsidy-client/actions
    :alt: CI

.. |codecov-badge| image:: https://codecov.io/github/edx/2u-enterprise-subsidy-client/coverage.svg?branch=main
    :target: https://codecov.io/github/edx/2u-enterprise-subsidy-client?branch=main
    :alt: Codecov

.. |doc-badge| image:: https://readthedocs.org/projects/2u-enterprise-subsidy-client/badge/?version=latest
    :target: https://2u-enterprise-subsidy-client.readthedocs.io/en/latest/
    :alt: Documentation

.. |pyversions-badge| image:: https://img.shields.io/pypi/pyversions/2u-enterprise-subsidy-client.svg
    :target: https://pypi.python.org/pypi/2u-enterprise-subsidy-client/
    :alt: Supported Python versions

.. |license-badge| image:: https://img.shields.io/github/license/edx/2u-enterprise-subsidy-client.svg
    :target: https://github.com/edx/2u-enterprise-subsidy-client/blob/main/LICENSE.txt
    :alt: License

.. TODO: Choose one of the statuses below and remove the other status-badge lines.
.. |status-badge| image:: https://img.shields.io/badge/Status-Experimental-yellow
.. .. |status-badge| image:: https://img.shields.io/badge/Status-Maintained-brightgreen
.. .. |status-badge| image:: https://img.shields.io/badge/Status-Deprecated-orange
.. .. |status-badge| image:: https://img.shields.io/badge/Status-Unsupported-red
