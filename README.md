# Lightning Multi Signatures

## Abstract

In Bitcoin, a UTXO can only be spent when a previously commited script is computed as valid. Although the Bitcoin script is not Turing copmlete, it is exhaustive with several OP codes which can be constructed into smart contracts. The most basic script is a single signature, where the proof of knowledge of a single private key with a cryptographic signature over the hash of the transaction data returns valid and thus enables the transafer of bitcoin to another commitment script. One of the most commonly used is OP_CHECKMULTISIG, where a coin can only be spent with m-of-n valid signatures. This allows for easy and secure co-ownership of bitcoin, which is useful in several business ventures and security models.

This thesis explains how multi sig is used on the first layer block chain; how lightning network payment channel use 2-of-2 time locked multi sig; suggests how m-of-n+1 multi sig payment channel can be constructed, updated and closed; estimates weather such a multi sig payment channel is useful for liquidity routing; and proposes different business models of lightning multi sig.

The paper is written in an open source process, and published under the [Creative Commons Attribution-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by/4.0/legalcode). If you'd like to contribute to the research and writing, please submit an issue, fork the repository, commit the changes on your own branch, and issue a pull request when you're satisfied with your work. Thank you for your support!

## ToDo

This thesis is in the early stages of research and writing, there are many topics that require further insight and clear explanation. Here is a list of rough ToDo's and the process plus notes to them.

* [Different type of transactions [P2PKH, P2SH, P2WPKH, P2WSH] including on chain multisig](/Transaction.asciidoc)
* [Funding, Commitment, Revocation and Closing Transaction of Payment Channel](/PaymentChannel.asciidoc)
* [HTLC and Routing](/Routing.asciidoc)
* [Possible Option 1: m-of-n + 1 commitment transaction](/LightningMultiSigTransaction.asciidoc)
* [Possible Option 2: 2-of-2 + with Shamir's secret sharing or aggregated Schnorr [likely nonsensical]](/LightningMultiSigTransaction.asciidoc)
* Usecases of multi signature both on- and off-chain