Sentry debian package maker
===========================

The code in this repository creates a deb that can be used to install sentry
on a host. It is not highly generic and may only work well for the author.

Notes
-----

The package will be created simply by running `mkdeb.sh`. It assumes that you
are building the package on the same target architecture as that which you are
installing to - e.g. 64bit Ubuntu, for example.

This assumption is due to the fact that, to speed up installation on target
machines, the deb packages together lots of pip Wheels which can have non
pure python modules compiled for the platform.
