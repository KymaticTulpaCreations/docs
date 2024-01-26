# JSON-RPC Endpoint

## Available Resources

### Mainnet(ChainID 0x3C46, 15430 in decimal)

NCRPC Endpoints:

!!! NOTE
	You can make `eth_getLogs` requests with up to a 5K block range.
	If you need to pull logs frequently, we recommend using WebSockets to push new logs to you when they are available.

Recommend

* https://nc-dataseed.kymaticscan.online/


NCWebsocket Endpoints:

*Note: provided by community with no quality promised, building your node should be always the long term goal*

* wss://nc-ws-node.kymaticscan.online:443


### Rate limit

The rate limit of KYMATIC endpoint on Testnet and Mainnet is 10K/5min.


## Start

You can start the HTTP JSON-RPC with the --rpc flag
```bash
## mainnet
geth attach https://mainnet-rpc.kymaticscan.online

## testnet
geth attach https://testnet-rpc.kymaticscan.online/
```

## JSON-RPC methods

Please refer to this [wiki page](https://github.com/ethereum/wiki/wiki/JSON-RPC) or use Postman: <https://documenter.getpostman.com/view/4117254/ethereum-json-rpc/RVu7CT5J?version=latest>
