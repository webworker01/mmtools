# mmtools
Bash CLI tools for MM2

Scripts in this repo work together as a whole, please follow the setup steps before usage.

The scripts in this repo are meant to be an educational and functional interaction with the mm2 API.  Each script contains in the beginning a link to the specific API call it is making so you can learn more details and create your own application to interact with the DEX.

* ![AtomicDex MM2 API Docs](https://developers.atomicdex.io/basic-docs/atomicdex/atomicdex-api.html)
* ![AtomicDex MM2 Repository](https://github.com/KomodoPlatform/atomicDEX-API)
* ![AtomicDex Desktop](https://github.com/KomodoPlatform/atomicDEX-Desktop) (if you don't want to use CLI)

![orderbook.png](./img/orderbook.png)

## Setup

```
cd ~
git clone https://github.com/webworker01/mmtools.git
cd ~/mmtools

#edit the config file with your wallet passphrase and rpc password
cp config.example config
nano config

#build atomicDEX-API
./init
```

After the build is complete start the marketmaker daemon

```
cd ~/mmtools
./start
```

In another window run:

```
cd ~/mmtools
./electrum rick
./electrum morty
```

Ready to go!

```
./orderbook rick morty
```
