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

Next the there is "20", which upon looking deeper into the contract, it appears that 20 is used to denote that a "RETURN" is in about to be defined. The same is true of "40", and conversely all odds (eg 10, 30, 50, etc), are modifiers. 

We see that "RETURN" has a value of "0", from the statementsDVM.md we learn that " Any entrypoint which returns uint64 value 0 is termed as success and will make transaction to commit all state changes." Which means that if "Function Deposit() Uint64" has happened, the DVM will return to the 0 position. 

There seems to be two things that we need to keep in mind with Functions. The first is that "Function may or may not have a return type." (we haven't seen an example in the contract thus far that looksl like "Function function_name( 0 or more arguments ) return type". And the second thing that we have to keep in mind is that "All functions must use RETURN to return from function or to return a value. RETURN is mandatory."

After that we see that there is an End Function to the "Function Deposit() Uint64". What we take this to mean is that the function is over. Pretty self-explanatory there. 

So I am going to take this feature and I am going to copy it to the desc.

It supposes that there is an owner of the contract.
"

It also supposes that there is a signer. shows that a person could deposit an arbitrary number of some asset and be given the another asset at a half ratio.

There are some additional modifiers to the code which would aide the contract owner.

- [ ] Write desc

DONE
---
- [x] Make github repo

