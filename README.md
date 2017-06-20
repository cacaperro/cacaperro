Cacaperro (CACA)
===========

To compile on Linux (tested with Debian 8):

Install dependencies
--------------------
	sudo apt-get install build-essential libboost-all-dev openssl-dev libdb++-dev libdb-dev git qt-sdk libminiupnpc-dev

BerkeleyDB must be version 5.3.x

Compile CLI
-----------

	make -f makefile.unix USE_UPNP=-
	
Compile Qt client
-----------------

	qmake "USE_UPNP=-" Cacaperro-qt.pro
	make

Don't forget to add cacaperro.chickenkiller.com to the cacaperro.conf file in the .cacaperro folder for the bootstrap:

	addnode=cacaperro.chickenkiller.com

If the file does not exist create it in YOURHOMEFOLDER/.cacaperro
