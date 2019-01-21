# Lightning Multi Signatures

## Abstract

In Bitcoin, a UTXO can only be spent when a previously commited script is computed as valid. Although the Bitcoin script is not Turing copmlete, it is exhaustive with several OP codes which can be constructed into smart contracts. The most basic script is a pay to single public key hash, where the proof of knowledge of one private key with a cryptographic signature over the hash of the transaction data returns valid and thus enables the transafer of bitcoin to another commitment script. One of the most commonly used OP codes is CHECKMULTISIG, where a coin can only be spent with m-of-n valid signatures. This allows for easy and secure co-control of bitcoin, which is useful in several business ventures and security models.

This thesis explains how multi sig is used on the first layer block chain; how lightning network payment channel use 2-of-2 time locked multi sig; suggests how different types of multi sig payment channel can be constructed, updated and closed; explores how multi sig access rights to a lightning node might work; estimates weather such a multi sig payment channel is useful for liquidity routing; and proposes different use cases and business models possible with lightning multi sig.

## License and Contribution

The paper is written in an open source process, and published under the [Creative Commons Attribution-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by/4.0/legalcode). If you'd like to contribute to the research and writing, please submit an issue, fork the repository, commit the changes on your own branch, and issue a pull request when you're satisfied with your work. I have 1001 questions and thank all the peers whom I can bather to ask them. If you have a proposal, feedback or question, don't hesitate to [reach out](/https://towardsliberty.com/contact)! Thank you very much for your support!

## Possible Approaches

I have no clue how to best do this. As far as I know, there is no proposal or implementation in existense yet. However, there are several approaches that might lead to the desired outcome and evolve into a suitable solution. All this is very much subject to change, new approaches will be discovered, and wrong ideas discarted. See the [Research file](/Research.asciidoc) for prerequisite work. 

* M-of-n key aggregation ontop of a regular 2-of-2 lightning payment channel
* Commitment transaction redeem script `m-of-n + 1`
* M-of-n access rights to node with 2-of-2 payment channels via macaroons, RPC, ...
* Hindering the pre image release of a 2-of-2 payment channel route with a m-of-n unlock script

## ToDo

This thesis is in the early stages of research and writing, there are many topics that require further insight and clear explanation. Here is a list of rough ToDo's with links to the working files.

* [Different type of transactions [P2PKH, P2SH, P2WPKH, P2WSH] including on chain multisig](/Transaction.asciidoc)
* [Funding, Commitment, Revocation and Closing Transaction of Payment Channel](/PaymentChannel.asciidoc)
* [HTLC and Routing](/Routing.asciidoc)
* [Option 1: m-of-n + 1 commitment transaction](/LightningMultiSigTransaction.asciidoc)
* [Option 2: 2-of-2 + with Shamir's secret sharing or aggregated ECDSA/Schnorr](/LightningMultiSigTransaction.asciidoc)
* Option 3: m-of-n access rights to node with 2-of-2 payment channel
* Option 4: Preimage locked with m-of-n
* [Usecases of multi signature both on- and off-chain](/UseCase.asciidoc)
* Punishment mechanism and game theory