Buildout Eggscleaner
======================

Introduction
------------
The buildout.eggscleaner extensions can be used to ensure your egg directory only contains 'used' eggs.
The extension can report, but also move unused eggs to a specified directory.


Installation
------------
Eggscleaner is a buildout extensions, can add it like so ::

    [buildout]
    extensions =
            buildout.eggscleaner


Options
----------
    old-eggs-directory
        The directory you want buildout.eggscleaner to move your unused eggs to.
        Should an excact egg already exist, we remove the one in the ''used'' eggs directory


    Example ::    

        [buildout]                                                                 
        extensions =                                                               
                buildout.eggscleaner  
        old-eggs-directory = ${buildout:directory}/old-eggs/

Tested under
-----------
Buildout 1.5.1 and 1.5.2
