# Inspect and regeneratate BIP39 binary data

Work in progress, a tool for converting any BIP39 mnemonic seed phrase to binary constitutes for the sake of binary backup of the seed.

## Online Version

https://huge.github.io/bip39/src/#notCompleteYet

## Standalone offline version

Download `bip39-standalone.html` from
[the releases](https://github.com/huge/bip39/releases). Seems a reasonable hosting/repository. sha and keybase underwriting would be good( #todo)

Open the file in a web browser. Use for your prosperity.

To created this final html file from source use the command `python compile.py` while in your local clone/copy of this repo.

## Usage

Enter your BIP39 phrase into the 'BIP39 Phrase' field
  should be largest UI element,..front.

'Generate Random Phrase' button just a tiny bit for "testing out"..

## Donations

Shamelessly wellcome BTCs at 
bc1q7tlnxywmefzn2qnuefarqrzmuj3v2545u2t3nx 

or XMR 4AeUXDQ1NWVArPPp8paMkxHRcXSB48QpnUHKDUmqZW9b88Z5TNjG6XA6bJX4SwXHd15PrR7RUPg1YV9aYshY1EJzJg7rEAE 

## Making changes

Make changes in `src/*`.

Changes are applied for a release using the command `python compile.py`.

# Tests

Tests depend on

* nodejs
* selenium webdriver - cd /path/to/bip39/tests; npm install
* selenium driver for firefox ([geckodriver](https://github.com/mozilla/geckodriver/releases)) and / or chrome ([chromedriver](https://sites.google.com/a/chromium.org/chromedriver/downloads))
* jasmine - npm install --global jasmine

Before running tests, the site must be served at http://localhost:8000.

```
$ cd /path/to/bip39/src
$ python -m http.server

or for python2
$ python -m SimpleHTTPServer
```

Run tests from the command-line

```
$ cd /path/to/bip39/tests
$ jasmine spec/tests.js
```

# License

This BIP39 tool is released under the terms of the MIT license. See LICENSE for
more information or see https://opensource.org/licenses/MIT.
