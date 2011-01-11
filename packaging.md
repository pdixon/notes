# Debian Packaging

## Rebuilding Packages
Sometimes I find it convenient to rebuild packages for local use. Typical because
there is a new version available in the development repos [^1].

[^1]: Particular for editors I can't stand to be on anything but the very latest
    formal release. Anything else just seems wrong.

To get the source package:

~~~~{.sh}
apt-get source
~~~~

To rebuild the package:
    
~~~~{.sh}
debuild -uc -us
~~~~
This rebuilds the package, but doesn't attempt to sign it.

Sometimes the latest upstream release hasn't been packaged yet. In this case
once you have download the existing source package:

~~~~{.sh}
uscan
~~~~

should update the package to the latest upstream release (if the source package
has a watch file setup).

~~~~{.sh}
dch -v newversion
~~~~

will create an entry in the change log for the new version. Save this then
rebuild the package with:

~~~~{.sh}
debuild -uc -us
~~~~

