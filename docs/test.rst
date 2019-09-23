Testing stakeholders-docker
===========================

To execute tests that do not require a web browser, run the following command from your shell.

.. code-block:: console

   [user@host stakeholders-docker]$ docker-compose exec stakeholders pytest -m "not browser" --cov --cov-report=term-missing
