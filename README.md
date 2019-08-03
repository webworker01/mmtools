# mmtools
Bash CLI tools for MM2

Follow these instructions for initial setup:
https://developers.atomicdex.io/basic-docs/atomicdex/atomicdex-setup/get-started-atomicdex.html

Clone this repo

```
cd ~
git clone https://github.com/webworker01/mmtools.git
cd ~/mmtools
git submodule update --init --recursive
cp config.example config
```

Now edit the config file with your wallet passphrase and rpc password

```
cd ~/mmtools
./start
```

In another window run:

```
cd ~/mmtools
./enable RICK
./enable MORTY
```

Ready to go!

```
./checkorderbooks rick morty
```
