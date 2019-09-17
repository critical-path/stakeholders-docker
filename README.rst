Introduction
============

Stakeholder management is critical to project management.  Inspired by the Project Management Body of Knowledge, this app helps project teams to perform the principal tasks associated with managing stakeholders.


Installing stakeholders-docker
==============================

stakeholders-docker is available on GitHub at https://github.com/critical-path/stakeholders-docker.  It is the Docker version of `stakeholders <https://github.com/critical-path/stakeholders>`__.

To install stakeholders-docker, run the following command from your shell.

.. code-block:: console

   [user@host ~]$ git clone git@github.com:critical-path/stakeholders-docker.git


Starting stakeholders-docker
============================

To start stakeholders-docker for the first time, run the following command from your shell.  This will build a container from scratch.

.. code-block:: console

   [user@host stakeholders-docker]$ docker-compose up --build

To restart it later, run the following command from your shell.

.. code-block:: console

   [user@host stakeholders-docker]$ docker-compose up


Using stakeholders-docker
=========================

Point your browser to any of the following URLs.

* :code:`http://localhost:8080/`
* :code:`http://localhost:8080/home`
* :code:`http://localhost:8080/index`

Then, add one or more stakeholders.

Next, add one or more deliverables.

Finally, add one or more associations between stakeholders and deliverables.  This will add content to your stakeholder management plan.


Notes on stakeholders-docker
============================

stakeholders-docker does not enforce constraints on the uniqueness of stakeholders, deliverables, or associations.  This is to avoid unnecessary complexity in the code.


Testing stakeholders-docker
===========================

To conduct testing, run the following command from your shell.

.. code-block:: console

   [user@host stakeholders-docker]$ docker-compose exec stakeholders pytest --cov --cov-report=term-missing
