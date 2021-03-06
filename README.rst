Django Forms Bootstrap
======================

.. image:: http://slack.pinaxproject.com/badge.svg
   :target: http://slack.pinaxproject.com/

.. image:: https://img.shields.io/travis/pinax/django-forms-bootstrap.svg
    :target: https://travis-ci.org/pinax/django-forms-bootstrap

.. image:: https://img.shields.io/coveralls/pinax/django-forms-bootstrap.svg
    :target: https://coveralls.io/r/pinax/django-forms-bootstrap

.. image:: https://img.shields.io/pypi/dm/django-forms-bootstrap.svg
    :target:  https://pypi.python.org/pypi/django-forms-bootstrap/

.. image:: https://img.shields.io/pypi/v/django-forms-bootstrap.svg
    :target:  https://pypi.python.org/pypi/django-forms-bootstrap/

.. image:: https://img.shields.io/badge/license-MIT-blue.svg
    :target:  https://pypi.python.org/pypi/django-forms-bootstrap/


Pinax
------
Pinax is an open-source platform built on the Django Web Framework. It is an ecosystem of reusable Django apps, themes, and starter project templates. 
This collection can be found at http://pinaxproject.com.


django-forms-bootstrap
-----------------------

``django-forms-bootstrap`` is a simple bootstrap filter for Django forms. Extracted from the
bootstrap theme for Pinax.


Getting Started
-----------

Include ``django-forms-bootstrap`` in your requirements file and
``django_forms_bootstrap`` in your ``INSTALLED APPS``.

Make sure your template loader finders includes app directories.

To style forms, add the following to the top of your template ::
    
    {% load bootstrap_tags %}

and include your form using something like the following markup: ::
    
    <form>
        <legend>My Form</legend>
        {% csrf_token %}
        {{ form|as_bootstrap }}
        <div class="form-actions">
          <a href="#back" class="btn">Go back</a>
          <button type="submit" class="btn btn-primary">Save changes</button>
        </div>
    </form>


Specifying Form Layouts
-----------------------

Bootstrap includes styles for four types of forms. To change the display of
your form, add one of the following class attributes to your form tag:

==================  ================   ==============================================================
        Name             Class                        Description
==================  ================   ==============================================================
Vertical (default)  .form-vertical     Stacked, left-aligned labels over controls
Horizontal          .form-horizontal   Float left, right-aligned labels on same line as controls
Inline              .form-inline       Left-aligned label and inline-block controls for compact style
Search              .form-search       Extra-rounded text input for a typical search aesthetic
==================  ================   ==============================================================


Documentation
--------------

The django-forms-bootstrap documentation is currently under construction. If you would like to help us write documentation, please join our Pinax Project Slack channel and let us know! The Pinax documentation is available at http://pinaxproject.com/pinax/.


License & Attribution
---------------------

Django Forms Bootstrap is released under the MIT license. It does not include
any styles or scripts from the Bootstrap project.


Code of Conduct
----------------

In order to foster a kind, inclusive, and harassment-free community, the Pinax Project has a code of conduct, which can be found here  http://pinaxproject.com/pinax/code_of_conduct/.


Pinax Project Blog and Twitter
-------------------------------

For updates and news regarding the Pinax Project, please follow us on Twitter at @pinaxproject and check out our blog http://blog.pinaxproject.com.


