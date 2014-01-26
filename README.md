cjdmanage
=========

A command line manager for handling a cjdns installation

Overview
--------
cjdmanage is a command line manager for managing `cjdns` (**C**aleb **J**ames **D**eLisle's **N**etwork **S**uite). If you know how to use `apt` on a *nix system, then you already have the basics of cjdmanage set out for you.

Syntax and Usage
----------------

* `cjdmanage install` Installs the latest version of `cjdns` to the subdirectory `./cjdns/`, pulled fresh from the GitHub repository
* `cjdmanage remove` Removes the installation of `cjdns` (moves your .conf file to `./cjdroute.conf` in case you need it)
* `cjdmanage update` Updates the copy of `cjdns` located in `./cjdns/` to the latest version pulled from GitHub
* `cjdmanage start` Starts cjdroute
* `cjdmanage stop` Stops all instances of cjdroute

Installation
------------

cjdmanage is written in Bash. Therefore, no compilation is necessary.

1. Pick a convenient location to clone cjdmanage to. cjdns will be installed into a subdirectory of this location, so choose wisely.
2. `git clone`
