.. module:: chainerio

API Reference
=============

Toplevel Functions
------------------

.. autofunction:: open
.. autofunction:: open_as_container
.. autofunction:: list
.. autofunction:: create_handler
.. autofunction:: info
.. autofunction:: isdir
.. autofunction:: mkdir
.. autofunction:: makedirs
.. autofunction:: exists
.. autofunction:: rename
.. autofunction:: remove

.. autofunction:: set_root
.. autofunction:: get_root_dir

.. autoclass:: IO
   :members:
.. autoclass:: chainerio.filesystem.FileSystem
   :members:
.. autoclass:: chainerio.container.Container
   :members:

.. note:: With environment variable
          ``KRB5_KTNAME=path/to/your.keytab`` set, ``hdfs``
          handler automatically starts automatic and periodical
          updating Kerberos ticket using `krbticket
          <https://pypi.org/project/krbticket/>`_ . The update
          frequency is every 10 minutes by default.
.. note::
          Only the username in the first entry in The
          keytab will be used to update the Kerberos ticket.


Cache API
---------

.. currentmodule:: chainerio.cache

.. autoclass:: Cache
   :members:

.. autoclass:: NaiveCache
   :members:

.. autoclass:: FileCache
   :members: preserve, preload

Chainer Extensions API
----------------------

.. currentmodule:: chainerio.chainer_extensions

.. autofunction:: load_snapshot

.. currentmodule:: chainerio.chainer_extensions.snapshot_writers

.. autoclass:: SimpleWriter
   :members:
