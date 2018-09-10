

### Public keys as identities
This article began with the understanding that a secure ledger makes creating digital currency straightforward. 

Let’s revisit this claim. 

When Alice wishes to pay Bob, she broadcasts the transaction to all bitcoin nodes. 

A transaction is simply a string: a statement encoding Alice’s wish to pay Bob some value, signed by her. 

The eventual inclusion of this signed statement into the ledger by miners is what makes the transaction real. 

Note that this doesn’t require Bob’s participation in any way. 

But let’s focus on what’s not in the transaction: conspicuously absent are Alice and Bob’s identities; instead, the transaction contains only their respective public keys. 

This is an important concept in bitcoin: public keys are the only kinds of identities in the system. Transactions transfer value from and to public keys, which are called addresses.
In order to “speak for” an identity, you must know the corresponding secret key. You can create a new identity at any time by generating a new key pair, with no central authority or registry. You don’t need to obtain a user name or inform others that you have picked a particular name. This is the notion of decentralized identity management. Bitcoin doesn’t specify how Alice tells Bob what her pseudonym is—that is external to the system. 
Although radically different from most other payment systems today, these ideas are quite old, dating back to David Chaum, the father of digital cash. In fact, Chaum also made seminal contributions to anonymity networks, and it is in this context that he invented this idea. In his 1981 paper, “Untraceable Electronic Mail, Return Addresses, and Digital Pseudonyms,”9 he states: “A digital ‘pseudonym’ is a public key used to verify signatures made by the anonymous holder of the corresponding private key.” 
Now, having message recipients be known only by a public key presents an obvious problem: there is no way to route the message to the right computer. This leads to a massive inefficiency in Chaum’s proposal, which can be traded off against the level of anonymity but not eliminated. Bitcoin is similarly exceedingly inefficient compared with centralized payment systems: the ledger containing every transaction is maintained by every node in the system. Bitcoin incurs this inefficiency for security reasons anyway, and thus achieves pseudonymity (i.e, public keys as identities) “for free.” Chaum took these ideas much further in a 1985 paper,11 where he presents a vision of privacy-preserving e-commerce based on pervasive pseudonyms, as well as “blind signatures,” the key technical idea behind his digital cash.
The public-keys-as-identities idea is also seen in b-money and bit gold, the two precursor essays to bitcoin discussed earlier. However, much of the work that built on Chaum’s foundation, as well as Chaum’s own later work on ecash, moved away from this idea. The cypherpunks were keenly interested in privacy-preserving communication and commerce, and they embraced pseudonyms, which they called nyms. But to them, nyms weren’t mere cryptographic identities (i.e., public keys), but rather, usually email addresses that were linked to public keys. Similarly, Ian Goldberg’s dissertation, which became the basis of much future work on anonymous communication, recognizes Chaum’s idea but suggests that nyms should be human-memorable nicknames with certificates to bind them.20 Thus Bitcoin proved to be the most successful instantiation of Chaum’s idea. 
