.. _changelog:

ChangeLog
=========

Changes to the library are recorded here.

v0.4.5
------
  * Long outstanding connection bug fixed by Estefan Ortiz! This is caused when something awry happens with rexster's rexpro socket either caused by titan or caused by network outtage

v0.4.4
------
  * Remove unused graph features which polls every connection. - thanks to atmos

v0.4.3
------
  * Loosen six version requirement

v0.4.2
------
  * Connection Bugfix, connections that had thrown exceptions were sometimes unusable at this point, so fix logic to re-create the socket

v0.4.1
------
  * python languange support via jython connectors like gremlin-python - thanks to Brian Corbin

v0.4.0
------
  * Pooling support for Blueprints Wrapper and session management - thanks to aolieman

v0.3.3
------
  * Fix Pooling issue: always return connections back to the pool by nvie

v0.3.2
------
  * Support None in response

v0.3.1
------
  * Transaction handling fix by nvie

v0.3.0
------
  * Python 3 support finalized, backported for python2 compatibility

v0.2.2
------
  * Better Python 3.3 and 3.4 testing

v0.2.1
------
  * Bugfix for closing transaction - thanks to Ashald for fixing this

v0.2.0
------
  * Robust Reconnect and session handling
  * Allow Gevent, Eventlet and native python socket implementations
  * Concurrency options are optional to use the library
     * To install with gevent: ``pip install rexpro[gevent]``
     * To install with eventlet: ``pip install rexpro[eventlet]``
  * Documentation Improvements

v0.1.8
------
  * Naive Reconnect

v0.1.7
------
  * Documentation

v0.1.6
------

  * Reconnect handling
  * Testing against Celery
    * must use ``-P gevent`` flag, ``eventlet`` is known to immediately hang forever


v0.1.5
------

  * Hotfix for connection pooling context manager


v0.1.4
------

  * Connection Pooling and Green Thread Friendly sockets using the ``gevent`` library.
    * Using gevent.socket directly, no monkey patching.


v0.1.3
------

  * Hotfix for new setup.py ``install_requires``


v0.1.2
------

  * Authentication Fixed
  * Coverage Testing
  * Fixed broken tests.
