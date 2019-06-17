# Non-Simulated Shared Ownership of scarce bitcoin with Multi Signatures in the Lightning Network

## Abstract

The universal axiom of scarcity is defined as the potential of conflict of control over a good. When Alice is utilzing a scarce good, Bob is excluded from using the same good at the same time but for a different task. Because of this fundamental rivelary over scarce goods, property rights emerge as a sound and logical structure to allocate resources throughout time. The binary opposite is a non-scarce good which is not restricted to individual control, it can be shared with whomever without the need of sacrifrice by the initial creator. Since non-scarce goods don`t need to be allocated througout time, property rights are neither necessary nor enforceable.

In Bitcoin, a unspent transaction output can only be spent when a previously committed script is computed as valid. Bitcoin script is exhaustive with several OP codes which can be constructed into smart contracts. The most basic script is a pay to single public key hash, where the proof of knowledge of one private key with a cryptographic signature returns valid and thus enables the transfer of bitcoin. Only with the knowledge of a non-scarce piece of information of the private key can the property rights of a scarce bitcoin be proven and enforced. Scripts can be constructed with OP_CHECKMULTISIG, where a coin can only be spent with m-of-n valid signatures. The Schnorr signature scheme can aggregate individual public keys and signatures for more efficient and secure multisig. Since a UTXO can only be spend with a threshold agreement between independent individuals, they have non-simulated shared ownership of scarce libre sound money.

The use case of multi signatures are far reaching, including strengthening the property right defense of a single individual with several separated keys, shared ownership of funds between likeminded peers, escrow security for ensuring honest trades, or as a basis for advanced scripts like paymentchannels in the lightning network or atomic swaps. 

## Structure

### PART I [On Scarcity](/Scarcity.asciidoc)

1. [Scarcity](/Scarcity.asciidoc#scarcity-1)
2. Private property
3. Mutually beneficial exchange
4. [Non-scarcity](/Scarcity.asciidoc#non-scarcity)
5. Open source libre software
6. Non-scarcity of Bitcoin and the scarcity of UTXOs

### PART II Shared Ownership

1. [Basics of Bitcoin Script](/Transaction.asciidoc)
2. [Script OP_CHECKMULTISIG](/ScriptMultisig.asciidoc)
3. [Schnorr aggregated MuSig](/SchnorrMuSig.asciidoc)
4. [Shamir's secret sharing](/ShamirsSecretSharing.asciidoc)
5. Schnorr threshold signatures

### PART III [Use Cases](/UseCase.asciidoc)

1. [1-of-2 Joint Spending](/UseCase.asciidoc#1-of-2-joint-spending)
2. [2-of-2 Joint Saving](/UseCase.asciidoc#2-of-2-joint-saving)
3. [2-of-2 Two-Factor Authentication](/UseCase.asciidoc#2-of-2-two-factor-authentication)
4. [2-of-2 Smart Contract Building Block](/UseCase.asciidoc#2-of-2-smart-bontract-building-block)
5. [2-of-3 Child Saving](/UseCase.asciidoc#2-of-3-child-saving)
6. [2-of-3 Buyer, Seller, Trust less Escrow](/UseCase.asciidoc#2-of-3-buyer-seller-trust-less-escrow)
7. [2-of-3 Hot Wallet Security](/UseCase.asciidoc#2-of-3-hot-wallet-security)
8. [3-of-5 Low Trust Joint Funds](/UseCase.asciidoc#3-of-5-lowtrust-joint-funds)
9. [2-of-2 lightning network payment channel](/PaymentChannel.asciidoc)
10. n-of-n lightning network channel factories
11. m-of-n lightning network individual payment

## License and Contribution

This Bachelor's thesis is written in an open source process, and published under the [Creative Commons Attribution-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by/4.0/legalcode). If you'd like to contribute to the research and writing, please submit an issue or fork the repository, commit the changes on your own branch, and issue a pull request. I have 1001 questions and thank all the peers whom I can bother to ask. If you have a proposal, feedback or question, don't hesitate to [reach out](https://towardsliberty.com/contact)! Thank you very much for your support!

The thesis is due on July 1st 2019 and written under the direction of [Prof. Dr. Bernd Kaltenhaeuser](https://www.dhbw-vs.de/hochschule/mitarbeitende/bernd-kaltenhaeuser.html). It will be published for peer review in the Libertarians Schollars Conference.

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

If you think that this research paper is of importance to you, your project and the Bitcoin network in general, please consider supporting this project. Mainly, contemplate the problem and share your ideas on how a solution can be implemented. If you know someone who is interested in this subject, feel free to [share the link](https://github.com/MaxHillebrand/LightningMultiSig/) and all the information contained in the repository. If you'd like to give financial support, I very much appreciate every Satoshi you can spare to [donate](https://tallyco.in/HillebrandMax)!

3GB2fALwyWpcBY98svyDfX6fVQp4rNfoQ5
