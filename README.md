dero-escrow is a work in progress to make escrow services private

As this is desc is my first smart contract, I will need to lean heavily on the work of Capt DERO and the documentation that he wrote here: https://github.com/deroproject/documentation. Specifically, I believe that his documentation on an asset exchange service will be key. 

TO-DO
---
- [ ] Test SC in testnet
- [ ] Deploy SC to mainnet

In-Progress
---
- [\] Study DVMDOCS & document findings

# DVMDOCS/examples/assetexchange
## asset_exchange.bas
This is a .bas file, or a BASIC file.

It begins with stating it has a "Function" and that is to " Deposit()". As istated in the DVMDOCS/statementsDVM.md, any uppercase function, ie Deposit(), can be used by any other smart contract externally, eg DERO at large, and any lowercase function can only be used by the smart contract internally.

What is to be deposited is defined by "Uint64". Uint means unsigned integer, or non-negative whole numbers.

It supposes that there is an owner of the contract.
"

It also supposes that there is a signer. shows that a person could deposit an arbitrary number of some asset and be given the another asset at a half ratio.

There are some additional modifiers to the code which would aide the contract owner.

- [ ] Write desc

DONE
---
- [x] Make github repo

