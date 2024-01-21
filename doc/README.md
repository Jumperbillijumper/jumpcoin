Jumpcoin
=============

Setup
---------------------
Jumpcoin is a Jumpcoin client and it builds the backbone of the network. However, it downloads and stores the entire history of Jumpcoin transactions (which is currently several GBs); depending on the speed of your computer and network connection, the synchronization process can take anywhere from a few hours to a day or more.

To download Jumpcoin, visit [jumpcoin.net](https://jumpcoin.net).

Running
---------------------
The following are some helpful notes on how to run Jumpcoin on your native platform.

### Unix

Unpack the files into a directory and run:

- `bin/jumpcoin-qt` (GUI) or
- `bin/jumpcoind` (headless)

### Windows

Unpack the files into a directory, and then run jumpcoin-qt.exe.

### OS X

Drag Jumpcoin.app to your applications folder, and then run Jumpcoin.

### Need Help?

* See the documentation at the [Bitcoin Wiki](https://en.bitcoin.it/wiki/Main_Page)
for help and more information.
* Ask for help on [#jumpcoin](http://webchat.freenode.net?channels=jumpcoin) on Freenode. If you don't have an IRC client use [webchat here](http://webchat.freenode.net?channels=jumpcoin).
* Ask for help in [Jumpcoin room](https://gitter.im/BlackCoin_Hub) on Gitter.
* Ask for help in [/r/jumpcoin/](https://nm.reddit.com/r/jumpcoin/) on Reddit.
* Ask for help on the [BitcoinTalk](https://bitcointalk.org/) forums, in the [Jumpcoin topic](https://bitcointalk.org/index.php?topic=3017838.new#new).

Building
---------------------
The following are developer notes on how to build Jumpcoin on your native platform. They are not complete guides, but include notes on the necessary libraries, compile flags, etc.

- [OS X Build Notes](build-osx.md)
- [Unix Build Notes](build-unix.md)
- [Windows Build Notes](build-windows.md)
- [OpenBSD Build Notes](build-openbsd.md)
- [Gitian Building Guide](gitian-building.md)

Development
---------------------
The Jumpcoin repo's [root README](/README.md) contains relevant information on the development process and automated testing.

- [Developer Notes](developer-notes.md)
- [Multiwallet Qt Development](multiwallet-qt.md)
- [Release Notes](release-notes.md)
- [Release Process](release-process.md)
- [Source Code Documentation (External Link)](https://dev.visucore.com/bitcoin/doxygen/)
- [Translation Process](translation_process.md)
- [Translation Strings Policy](translation_strings_policy.md)
- [Unit Tests](unit-tests.md)
- [Unauthenticated REST Interface](REST-interface.md)
- [Shared Libraries](shared-libraries.md)
- [BIPS](bips.md)
- [Dnsseed Policy](dnsseed-policy.md)
- [Benchmarking](benchmarking.md)

### Resources
* Discuss on the [BitcoinTalk](https://bitcointalk.org/) forums, in the [Jumpcoin topic](https://bitcointalk.org/index.php?topic=3017838.new#new).
* Discuss Jumpcoin development in [Jumpcoin room](https://gitter.im/BlackCoin_Hub) on Gitter.
* Discuss Jumpcoin development in [Jumpcoin team](https://keybase.io/team/jumpcoin) on Keybase.

### Miscellaneous
- [Assets Attribution](assets-attribution.md)
- [Files](files.md)
- [Tor Support](tor.md)
- [Init Scripts (systemd/upstart/openrc)](init.md)

License
---------------------
Distributed under the [MIT software license](http://www.opensource.org/licenses/mit-license.php).
This product includes software developed by the OpenSSL Project for use in the [OpenSSL Toolkit](https://www.openssl.org/). This product includes
cryptographic software written by Eric Young ([eay@cryptsoft.com](mailto:eay@cryptsoft.com)), and UPnP software written by Thomas Bernard.
