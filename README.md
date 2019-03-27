# Non-Simulated Shared Ownership of bitcoin with Multi Signatures in the Lightning Network

## Abstract

The universal axiom of scarcity is defined as the potential of conflict of control over a good. Either Alice, or Bob can hold and use a gold coin, there is no possibility that both at the same time have full deposal over it. Because of this fundamental scarcity, property rights emerge as a sound and logical structure to allocate resources throughout time. There are however non-scarce goods which are not restricted to individual control and use. Like ideas, music or speech, these libre goods can be shared with whomever without the need of sacrifice by the initial creator. The poet still knows his poem after he has performed it on stage, yet the audience has gained the knowledge conveyed. Thus there is no need for property rights and ownership in the realm of ideas and mind.

In Bitcoin, a unspent transaction output can only be spent when a previously committed script is computed as valid. Although the Bitcoin script is not Turing complete, it is exhaustive with several OP codes which can be constructed into smart contracts. The most basic script is a pay to single public key hash, where the proof of knowledge of one private key with a cryptographic signature returns valid and thus enables the transfer of bitcoin to another commitment script. Only with the knowledge of a non-scarce piece of information, can the property rights of a scarce bitcoin be proven and enforced. One of the most commonly used OP codes is CHECKMULTISIG, where a coin can only be spent with m-of-n valid signatures. This allows for non-simulated shared ownership of libre sound money, which is a groundbreaking innovation with vast consequences.

This thesis explains the universal divide between scarce and non-scarce goods; the emergence and importance of private property and the the public commons; the novel invention of non-simulated shared ownership of bitcoin; the basics of Bitcoin script; how multi sig is used on the first layer block chain; and the basics of lightning network and it's use of multi sig. The novel research of this thesis is to suggests how different types of multi sig payment channel can be constructed, updated and closed; how multi sig access rights to a lightning node might work; and estimates weather such a multi sig payment channel is useful for liquidity routing. Concluding with different use cases and business models possible with lightning multi sig.

## Structure

### PART I [On Scarcity](/Scarcity.asciidoc)

1. Scarcity
2. Private property
3. Mutually beneficial exchange
4. Non-scarcity
5. Open source libre software
6. Non-simulated shared ownership of bitcoin

### PART II [On-chain Transactions](/Transaction.asciidoc)

1. Pay to public key hash P2PKH [lecagcy and segwit]
2. Pay to script hash P2SH [lecagcy and segwit]
3. M-of-n Multi Signature on chain

### PART III [Lightning Network Basics](/PaymentChannel.asciidoc)

1. Funding transaction
2. Commitment transaction
3. Closing transaction
4. [Routing](/Routing.asciidoc)

### PART IV [Lightning Network Multi Sig](/LightningMultiSigTransaction.asciidoc)

1. M-of-n key aggregation on top of a regular 2-of-2 lightning payment channel
2. Commitment transaction redeem script `m-of-n + 1`
3. M-of-n access rights to node with 2-of-2 payment channels via macaroons, RPC, ...
4. Hindering the pre image release of a 2-of-2 payment channel route with a m-of-n unlock script

### PART V [Use Cases](/UseCase.asciidoc)

1. Single party multi sig
    
    1.1.  n-of-n Second Factor Authentication
    
    1.2.  m-of-n Second Factor Authentication

2. Multi Party Multi Signatures
    
    2.1.  Group Fund Management
    
    2.2.  Escrow
    
    2.3.  Vault

## License and Contribution

This Bachelor's thesis is written in an open source process, and published under the [Creative Commons Attribution-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by/4.0/legalcode). If you'd like to contribute to the research and writing, please submit an issue or fork the repository, commit the changes on your own branch, and issue a pull request. I have 1001 questions and thank all the peers whom I can bother to ask. If you have a proposal, feedback or question, don't hesitate to [reach out](https://towardsliberty.com/contact)! Thank you very much for your support!

The thesis is due on July 1st 2019 and written under the direction of [Prof. Dr. Bernd Kaltenhaeuser](https://www.dhbw-vs.de/hochschule/mitarbeitende/bernd-kaltenhaeuser.html).

## Possible Approaches

I have no clue how to best do this. As far as I know, there is no proposal or implementation in existence yet. However, there are several approaches that might lead to the desired outcome and evolve into a suitable solution. All this is very much subject to change, new approaches will be discovered, and wrong ideas discarded. See the [Research file](/Research.asciidoc) for prerequisite work.

* M-of-n key aggregation on top of a regular 2-of-2 lightning payment channel
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
* Option 5: split `revocation_basepoint_secret` into m-of-n, with 2-of-2 payment channel
* [Usecases of multi signature both on- and off-chain](/UseCase.asciidoc)
* Punishment mechanism and game theory

## Support

If you think that this research paper is of importance to you, your company and the Bitcoin network in general, please consider supporting this project. Mainly, contemplate the problem and share your ideas on how a solution can be implemented. If you know someone who is interested in this subject, feel free to [share the link](https://github.com/MaxHillebrand/LightningMultiSig/) and all the information contained in the repository. If you'd like to give financial support, I'd very much appreciate every Satoshi you can spare to [donate](https://tallyco.in/HillebrandMax)!

3GB2fALwyWpcBY98svyDfX6fVQp4rNfoQ5