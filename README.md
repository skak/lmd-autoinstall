lmd-autoinstall
===============

Automatically clone, build, and install libimobiledevice from github.com/libimobiledevice.

1. Run lmd-cloner
2. Run lmd-install

I don't know if what I've created is considered correct.
It works for me. I use Slackware 14.1.
It's just shell script and a modified Makefile.

It uses git to clone the repos from the libimobiledevice github repo set and then builds and installs them.
I'm not sure how to use (sed perhaps?) to insert -lncurses into a certain line in a certain makefile (/libirecovery/tools/Makefile) so that it will compile in Slackware, so I included 
the modified file and just used an if statement to copy it.

It clones, but does not build or install sbmanager. I do not need sbmanager and it requires libclutter and I do not care enough to fit that together.

Enjoy.
