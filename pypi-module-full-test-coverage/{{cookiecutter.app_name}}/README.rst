.. Flask Chemist documentation master file, created by
   sphinx-quickstart on Sun Nov 19 22:16:39 2017.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Chemist
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

    from {{cookiecutter.app_name}} import (
        Model, db, MetaData,
        get_or_create_engine,
    )

    metadata = MetaData()
    engine = get_or_create_engine('sqlite:///example.db')

    class BlogPost(Model):
          table = db.Table('blog_post',metadata,
              db.Column('id', db.Integer, primary_key=True),
              db.Column('title', db.Unicode(200), nullable=False),
              db.Column('content', db.UnicodeText, nullable=False),
         )

    post1 = BlogPost.create(title='Hello World', content='\n'.join([
        'Introduction...',
        'Supporting Theory 1...',
        'Supporting Theory 2...',
        'Supporting Theory 3...',
        'Conclusion',
    ]))


    for post in BlogPost.all():
        print(post.title, post.id)


Examples
--------

1. `flask app <https://github.com/{{cookiecutter.github_username}}/{{cookiecutter.app_name}}/blob/master/examples/flask-app.py>`_
