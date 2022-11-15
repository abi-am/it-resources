The server has multipe versions of python.
To see available versions write ``python`` in terminal and press "Tab" button twice on your keyboard. 
To use or run specific version of python write available version rigth after the python like this: ``python3.9``

If you prefer to always use specific version of python, the simplest way would be to add an alias for desired version to always run that specific version when ``python`` called in your bash. Add this line in the end of ``~/.bashrc`` file.

``alias python="python3.9"``

Save modified file and run

``source ~/.bashrc``

Now python3.9 will be used when you call ``python`` in your bash profile.
