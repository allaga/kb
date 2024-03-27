su [options] [-] [user [argument...]]

su - user

su -l

-, -l, --login
           Start the shell as a login shell with an environment similar to a
           real login:

           •   clears all the environment variables except TERM and variables
               specified by --whitelist-environment

           •   initializes the environment variables HOME, SHELL, USER,
               LOGNAME, and PATH

           •   changes to the target user’s home directory

           •   sets argv[0] of the shell to '-' in order to make the shell a
               login shell
