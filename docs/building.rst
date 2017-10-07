Building
========
The build stack uses the Rust_ development tools on your system. Install these
on your system with rustup_ if they are not already available.

.. _Rust: https://www.rust-lang.org
.. _rustup: https://www.rustup.rs

The following dependencies are also needed to build the project.

* CMake_: Needed by Cargo tool library dependency.
* Libssl_: Needed by Cargo tool library dependency.

.. _CMake: https://cmake.org
.. _Libssl: https://wiki.openssl.org/index.php/Libssl_API

A rkt_ container build script is included in the project repository and
provides an installation which can be used to build the project also. See the
description on building and running the container in the :ref:`dev` section
of this document for details.

.. _rkt: https://coreos.com/rkt

For macOS, RktMachine_ provides a CoreOS VM which supports developing using
the rkt container system.

.. _RktMachine: https://github.com/woofwoofinc/rktmachine

To build and test the project, use:

::

    cargo test