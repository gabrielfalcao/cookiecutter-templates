{{cookiecutter.project_name}}
=======

{{cookiecutter.project_short_description}}

.. image:: https://readthedocs.org/projects/{{cookiecutter.app_name}}/badge/?version=latest
   :target: http://{{cookiecutter.app_name}}.readthedocs.io/en/latest/?badge=latest
   :alt: Documentation Status
.. image:: https://travis-ci.org/{{cookiecutter.github_username}}/{{cookiecutter.app_name}}.svg?branch=master
    :target: https://travis-ci.org/{{cookiecutter.github_username}}/{{cookiecutter.app_name}}
.. |PyPI python versions| image:: https://img.shields.io/pypi/pyversions/{{cookiecutter.app_name}}.svg
   :target: https://pypi.python.org/pypi/{{cookiecutter.app_name}}
.. |Join the chat at https://gitter.im/{{cookiecutter.github_username}}/{{cookiecutter.app_name}}| image:: https://badges.gitter.im/{{cookiecutter.github_username}}/{{cookiecutter.app_name}}.svg
   :target: https://gitter.im/{{cookiecutter.github_username}}/{{cookiecutter.app_name}}?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge



Install
-------

.. code:: bash

   pip install {{cookiecutter.app_name}}


Documentation
-------------

`{{cookiecutter.app_name}}.readthedocs.io <https://{{cookiecutter.app_name}}.readthedocs.io/en/latest/>`_


Basic Usage
-----------


.. code:: python

    from {{cookiecutter.app_name}} import readme

    # demo your module

    readme.then.replace.this.usage.with_a_real_example_of(
        app_name="{{cookiecutter.app_name}}",
        full_name="{{cookiecutter.full_name}}",
        email="{{cookiecutter.email}}",
        project_short_description="{{cookiecutter.project_short_description}}",
        github_username="{{cookiecutter.github_username}}",
        project_name="{{cookiecutter.project_name}}",
        version="{{cookiecutter.version}}",
    )
