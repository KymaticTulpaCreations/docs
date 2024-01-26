# How to Run A Fullnode on Kymatic Chain

## Fullnodes Functions

* Stores the full blockchain history on disk and can answer the data request from the network.
* Receives and validates the new blocks and transactions.
* Verifies the states of every accounts.

## Supported Platforms

We support running a full node on `Mac OS X`and `Linux`.

## Suggested Requirements

### Fullnode
- VPS running recent versions of Mac OS X or Linux.
- 4 cores of CPU and 8 gigabytes of memory (RAM).
- A broadband Internet connection with upload/download speeds of 5 megabyte per second


## Steps to Run a Full Node

Download  kymatic_mainnet.json, config.toml and file geth from  https://github.com/KymaticTulpaCreations/KymaticNetwork

```
wget  https://raw.githubusercontent.com/KymaticTulpaCreations/KymaticNetwork/master/kymatic_mainnet.json
wget https://raw.githubusercontent.com/KymaticTulpaCreations/KymaticNetwork/master/config.toml
wget https://raw.githubusercontent.com/KymaticTulpaCreations/KymaticNetwork/master/geth

```

Make node folder

```
mkdir node
```

Initialize the Node
```
./geth --datadir ./node init kymatic_mainnet.json

```

Run the Nodes

```
./geth --datadir node -snapshot=false --gcmode=archive --config config.toml --allow-insecure-unlock --cache=1024

```
