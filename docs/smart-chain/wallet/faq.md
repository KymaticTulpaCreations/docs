# KYMATIC Extension Wallet FAQ
## Tokens not visible after withdrawing from KYMATIC


Many users who interact with a centralized exchange like KYMATIC eventually want to withdraw to a wallet that they fully control, like MetaMask. So once you've used their withdraw form, what could be scarier than not seeing your tokens?

First, you'll need to use the MetaMask add Custom Network feature to add the Kymatic Chain or Kymatic Chain's RPC URLs endpoints to your MetaMask.

Once you've added the Kymatic Chain or the Kymatic Chain to your MetaMask, you will be able to select different networks to view the assets (you may need to add Custom Tokens too) held by your selected account on that network.


## How Much KYMATIC You Need To Send Tokens

if you try to send tokens without having any KYMATIC in your account you will be told you have insufficient funds. This means you do not have enough KYMATIC in your account to cover the cost of gas. Each transaction (including token and contract transactions) require gas and that gas is paid in KYMATIC. You can think of this like a transaction fee.

You can remedy this by sending 0.001 KYMATIC to that account in order to be able to make the transaction.

A standard Ether transfer TX will be 21000 gas & a gas price of 15 Gwei.
With tokens, the amount of gas is typically  gas, so the total TX fee increases to 0.002 KYMATIC - 0.003 KYMATIC.


## Current Gas Price

```
curl --location --request POST 'https://nc-dataseed2.kymaticscan.online' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc":"2.0", "id":1, "method":"eth_gasPrice", "params": []}'
```