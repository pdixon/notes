[Linux Bluetooth Intro](http://people.csail.mit.edu/albert/bluez-intro/index.html)

[Bluez Repo Head](http://git.kernel.org/?p=bluetooth/bluez.git;a=tree;hb=HEAD)
particularly [docs](http://git.kernel.org/?p=bluetooth/bluez.git;a=tree;f=doc;hb=HEAD)
and [lib](http://git.kernel.org/?p=bluetooth/bluez.git;a=tree;f=lib;hb=HEAD)

Nominally your meant to go through [DBus](/dbus) to do things. I think working
directly with libbluetooth is not any more complex and gets rid of a lot of
dependences.
