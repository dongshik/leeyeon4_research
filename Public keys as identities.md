### Public keys as identities

This article began with the understanding that a secure ledger makes creating digital currency straightforward. 

Let’s revisit this claim. 

When Alice wishes to pay Bob, she broadcasts the transaction to all bitcoin nodes. 

A transaction is simply a string: a statement encoding Alice’s wish to pay Bob some value, signed by her. 

The eventual inclusion of this signed statement into the ledger by miners is what makes the transaction real. 

Note that this doesn’t require Bob’s participation in any way. 

But let’s focus on what’s not in the transaction: conspicuously absent are Alice and Bob’s identities; instead, the transaction contains only their respective public keys. 
그러나 transaction에 없는 것에 초점을 맞춰보면, 분명히 앨리스와 밥의 신원증명(identities)은 없습니다. 대신 트랜잭션에는 각각의 공개 키만 포함됩니다.

This is an important concept in bitcoin: public keys are the only kinds of identities in the system. 
이것은 비트코인(bitcoin)의 중요한 개념(concept)입니다. 공개키는 시스템의 유일한 신원증명입니다.

Transactions transfer value from and to public keys, which are called addresses.
트랜잭션(transaction)은 주소(address)라고 부르는 공개키들간에 값을 전달합니다.

In order to “speak for” an identity, you must know the corresponding secret key. 
신원증명에 대해 "말하기" 위해서 상응하는 비밀키(secret key)를 알아야 합니다.

You can create a new identity at any time by generating a new key pair, with no central authority or registry. 
중앙 권한이나 등재(등록)없이 새로운 키쌍을 생성함으로서 언제든지 새로운 신원증명을 생성 할 수 있습니다

You don’t need to obtain a user name or inform others that you have picked a particular name. 
사용자이름을 얻가나 특정 이름을 선택했다고 다른사람들에게 알려줄 필요도 없습니다.

This is the notion of decentralized identity management. 
이것이 바로 탈중앙화(decentralized) 신원증명 관리의 개념입니다.

Bitcoin doesn’t specify how Alice tells Bob what her pseudonym is—that is external to the system. 
비트코인은 어떻게 Alice가 Bob에게 그녀의 가명을 알려줄지 지정하지 않았습니다. 이는 시스템외적인 것입니다.

Although radically different from most other payment systems today, these ideas are quite old, dating back to David Chaum, the father of digital cash. 
비록 오늘날의 대부분의 다른 지불 시스템(payment system)과는 근본적으로 다르지만, 이 아이디어는 꽤 오래되었으며, 디지털 캐쉬(digitla cash)의 아버지인 
데이빗 차움(David Chaum)으로 거슬러 올라갑니다. 

In fact, Chaum also made seminal contributions to anonymity networks, and it is in this context that he invented this idea. 
사실, 차움은 익명 네트워크에 대한 종자적 공헌을 했을뿐아니라 그런 맥락에서 그는 이 개념(idea)를 발명했습니다.

In his 1981 paper, “Untraceable Electronic Mail, Return Addresses, and Digital Pseudonyms,” he states: “A digital ‘pseudonym’ is a public key used to verify signatures made by the anonymous holder of the corresponding private key.” 
그의 1981년 논문 "추적할 수 없는 전자 메일, 반송 주소, 디지털 가명"에서 그는 "디지털 '가명'이란 해당 개인 키의 익명 보유자가 만든 서명을 확인하는 데 사용되는 공개 키이다."라고 기술 했습니다.

Now, having message recipients be known only by a public key presents an obvious problem: there is no way to route the message to the right computer. 
이제, 공개키로만 메시지 수신자를 알게되면 명백한 문제가 발생합니다. 메시지를 정확한 컴퓨터로 배달할 방법이 없습니다.

This leads to a massive inefficiency in Chaum’s proposal, which can be traded off against the level of anonymity but not eliminated. 
이는 차움의 제안에 엄청난 비효율성을 가져오는데, 익명성의 수준에 반하여 제거될뿐아니라 상쇄 될 수 있습니다.

Bitcoin is similarly exceedingly inefficient compared with centralized payment systems: the ledger containing every transaction is maintained by every node in the system. 
비트코인은 중앙집중적 지불 시스템과 비교하여도 마찬가지로 비효율적입니다. 모든 트랜잭션을 포함하는 장부는 시스템의 모든 노드에서 관리됩니다.

Bitcoin incurs this inefficiency for security reasons anyway, and thus achieves pseudonymity (i.e, public keys as identities) “for free.” 
비트코인은 어쨌든 보안상의 이유로 비효율적인 결과를 초래하기 때문에, 가명(예를들어, 신원증명으로써의 공개키)을 "무료"로 제공합니다.

Chaum took these ideas much further in a 1985 paper, where he presents a vision of privacy-preserving e-commerce based on pervasive pseudonyms, as well as “blind signatures,” the key technical idea behind his digital cash.
차움은 이런 개념을 1985년 논문에서 더 받아들였습니다. 퍼블릭 가명에 기반한 개인 정보 보호 전자 상거래와 과거 그의 디지털 현금의 핵심 기술 아이디어 인 "blind signatures"을 제시했습니다. 

주) https://en.wikipedia.org/wiki/Blind_signature

The public-keys-as-identities idea is also seen in b-money and bit gold, the two precursor essays to bitcoin discussed earlier. 
신원증명 공개키 아이디어는 이전에 논의 된 비트 코인에 대한 두 개의 선구자 에세이 인 b-money와 bit gold에서도 볼 수 있습니다.

However, much of the work that built on Chaum’s foundation, as well as Chaum’s own later work on ecash, moved away from this idea. 

The cypherpunks were keenly interested in privacy-preserving communication and commerce, and they embraced pseudonyms, which they called nyms. 

But to them, nyms weren’t mere cryptographic identities (i.e., public keys), but rather, usually email addresses that were linked to public keys. 

Similarly, Ian Goldberg’s dissertation, which became the basis of much future work on anonymous communication, recognizes Chaum’s idea but suggests that nyms should be human-memorable nicknames with certificates to bind them.

Thus Bitcoin proved to be the most successful instantiation of Chaum’s idea. 
