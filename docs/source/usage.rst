.. _installation:

Installation
------------

To install checkoAPI:

.. code-block:: console

 $ pip install checkoAPI

Or

.. code-block:: console

$ git clone https://github.com/webcartel-https/checkoAPI

$ cd checkoAPI

$ python3 setup.py

Creating recipes
----------------

To retrieve a list of random ingredients,
you can use the ``lumache.get_random_ingredients()`` function:

.. autofunction:: lumache.get_random_ingredients

The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
or ``"veggies"``. Otherwise, :py:func:`lumache.get_random_ingredients`
will raise an exception.

.. autoexception:: lumache.InvalidKindError

For example:

>>> import lumache
>>> lumache.get_random_ingredients()
['shells', 'gorgonzola', 'parsley']

