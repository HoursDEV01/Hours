Hours Core
=============

Setup
---------------------
Hours Core is the original Hours client and it builds the backbone of the network. It downloads and, by default, stores the entire history of Hours transactions (which is currently more than 7 GBs); depending on the speed of your computer and network connection, the synchronization process can take anywhere from a few hours to a day or more.

To download Hours Core, visit [Hours.org](https://Hours.org).

Running
---------------------
The following are some helpful notes on how to run Hours on your native platform.

### Unix

Unpack the files into a directory and run:

- `bin/Hours-qt` (GUI) or
- `bin/Hoursd` (headless)

### Windows

Unpack the files into a directory, and then run Hours-qt.exe.

### OS X

Drag Hours-Core to your applications folder, and then run Hours-Core.

### Need Help?

* See the documentation at the [Hours Wiki](https://Hours.info/)
for help and more information.
* Ask for help on [#Hours](http://webchat.freenode.net?channels=Hours) on Freenode. If you don't have an IRC client use [webchat here](http://webchat.freenode.net?channels=Hours).
* Ask for help on the [HoursTalk](https://Hourstalk.io/) forums.

Building
---------------------
The following are developer notes on how to build Hours on your native platform. They are not complete guides, but include notes on the necessary libraries, compile flags, etc.

- [OS X Build Notes](build-osx.md)
- [Unix Build Notes](build-unix.md)
- [Windows Build Notes](build-windows.md)
- [OpenBSD Build Notes](build-openbsd.md)
- [Gitian Building Guide](gitian-building.md)

Development
---------------------
The Hours repo's [root README](/README.md) contains relevant information on the development process and automated testing.

- [Developer Notes](developer-notes.md)
- [Release Notes](release-notes.md)
- [Release Process](release-process.md)
- [Source Code Documentation (External Link)](https://dev.visucore.com/Hours/doxygen/)
- [Translation Process](translation_process.md)
- [Translation Strings Policy](translation_strings_policy.md)
- [Travis CI](travis-ci.md)
- [Unauthenticated REST Interface](REST-interface.md)
- [Shared Libraries](shared-libraries.md)
- [BIPS](bips.md)
- [Dnsseed Policy](dnsseed-policy.md)
- [Benchmarking](benchmarking.md)

### Resources
* Discuss on the [HoursTalk](https://Hourstalk.io/) forums.
* Discuss general Hours development on #Hours-dev on Freenode. If you don't have an IRC client use [webchat here](http://webchat.freenode.net/?channels=Hours-dev).

### Miscellaneous
- [Assets Attribution](assets-attribution.md)
- [Files](files.md)
- [Fuzz-testing](fuzzing.md)
- [Reduce Traffic](reduce-traffic.md)
- [Tor Support](tor.md)
- [Init Scripts (systemd/upstart/openrc)](init.md)
- [ZMQ](zmq.md)

License
---------------------
Distributed under the [MIT software license](/COPYING).
This product includes software developed by the OpenSSL Project for use in the [OpenSSL Toolkit](https://www.openssl.org/). This product includes
cryptographic software written by Eric Young ([eay@cryptsoft.com](mailto:eay@cryptsoft.com)), and UPnP software written by Thomas Bernard.
