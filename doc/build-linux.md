Building on Linux
===============

To install the required dependencies, run the following command:

For non GUI
$ sudo apt-get install git-core build-essential libssl-dev libboost-all-dev libdb5.3-dev libdb5.3++-dev libgtk2.0-dev libminiupnpc-dev qt4-qmake synaptic qt-sdk qt4-dev-tools libqt4-dev libdb++-dev miniupnpc -y

$ sudo apt-get install ntp unzip git build-essential libssl-dev libdb-dev libdb++-dev libboost-all-dev libqrencode-dev aptitude && aptitude install miniupnpc libminiupnpc-dev -y


For GUI
$ sudo apt-get install git-core build-essential libssl-dev libboost-all-dev libdb5.1-dev libdb5.1++-dev libgtk2.0-dev libminiupnpc-dev qt4-qmake mingw32 synaptic qt-sdk qt4-dev-tools libqt4-dev libqt4-core libqt4-gui libdb++-dev miniupnpc

Then grab the latest version of the source code from Github



To build the daemon, run the following commands

$ cd jumpcoin/src/leveldb

$ sudo chmod 755 *

$ sudo make clean

$ sudo make libleveldb.a libmemenv.a -j <threads>

$ cd ..

$ sudo make -f makefile.unix -j <threads

Optionally, debugging symbols can be removed from the binary to reduce it's size. This can be done using strip.

$ sudo strip jumpcoind

Then, to build the GUI, run the following commands:

$ cd ..

$ qmake

$ make

Troubleshooting:
-------------

Building miniupnpc
----------------

If your OS doesn't support libminiupnpc, you can build this manually by performing the following steps:

$ wget 'http://miniupnp.free.fr/files/download.php?file=miniupnpc-1.6.tar.gz' -O miniupnpc-1.6.tar.gz

$ tar -xzvf miniupnpc-1.6.tar.gz

$ cd miniupnpc-1.6
	
$ make

$	make install

Cleaning the build:
----------------=

If you have to clean your build environment you may have to rebuild LevelDB manually. This can be done using:

$ cd src/leveldb

$ chmod +x build_detect_platform

$ ./build_detect_platform

Ignore the usage errors (it still builds the relevent file) and now run:

$ make libleveldb.a libmemenv.a
