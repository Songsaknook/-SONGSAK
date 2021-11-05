#https://github.com/21-twenty-one/21/security/advisories
# Trezor Connect API version 8.1.30-beta.2


Trezor Connect is a platform for easy integration of Trezor into 3rd party services. It provides API with functionality to access public keys, sign transactions and authenticate users. User interface is presented in a secure popup window served from `https://connect.trezor.io/8/popup.html`

* [Integration](docs/index.md)
* [Development](https://wiki.trezor.io/Developers_guide:Trezor_Connect_API)


## Versions
We started tagging versions and releasing them to separate URLs, so we don't break any existing (and working) integrations.

Currently, we are at version 8, which has an url https://connect.trezor.io/8/trezor-connect.js. If you would like to find out which version is deployed precisely simply run:

`curl -s https://connect.trezor.io/8/trezor-connect.js | grep VERSION`

With regards to this repo - All updates should go to current version branch, the previous releases are in corresponding branches. The gh-pages is the same older version, that is used at trezor.github.io/connect/connect.js, and it's there for backwards compatibility; please don't touch.

## Tests
For integration testing against trezord and emulator refer to [this document](./tests/README.md).
