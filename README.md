AlqCoin
=====================================

http://alquimista.webflow.io/

What is AlqCoin?
----------------

AlqCoin is a peer-to-peer Internet currency that enables instant, with almost non-existing cost payments to anyone around the world. AlqCoin is a completely open source, global payment network that is fully decentralized. Meaning there isn’t a central authority to dictate arbitrary limits. Our mathematical algorithms ensure the security of the network and allows any individual the freedom to control their own finances.


License
-------

AlqCoin is an open source software project released under the MIT/X11 license which gives you the power to run, modify, and copy the software and to distribute, at your option, modified copies of the software. The software is released in a transparent process that allows for independent verification of binaries and their corresponding source code. See [COPYING](COPYING) for more
information or see https://opensource.org/licenses/MIT.

Development Process
-------------------

The contribution workflow is described in [CONTRIBUTING.md](CONTRIBUTING.md).

Developer IRC can be found on Freenode at #AlqCoin-core-dev.

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test on short notice. Please be patient and help out by testing
other people's pull requests, and remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write [unit tests](src/test/README.md) for new code, and to
submit new unit tests for old code. Unit tests can be compiled and run
(assuming they weren't disabled in configure) with: `make check`. Further details on running
and extending unit tests can be found in [/src/test/README.md](/src/test/README.md).

There are also [regression and integration tests](/test), written
in Python, that are run automatically on the build server.
These tests can be run (if the [test dependencies](/test) are installed) with: `test/functional/test_runner.py`

The Travis CI system makes sure that every pull request is built for Windows, Linux, and OS X, and that unit/sanity tests are run automatically.

### Manual Quality Assurance (QA) Testing

Changes should be tested by somebody other than the developer who wrote the
code. This is especially important for large or high-risk changes. It is useful
to add a test plan to the pull request description if testing the changes is
not straightforward.
