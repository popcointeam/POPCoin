POPCoin
==========================================

Copyright (c) 2009-2013 Bitcoin Developers
Copyright (c) 2011-2013 Litecoin Developers
Copyright (c) 	   2014 StartJOIN
Copyright (c) 	   2017 POPCoin Team

What is POPCoin?
----------------

An open source, global payment network that is fully decentralized without any central authorities. Mathematics secures the network and empowers individuals to control their own finances

License
-------

POPCoin is released under the terms of the MIT license. See `COPYING` for more
information or see http://opensource.org/licenses/MIT.

### Building POPCoin

See doc/readme-qt.rst for instructions on building POPCoin-Qt,
the intended-for-end-users, nice-graphical-interface, reference
implementation of POPCoin.

See doc/build-*.txt for instructions on building popcoind,
the intended-for-services, no-graphical-interface, reference
implementation of POPCoin.



### Automated Testing

Developers are strongly encouraged to write unit tests for new code, and to
submit new unit tests for old code.

Unit tests for the core code are in `src/test/`. To compile and run them:

    cd src; make -f makefile.unix test

Unit tests for the GUI code are in `src/qt/test/`. To compile and run them:

    qmake POPCOIN_QT_TEST=1 -o Makefile.test popcoin-qt.pro
    make -f Makefile.test
    ./popcoin-qt_test
