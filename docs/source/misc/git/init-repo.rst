.. _init-repo:

Git Repository initialisieren
=====================================================

1. Creating a new repository on the command line

.. code-block:: bash
    :linenos:

    touch README.md
    git init
    git checkout -b main
    git add README.md
    git commit -m "first commit"
    git remote add origin https://git.sirenthesiren.xyz/SirenTheSiren/berufsschule.git
    git push -u origin main

2. Pushing an existing repository from the command line

.. code-block:: bash
    :linenos:

    git remote add origin https://git.sirenthesiren.xyz/SirenTheSiren/berufsschule.git
    git push -u origin main
