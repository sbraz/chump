Chump
=====
.. image:: https://badge.fury.io/py/chump.png
	:target: http://badge.fury.io/py/chump

Chump is an Apache2 Licensed, fully featured API wrapper for `Pushover <https://pushover.net>`_:

.. code-block:: pycon

	>>> from chump import Pushover
	>>> app = Pushover('vmXXhu6J04RCQPaAIFUR6JOq6jllP1')
	>>> app.is_authenticated
	True
	>>> user = app.get_user('KAGAw2ZMxDJVhW2HAUiSZEamwGebNa')
	>>> user.is_authenticated
	True
	>>> user.devices
	set([u'iPhone'])
	>>> message = u.send_message('Hi!')
	>>> message.id
	u'74f737c1f0c49b65ed511b97a70f4d37'


Installation
------------

Install chump just like everything else:

.. code-block:: bash

	$ pip install chump