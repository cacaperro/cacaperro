Cacaperro (CACA)
===========

###To compile on Linux (tested with Debian 8):

Install dependencies
--------------------
	sudo apt-get install build-essential libboost-all-dev openssl-dev libdb++-dev libdb-dev git qt-sdk libminiupnpc-dev

Compile CLI
-----------

	make -f makefile.unix USE_UPNP=-
	
Compile Qt client
-----------------

	qmake "USE_UPNP=-" Cacaperro-qt.pro
	make

