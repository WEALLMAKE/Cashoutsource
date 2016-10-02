Copyright (c) 2016 cashout Developers

What is cashout?
----------------

CASHOUT SPECIFICATION


Algorithm   SHA256
Type   PoW
Abbreviation   CSH
Block reward   50 coins
Total coin supply   100000000 coins
Premine percent   20%
Premine amount   20000000 coins
Coinbase maturity   2 blocks
Target spacing   1 minutes
Target timespan   1000 minutes
Transaction confirmations   2 blocks

We are going to release the first version of the Cashout website for direct information about CASHOUT

From the website your a going to be able to download the wallet into the download section



Cashout is a new digital currency that enables instant payments to
anyone, anywhere in the world. cashout uses peer-to-peer technology to operate
with no central authority: managing transactions and issuing money are carried
out collectively by the network. cashout is also the name of the open source
software which enables the use of this currency.

For more information, as well as an immediately useable, binary version of
the cashout client software

License
-------

Cashout is released under the terms of the MIT license. See `COPYING` for more
information or see http://opensource.org/licenses/MIT.

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/cashout/cashout/tags) are created
regularly to indicate new official, stable release versions of cashout.

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

    qmake BITCOIN_QT_TEST=1 -o Makefile.test cashout-qt.pro
    make -f Makefile.test
    ./cashout-qt_test

Every pull request is built for both Windows and Linux on a dedicated server,
and unit and sanity tests are automatically run. The binaries produced may be
used for manual QA testing — a link to them will appear in a comment on the
pull request posted by [cashoutPullTester](https://github.com/cashoutPullTester). See https://github.com/TheBlueMatt/test-scripts
for the build/test scripts.

### Manual Quality Assurance (QA) Testing

Large changes should have a test plan, and should be tested by somebody other
than the developer who wrote the code.

See https://github.com/cashout/QA/ for how to create a test plan.
