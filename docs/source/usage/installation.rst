Using conda
===========

.. code:: bash

    conda install -c conda-forge ipympl

    # If using JupyterLab
    conda install -c conda-forge nodejs
    jupyter labextension install @jupyter-widgets/jupyterlab-manager jupyter-matplotlib
    

Using pip
=========

.. code:: bash

    pip install ipympl

    # If using JupyterLab
    # Install nodejs: https://nodejs.org/en/download/
    jupyter labextension install @jupyter-widgets/jupyterlab-manager jupyter-matplotlib


For a development installation (requires nodejs):
=================================================

.. code:: bash

    git clone https://github.com/matplotlib/ipympl.git
    cd ipympl
    pip install -e .

    # If using classic Jupyter Notebook
    jupyter nbextension install --py --symlink --sys-prefix ipympl
    jupyter nbextension enable --py --sys-prefix ipympl

    # If using JupyterLab
    jupyter labextension install @jupyter-widgets/jupyterlab-manager --no-build
    jupyter labextension link ./js
    cd js && npm run watch
    # Launch jupyterlab as `jupyter lab --watch` in another terminal