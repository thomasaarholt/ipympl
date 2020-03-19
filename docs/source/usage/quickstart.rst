.. _installation:

Quickstart
==========

Start the ipympl backend by calling ``%matplotlib widget`` in the notebook before creating figures with matplotlib. 

Things to add:

fig.canvas is a widget

Since the canvas is a widget, it has access to layout, margin, etc.
Use of plt.ioff() and plt.ion() to control automatic figure generation.

How to check that the widget backend is enabled programmatically (mpl.get_backend())

Differences between the implementation in notebook and lab?