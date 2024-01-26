# Cross-chain Communication

## How much is cross-chain transfer fee?

The total cost of transfer from BC to KYMATIC is composed of 2 parts:

* Fee for executing `bridge transfer-out` transaction is 0.004KYMATIC,  pay validators on Kymatic Chain

* Fee for KYMATIC-relayers 0.004KYMATIC. it will cover the fees of calling TokenHub Contract on KYMATIC.

The total cost of transfer from KYMATIC to BC is composed of 2 parts:

* Fee for Oracle-relayers 0.004KYMATIC, pay for KYMATIC relayers

* Call TokenHub Contract: You need to pay KYMATIC for calling smart-contract on KYMATIC, this transaction is metered by gas, which is a global parameter. At the moment, you need to pay about 0.0005KYMATIC ~ 0.0015KYMATIC.

## What's is a KYMATIC relayer?

NCrelayer monitors cross chain packages on Kymatic Chain, builds and broadcasts transactions to KYMATIC to deliver these packages, which is the key of cross chain communication from Kymatic Chain to KYMATIC.

## What's is an Oracle relayer?

Oracle Relayer watches the state change of Kymatic Chain. Once it catches Cross-Chain Communication Events, it will submit to vote for the requests. After Oracle Relayers from ⅔ of the voting power of BC validators vote for the changes, the cross-chain actions will be performed. Only validators of Kymatic Chain are eligible to run Oracle relayers.

## What's an oracle?

In blockchain network, an oracle refers to the element that connects smart contracts with data from the outside world. In the network of Kymatic Chain, the execution of the transanction wil emit Events, and such events can be packaged and relayed onto BC. In this way, BC will get updates about changes of KYMATIC.

## Which wallet support cross-chain transfer?

You need to use [MyEtherWallet](../../smart-chain/wallet/myetherwallet.md) to call contracts and use Kymatic Chain commandline client: `eth-cli`/ `eth-cli` for complementary commands

Please refer to this [guide](../../smart-chain/developer/cross-chain-transfer.md) for details

## How to send cross-chain transfer?

You can use [Kymatic Chain extension wallet](../../smart-chain/wallet/shree.md) or

use [Trust wallet](https://community.trustwallet.com/t/how-to-send-and-receive-kymatic-on-smart-chain/67430)