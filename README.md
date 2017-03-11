================================================================
              Goshencoin integration/staging tree
================================================================


http://www.goshencoin.org

Copyright (c) 2009-2014 Bitcoin Developers
Copyright (c) 2011-2014 Litecoin Developers
Copyright (c) 2017 Goshencoin Developers

What is Goshencoin?
----------------

Goshen Project is a global initiative with the goal of adding value in unique ways, to all stakeholders. The GoshenCoin is a product of this initiative, and it is a decentralized peer-to-peer exchange system for communicating value among users. It is promoted by Eugene Nwoji, while Bitfawkes is the head of the development team.

The Goshen Project stands for Greater Good, Xcellence, and Prosperity (GXP)

Benefits

GoshenCoin is borne out of the desire to improve the quality of life to all. The Goshen Project, aside of its profit making activities, will strive to improve the lives of the less priviledged. By giving to different causes, direct involvement in empowerment of those who lack the basic means to provide for themselves. The collective Greater Good for all is paramount.

GoshenCoin cut out a class of its own with its delivery of innovative and excellent services. An infrastructure that facilitates long distance based transactions, at little or no cost, and easy conversion between virtual and fiat currencies. GoshenCoin is arguably the best cryptocurrency for remittances. Xcellence is built into the DNA of GoshenCoin.

At a time when everyone seeks a credible class that can guarantee steady and consistent returns, GoshenCoin steps in to fill the void. It is no more news that lots of investments made in conventional instruments do not turn out right, considering the persistent fall in value of regular currencies. With our well designed Price Stability Mechanism, you’re rest assured that GoshenCoin in your wallet today will be more valuable in the future. GoshenCoin is a store of value, and will continually appreciate in value as we witness greater adoption by by merchants, investors, and users. GoshenCoin is more than a coin, it is an Asset Class. Join us as we create value, great user experience, and Prosperity for all.

Goshencoin is a lite version of Bitcoin using scrypt as a proof-of-work algorithm.
 - 1 minute block targets
 - 1440 blocks to retarget difficulty
 - 50 coins per block
 - subsidy halves in 525k blocks (~1 years)
 - ~52 million total coins
 - 5 million premined coins

For more information, as well as an immediately useable, binary version of
the Goshencoin client sofware, see http://www.goshencoin.com.

License
-------

Goshencoin is released under the terms of the MIT license. See `COPYING` for more
information or see http://opensource.org/licenses/MIT.

Development process
-------------------

Developers work in their own trees, then submit pull requests when they think
their feature or bug fix is ready.

If it is a simple/trivial/non-controversial change, then one of the Goshencoin
development team members simply pulls it.

If it is a *more complicated or potentially controversial* change, then the patch
submitter will be asked to start a discussion with the devs and community.

The patch will be accepted if there is broad consensus that it is a good thing.
Developers should expect to rework and resubmit patches if the code doesn't
match the project's coding conventions (see `doc/coding.txt`) or are
controversial.

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/goshencoin-project/goshencoin/tags) are created
regularly to indicate new official, stable release versions of Goshencoin.

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test. Please be patient and help out, and
remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write unit tests for new code, and to
submit new unit tests for old code.

Unit tests for the core code are in `src/test/`. To compile and run them:

    cd src; make -f makefile.unix test

Unit tests for the GUI code are in `src/qt/test/`. To compile and run them:

    qmake BITCOIN_QT_TEST=1 -o Makefile.test bitcoin-qt.pro
    make -f Makefile.test
    ./goshencoin-qt_test

