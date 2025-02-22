PyMechanical documentation |version|
====================================

.. toctree::
   :hidden:
   :maxdepth: 3


   getting_started/index
   user_guide_scripting/index
   user_guide_session/index
   user_guide_embedding/index
   api/index
   examples/index
   contributing



Introduction
------------
PyMechanical is part of the larger `PyAnsys <pyansys_>`_
effort to facilitate the use of Ansys technologies directly from
Python. Its primary package, ``ansys-mechanical-core``, provides
scripting of Ansys Mechanical through Python.

With PyMechanical, you can integrate the simulation capabilities
of the Mechanical multiphysics solver directly into novel apps.
The ``ansys-mechanical-core`` package presents a Python-friendly
interface to drive the software that facilitates the use of Mechanical
scripting commands.

With PyMechanical, you can accomplish tasks like these:

- Accelerate the preparation of your simulations.
- Combine the expressiveness of general-purpose Python code to control
  the flow in your input decks with methods that drive the solver.
- Explore proof-of-concept studies or capture knowledge using interactive
  Jupyter notebooks.
- Tap the solver as the physics engine in your next AI app.

Contributions to this open source library are welcome. For more information,
see :ref:`ref_contributing`.


Mechanical scripting
--------------------
You can already perform scripting of Mechanical with Python from inside
Mechanical. PyMechanical leverages the same APIs as Mechanical but allows
you to run your automation from outside Mechanical. For more information
on using these APIs, see :ref:`ref_user_guide_scripting`.

Background
----------
PyMechanical contains two interfaces: a remote session and an embedded instance.

Remote session
^^^^^^^^^^^^^^
PyMechanical's  remote session is based on `gRPC <https://grpc.io/>`_.
Mechanical runs as a server, ready to respond to any clients.

PyMechanical provides a client to connect to a Mechanical server and make API
calls to this server.

For information on using a remote session, see
:ref:`ref_user_guide_session`.

Embedded instance
^^^^^^^^^^^^^^^^^

.. vale off

PyMechanical's embedded instance is based on `Python.NET <http://pythonnet.github.io/>`_.
Rather than starting a new process for Mechanical, a Mechanical object (which is
implemented in .NET) is directly loaded into Python memory using Python.NET. From
there, Mechanical's entire data model is available for use from Python code.

.. vale on

For information on using an embedded instance, see :ref:`ref_user_guide_embedding`.

Documentation and issues
------------------------
Documentation for the latest stable release of PyMechanical is hosted at `PyMechanical documentation
<https://mechanical.docs.pyansys.com/version/stable/>`_.

In the upper right corner of the documentation's title bar, there is an option for switching from
viewing the documentation for the latest stable release to viewing the documentation for the
development version or previously released versions.

You can also `view <https://cheatsheets.docs.pyansys.com/pymechanical_cheat_sheet.png>`_ or
`download <https://cheatsheets.docs.pyansys.com/pymechanical_cheat_sheet.pdf>`_ the
PyMechanical cheat sheet. This one-page reference provides syntax rules and commands
for using PyMechanical. 

On the `PyMechanical Issues <https://github.com/ansys/pymechanical/issues>`_ page,
you can create issues to report bugs and request new features. On the `PyMechanical Discussions
<https://github.com/ansys/pymechanical/discussions>`_ page or the `Discussions <https://discuss.ansys.com/>`_
page on the Ansys Developer portal, you can post questions, share ideas, and get community feedback. 

To reach the project support team, email `pyansys.core@ansys.com <pyansys.core@ansys.com>`_.

Project index
-------------

* :ref:`genindex`
