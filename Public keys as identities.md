### Public keys as identities

이 글은 보안 원장이 디지털 통화를 쉽게 만들 수 있다라는 이해에서 시작했습니다.

이 주장을 다시 확인해 보겠습니다.

Alice가 Bob에게 지불하기를 원할때, 모든 비트코인 노드들에게 트랜잭션을 브로드 캐스팅합니다.

트랜잭션은 단순한 문자열입니다. 이는 Alice에 의해 서명된 Bob에게 어떤 값을 지불하기를 원하는 설명의 인코딩입니다.

이 서명된 성명서가 마이너에 의해 장부에 궁극적으로 포함되게되면 실제 트랜잭션이 이루어집니다.

어떤 방식으로든 Bob의 참여는 필요가 없습니다.

그러나 transaction에 없는 것에 초점을 맞춰보면, 분명히 앨리스와 밥의 신원증명(identities)은 없습니다. 대신 트랜잭션에는 각각의 공개 키만 포함됩니다.

이것은 비트코인(bitcoin)의 중요한 개념(concept)입니다. 공개키는 시스템의 유일한 신원증명입니다.

트랜잭션(transaction)은 주소(address)라고 부르는 공개키들간에 값을 전달합니다.

신원증명에 대해 "말하기" 위해서 상응하는 비밀키(secret key)를 알아야 합니다.

중앙 권한이나 등재(등록)없이 새로운 키쌍을 생성함으로서 언제든지 새로운 신원증명을 생성 할 수 있습니다

사용자이름을 얻가나 특정 이름을 선택했다고 다른사람들에게 알려줄 필요도 없습니다.

이것이 바로 탈중앙화(decentralized) 신원증명 관리의 개념입니다.

비트코인은 어떻게 Alice가 Bob에게 그녀의 가명을 알려줄지 지정하지 않았습니다. 이는 시스템외적인 것입니다.

비록 오늘날의 대부분의 다른 지불 시스템(payment system)과는 근본적으로 다르지만, 이 아이디어는 꽤 오래되었으며, 디지털 캐쉬(digitla cash)의 아버지인 
데이빗 차움(David Chaum)으로 거슬러 올라갑니다. 

사실, 차움은 익명 네트워크에 대한 종자적 공헌을 했을뿐아니라 그런 맥락에서 그는 이 개념(idea)를 발명했습니다.
 
그의 1981년 논문 "추적할 수 없는 전자 메일, 반송 주소, 디지털 가명"에서 그는 "디지털 '가명'이란 해당 개인 키의 익명 보유자가 만든 서명을 확인하는 데 사용되는 공개 키이다."라고 기술 했습니다.

이제, 공개키로만 메시지 수신자를 알게되면 명백한 문제가 발생합니다. 메시지를 정확한 컴퓨터로 배달할 방법이 없습니다.

이는 차움의 제안에 엄청난 비효율성을 가져오는데, 익명성의 수준에 반하여 제거될뿐아니라 상쇄 될 수 있습니다.

비트코인은 중앙집중적 지불 시스템과 비교하여도 마찬가지로 비효율적입니다. 모든 트랜잭션을 포함하는 장부는 시스템의 모든 노드에서 관리됩니다.

비트코인은 어쨌든 보안상의 이유로 비효율적인 결과를 초래하기 때문에, 가명(예를들어, 신원증명으로써의 공개키)을 "무료"로 제공합니다.

차움은 이런 개념을 1985년 논문에서 더 받아들였습니다. 퍼블릭 가명에 기반한 개인 정보 보호 전자 상거래와 과거 그의 디지털 현금의 핵심 기술 아이디어 인 "blind signatures"을 제시했습니다. 

주) https://en.wikipedia.org/wiki/Blind_signature

신원증명 공개키 아이디어는 이전에 논의 된 비트 코인에 대한 두 개의 선구자 에세이 인 b-money와 bit gold에서도 볼 수 있습니다.

그렇지만, 차움 자신이 나중에 수행한 ecash 뿐만아니라, 차움의 기반위에 이루어진 많은 일들은 이 사상에서 벋어났습니다.
 
Cypherpunks는 개인 정보를 보존하는 통신 및 상거래에 매우 관심이 많았으며, 그들은 nyms라고 불리는 가명을 채택했습니다.

그러나 그들에게 nyms는 단순한 암호 식별 (즉, 공개 키)이 아니라, 오히려 보통 공개 키에 링크 된 전자 메일 주소였습니다.

비슷하게, 익명의 의사 소통에 대한 많은 연구의 기초가 된 Ian Goldberg의 논문은 Chaum의 생각을 인정하지만, nyms는 이들을 묶을 인증이있는 인간이 기억할만한 별명이어야 한다고 제안합니다.

따라서 Bitcoin은 Chaum의 아이디어를 가장 성공적으로 예시화(instantiation) 한 것으로 입증되었습니다.

---
http://wiki.hash.kr/index.php/사이퍼펑크
사이퍼펑크(cypherpunk)란 암호기술을 이용하여 기존의 중앙집권화된 국가와 기업구조에 저항하려는 사회운동가이다. 암호를 뜻하는 사이퍼(cipher)라는 단어에서 'i'를 'y'로 바꾸고, 기존 권위와 조직에 대한 저항을 의미하는 펑크(punk)라는 단어를 결합하여 사이퍼펑크(cypherpunk)라는 용어를 만들었다. 비트코인 등 블록체인 기반의 암호화폐는 사이퍼펑크 운동에 뿌리를 두고 있다.


-----

This article began with the understanding that a secure ledger makes creating digital currency straightforward. 

Let’s revisit this claim. 

When Alice wishes to pay Bob, she broadcasts the transaction to all bitcoin nodes. 

A transaction is simply a string: a statement encoding Alice’s wish to pay Bob some value, signed by her. 

The eventual inclusion of this signed statement into the ledger by miners is what makes the transaction real. 

Note that this doesn’t require Bob’s participation in any way. 

But let’s focus on what’s not in the transaction: conspicuously absent are Alice and Bob’s identities; instead, the transaction contains only their respective public keys. 

This is an important concept in bitcoin: public keys are the only kinds of identities in the system. 

Transactions transfer value from and to public keys, which are called addresses.

In order to “speak for” an identity, you must know the corresponding secret key. 

You can create a new identity at any time by generating a new key pair, with no central authority or registry. 

You don’t need to obtain a user name or inform others that you have picked a particular name. 

This is the notion of decentralized identity management. 

Bitcoin doesn’t specify how Alice tells Bob what her pseudonym is—that is external to the system. 

Although radically different from most other payment systems today, these ideas are quite old, dating back to David Chaum, the father of digital cash. 

In fact, Chaum also made seminal contributions to anonymity networks, and it is in this context that he invented this idea. 

In his 1981 paper, “Untraceable Electronic Mail, Return Addresses, and Digital Pseudonyms,” he states: “A digital ‘pseudonym’ is a public key used to verify signatures made by the anonymous holder of the corresponding private key.” 

Now, having message recipients be known only by a public key presents an obvious problem: there is no way to route the message to the right computer. 

This leads to a massive inefficiency in Chaum’s proposal, which can be traded off against the level of anonymity but not eliminated. 

Bitcoin is similarly exceedingly inefficient compared with centralized payment systems: the ledger containing every transaction is maintained by every node in the system. 

Bitcoin incurs this inefficiency for security reasons anyway, and thus achieves pseudonymity (i.e, public keys as identities) “for free.” 

Chaum took these ideas much further in a 1985 paper, where he presents a vision of privacy-preserving e-commerce based on pervasive pseudonyms, as well as “blind signatures,” the key technical idea behind his digital cash.

주) https://en.wikipedia.org/wiki/Blind_signature

The public-keys-as-identities idea is also seen in b-money and bit gold, the two precursor essays to bitcoin discussed earlier. 

However, much of the work that built on Chaum’s foundation, as well as Chaum’s own later work on ecash, moved away from this idea. 

The cypherpunks were keenly interested in privacy-preserving communication and commerce, and they embraced pseudonyms, which they called nyms. 

But to them, nyms weren’t mere cryptographic identities (i.e., public keys), but rather, usually email addresses that were linked to public keys. 

Similarly, Ian Goldberg’s dissertation, which became the basis of much future work on anonymous communication, recognizes Chaum’s idea but suggests that nyms should be human-memorable nicknames with certificates to bind them.

Thus Bitcoin proved to be the most successful instantiation of Chaum’s idea. 
