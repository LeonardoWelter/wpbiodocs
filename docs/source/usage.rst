Como usar
=====

.. _installation:

Instalação
------------

Para instalar o WP Bio, primeiramente selecione a aba "Plugins" no menu administrativo do Wordpress:

.. figure:: docs/images/wpbio_tutorial_plugins_page2.png
   :width: 60%
   :align: center
   :alt: Wordpress Plugin Page

   Wordpress Plugin Page

Selecione "Adicionar Novo" no topo da página, e então selecione "Enviar Plugin":

.. figure:: docs/images/wpbio_tutorial_plugins_store2.png
   :width: 60%
   :align: center
   :alt: Wordpress Send Plugin

   Wordpress Send Plugin

To use Lumache, first install it using pip:

.. code-block:: console

   (.venv) $ pip install lumache

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

