cjdmanage
=========

A command line manager for handling a cjdns installation

Overview
--------
cjdmanage is a command line manager for managing [`cjdns`](http://github.com/cjdelisle/cjdns) (**C**aleb **J**ames **D**eLisle's **N**etwork **S**uite). If you know how to use `apt` on a *nix system, then you already have the basics of cjdmanage set out for you.

Features (that are actually worth mentioning)
---------------------------------------------
* Install, remove, update, and manage the cjdroute service all from one program
* Don't have Git? Don't worry! cjdmanage can also download, install, and update with `wget` or `curl` instead (for that, you'll need `tar` or `unzip` installed though)

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

### One Line Install Method
**CAUTION: You should *always* review any code that you're asked to pipe from `curl` to `sh` - in this case however, the Bash script is right here in this repository, for your convenience.**

I'm still working on the one line install method. It should be done pretty soon.

### With Git
1. Pick a convenient location to clone cjdmanage to. cjdns will be installed into a subdirectory of this location, so choose wisely.
2. `git clone https://github.com/alebcay/cjdmanage.git`
3. `cd cjdmanage`
4. `chmod +x ./cjdmanage`
5. All set! See "Syntax and Usage" to get started.
<br />


*Note: You still need to find peers on Hyperboria or elsewhere in order to get off the ground. cjdmanage (and all the money in the world) can't buy you friends.*


### Without fussing with the doggone command line
1. Download the archive of the latest version:
   * ZIP: http://github.com/alebcay/cjdmanage/archive/master.zip
   * TAR.GZ: http://github.com/alebcay/cjdmanage/archive/master.tar.gz
2. Extract contents to a convenient location. cjdns will be installed into a subdirectory of this location, so choose wisely.
3. Enter the subdirectory `cjdmanage-master` (you can actually rename that to whatever you want).
4. Give execute permissions to the file `cjdmanage`.
5. In the end, you still need the command line. Maybe that's because it's a *command line tool*. See "Syntax and Usage" to get started.


*Note: You still need to find peers on Hyperboria or elsewhere in order to get off the ground. cjdmanage (and all the money in the world) can't buy you friends.*

Editing/Modifying
-----------------
cjdmanage is a Bash script, so just open it in a text editor and make whatever changes you want. Then save it and run it again.

Contributing
------------
If you care to contribute to cjdmanage, feel free to fork and send pull requests. I'll try my best to review them.
