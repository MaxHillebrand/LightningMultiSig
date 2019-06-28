# Non-Simulated Shared Ownership of scarce bitcoin with Multi Signatures in the Lightning Network

## Abstract

The universal axiom of scarcity is defined as the potential of conflict of control over a good. When Alice is utilizing a scarce good, Bob is excluded from using the same good at the same time but for a different task. Because of this fundamental rivalry over scarce goods, property rights emerge as a sound and logical structure to allocate resources throughout time. The binary opposite is a non-scarce good which is not restricted to individual control; it can be shared with whomever, without the need of sacrifice by the initial creator. Since non-scarce goods don't need to be allocated throughout time, property rights are neither necessary nor enforceable.

In Bitcoin, an unspent transaction output can only be spent when a previously-committed script is computed as valid. Bitcoin script is exhaustive with several `opcodes` which can be constructed into smart contracts. The most basic script is a `pay-to-single public key hash [P2PKH]`, where the knowledge of one private belonging to the address, the intent to transfer bitcoins to particular set of outputs and integrity of said intent proven with a cryptographic signature returns valid, and thus enables the transfer of bitcoin. Only with the knowledge of a non-scarce piece of information of the private key can the property rights of a scarce bitcoin be proven and enforced. Scripts can be constructed with `OP_CHECKMULTISIG`, where a coin can only be spent with m-of-n valid signatures. The Schnorr signature scheme can aggregate individual public keys and signatures for a more efficient and secure multisig implementation. Since a `UTXO` can only be spent within a threshold agreement between independent individuals, they have non-simulated shared ownership of scarce libre sound money.

The use cases of multi signatures are far reaching, including strengthening the property right defence of a single individual with several separated keys, shared ownership of funds between like-minded peers, escrow security for ensuring honest trades, or as a basis for advanced scripts like `paymentchannels` in the lightning network or atomic swaps. 

## Structure

### PART I [On Scarcity](/Scarcity.asciidoc)

1. [Human Action](/Scarceity.asciidoc#human-action)
2. [Exclusivity of Scarce Goods](/Scarceity.asciidoc#exclusivity-of-scarce-goods)
3. [Rarity of Scarce Goods](/Scarceity.asciidoc#rarity-of-scarce-goods)
4. [Liberty](/Scarcity.asciidoc#liberty)<br/>
   4.1 [Private property](/Scarcity.asciidoc#private-property)<br/>
   4.2 [Homesteading](/Scarcity.asciidoc#homesteading)<br/>
   4.3 [Mutually beneficial exchange](/Scarcity.asciidoc#mutually-beneficial-exchange)
5. [Slavery](/Scarcity.asciidoc#slavery)<br/>
   5.1 [Autistic Intervention](/Scarcity.asciidoc#autistic-intervention)<br/>
   5.2 [Binary Intervention](/Scarcity.asciidoc#binary-intervention)<br/>
   5.3 [Triangular Intervention](/Scarcity.asciidoc#triangular-intervention)
6. [Communism](/Scarcity.asciidoc#communism)
7. [Non-scarcity](/Scarcity.asciidoc#non-scarcity)
8. [Libre Open Source Software](/Scarcity.asciidoc#libre-open-source-software)
9. [Fallacy of Intellectual Property](/Scarcity.asciidoc#fallacy-of-intellectual-property)
10. [Non-scarcity of Cryptography](/Scarcity.asciidoc#non-scarcity-of-cryptography)
11. [Scarcity of UTXOs](/Scarcity.asciidoc#scarcity-of-utxos)<br/>
    11.1 [Double Spending is Non-Scarcity](/Scarcity.asciidoc#double-spending-is-non-scarcity)<br/>
    11.2 [Bitcoin Halving and Scarcity](/Scarcity.asciidoc#bitcoin-halving-and-scarcity)<br/>
    11.3 [Full Nodes Define, Verify and Enforce Scarcity](/Scarcity.asciidoc#full-nodes-define,-verify-and-enforce-scarcity)

### PART II [Shared Ownership](/SharedOwnership.asciidoc)

1. [Basics of Bitcoin Script](/SharedOwnership.asciidoc/basics-of-bitcoin-script)<br/>
   1.1 [Pay to Public Key Hash](SharedOwnership.asciidoc#pay-to-public-key-hash)<br/>
   1.2 [Pay to Script Hash](/SharedOwnership.asciidoc#pay-to-script-hash)<br/>
   1.3 [Pay to Witness Public Key Hash](/SharedOwnership.asciidoc#pay-to-witness-public-key-hash)<br/>
   1.4 [Pay to Witness Script Hash](/SharedOwnership.asciidoc#pay-to-witness-script-hash)
2. [Script OP_CHECKMULTISIG](/SharedOwnership.asciidoc#script-multi-signatures)
3. [Schnorr aggregated MuSig](/SharedOwnership.asciidoc#schnorr-signatures)
4. [Taproot](/SharedOwnership.asciidoc#taproot)
5. [Shamir's secret sharing](/SharedOwnership.asciidoc#shamir’s-secret-sharing-scheme)
6. [Schnorr threshold signatures](/SharedOwnership.asciidoc#schnorr-threshold-signatures)
7. [Lightning Network](/SharedOwnership.asciidoc#lightning-network)<br/>
   7.1 [2-of-2 lightning network payment channel](/SharedOwnership.asciidoc#2-of-2-lightning-network-payment-channel)<br/>
   7.2 [n-of-n lightning network channel factories](/SharedOwnership.asciidoc#n-of-n-multi-party-channel-factories)

### PART III [Use Cases](/UseCase.asciidoc)

1. [1-of-2 Joint Spending](/UseCase.asciidoc#1-of-2-joint-spending)
2. [2-of-2 Joint Saving](/UseCase.asciidoc#2-of-2-joint-saving)
3. [2-of-2 Two-Factor Authentication](/UseCase.asciidoc#2-of-2-two-factor-authentication)
4. [2-of-3 Child Saving](/UseCase.asciidoc#2-of-3-child-saving)
5. [2-of-3 Buyer, Seller, Trust less Escrow](/UseCase.asciidoc#2-of-3-buyer-seller-trust-less-escrow)
6. [2-of-3 Hot Wallet Security](/UseCase.asciidoc#2-of-3-hot-wallet-security)
7. [3-of-5 Low Trust Joint Funds](/UseCase.asciidoc#3-of-5-lowtrust-joint-funds)
8. [Transaction Output Commitments](/UseCase.asciidoc#transaction-output-commitments)

## License and Contribution

This Bachelor's thesis is written in an open source process, and published under the [Creative Commons Attribution-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by/4.0/legalcode). If you'd like to contribute to the research and writing, please submit an issue or fork the repository, commit the changes on your own branch, and issue a pull request. I have 1001 questions and thank all the peers whom I can bother to ask. If you have a proposal, feedback or question, don't hesitate to [reach out](https://towardsliberty.com/contact)! Thank you very much for your support!

The thesis is due on July 1st 2019 and written under the direction of [Prof. Dr. Bernd Kaltenhaeuser](https://www.dhbw-vs.de/hochschule/mitarbeitende/bernd-kaltenhaeuser.html). The [Declaration of Honor](/DeclarationOfHonor.asciidoc) is signed here. It will be published for peer review in the Libertarians Scholars Conference.

## Support

If you think that this research paper is of importance to you, your project and the Bitcoin network in general, please consider supporting this project. Mainly, contemplate the problem and share your ideas on how a solution can be implemented. If you know someone who is interested in this subject, feel free to [share the link](https://github.com/MaxHillebrand/LightningMultiSig/) and all the information contained in the repository. If you'd like to give financial support, I very much appreciate every Satoshi you can spare to [donate](https://tallyco.in/HillebrandMax)!

3GB2fALwyWpcBY98svyDfX6fVQp4rNfoQ5
