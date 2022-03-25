Benutzung
=====

.. _Schnellstart:

Schnellstart
------------

Um das Webhook-System verwenden zu können benötigen sie folgende Rechte:

.. code-block:: console

   webhook_system

Erstellen einer Webhook-Aktion
------------------------------

Ziehen Sie zum Erstellen einer Webhookaktion das Symbol aus der
Aktionsleiste in den Kampagnenmanager in eine Kampagne.

.. autofunction:: lumache.get_random_ingredients

The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
or ``"veggies"``. Otherwise, :py:func:`lumache.get_random_ingredients`
will raise an exception.

.. autoexception:: lumache.InvalidKindError

For example:

>>> import lumache
>>> lumache.get_random_ingredients()
['shells', 'gorgonzola', 'parsley']

