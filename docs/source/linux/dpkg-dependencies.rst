.. title:: Installing dpkg Dependencies

Installing dpkg Dependencies
----

When installing a .deb package manually with dpkg, missing dependencies may cause errors. To resolve them, use the following commands:

.. code-block:: shell

    dpkg -i <package-name>.deb
    apt-get -f install

The first command installs the package, and the second fixes any missing dependencies automatically by fetching and installing the required packages.
