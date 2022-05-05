Usage
=====

.. _installation:

Installation
------------

To use Arora, first install it using pip:

.. code-block:: console

   (.venv) $ pip install Arora

.. _basicmathematicalfeatures:

For example:

>>> import arora
>>> lumache.get_random_ingredients()
['shells', 'gorgonzola', 'parsley']

Basic Mathematic Features
-------------------------

.. _mean
Mean
----

To get the mean of a particular signal you can use the ``arora.math.mean_val()``

.. autofunction:: arora.math.mean_val()

For example:

>>> import arora
>>> arora.math.mean_val()
['shells', 'gorgonzola', 'parsley']



.. _standarddeviation
Standard Deviation
------------------

To get the standard deviation of a particular signal you can use the ``arora.math.std_val()``

.. autofunction:: arora.math.std_val()


.. _skewness
Skewness
--------

To get skewness ``arora.math.compute_skew()``

.. autofunction:: arora.math.compute_skew()



To retrieve a list of random ingredients,
you can use the ``lumache.get_random_ingredients()`` function:

.. autofunction:: lumache.get_random_ingredients



.. autoexception:: lumache.InvalidKindError

For example:

>>> import lumache
>>> lumache.get_random_ingredients()
['shells', 'gorgonzola', 'parsley']

The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
or ``"veggies"``. Otherwise, :py:func:`lumache.get_random_ingredients`
will raise an exception.


arora.core.get_signal
---------------------
``arora.core.get_signal(file, signal_name )``

	Parameters:
		file : an .edf file
            The edf file that is to be imported

		signal_name : str or list[str] or List[dict]
                The name of the signals that is wanted, can also be a list of signals that are wanted

	Returns: list of all the signals that were requested

