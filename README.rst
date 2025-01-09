Project Elara Jupyterbook v2 Test Book
======================================

This is `a fork of the readthedocs Jupyterbook template <https://github.com/readthedocs-examples/example-jupyter-book>`_ used to test `Jupyterbook v2 <https://next.jupyterbook.org/>`_ for an eventual migration (see https://github.com/elaraproject/elara-handbook/issues/7).

To test, clone and enter the repo, then create a virtual env

.. code-block:: bash

	python -m venv .venv
	# Windows
	source .venv/Scripts/activate
	# Mac/Linux
	source .venv/bin/activate

Then install Jupyterbook v2:

.. code-block:: bash

	pip install "jupyter-book>=2"

Also make sure you have LaTeX installed, there are distributions with installers like `TeX Live <https://tug.org/texlive/>`_ or `MikTeX <https://miktex.org/>`_. Then to run the book on localhost do:

.. code-block:: bash

	jupyter book start

This creates a local web server to preview the web version. To build a PDF you must have LaTeX pre-installed. Then run:

.. code-block:: bash

	jupyter book build --pdf

This should output a book in the ``_build/exports/<somefile.pdf>``.
