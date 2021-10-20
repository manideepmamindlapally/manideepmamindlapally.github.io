These are the research topics I have been working on up until now.

---
## Security and Privacy - The Commitment Problem
Collaborators: _[Amitalok J Budkuley](http://www.facweb.iitkgp.ac.in/~amitalok/index.html)(guide), [Anuj K Yadav](https://anuj-k-yadav.github.io/), [Pranav Joshi](), [Manoj Mishra](https://www.niser.ac.in/users/manojmishra)_

Commitment is a cryptographic protocol. To understand this, think of an example. Courtesy [[_Winter 'et al. '03_](https://arxiv.org/abs/cs/0304014)]. Say there are two kids, Alice and Bob, playing a game of chess. It gets night and they decide to continue the game in the morning from the same position they leave off. However, there is one concern. If a player, say Bob were to play the last move in the night, Alice would have an entire night to think over her next move. This makes the game unfair. To do away with this problem we can ask Alice to think and write down his next move on an envelope and seal it off in the night itself. This way she _commits_ to that move. Only in the morning she _reveals_ it by playing that move. Bob then verifies by opening the seal and checking the envelope. This is a raw execution of the _commitment protocol_ where a trusted third party, the sealed envelope is used.

In our work we study and design commitment protocols that instead use certain "noisy" communication channels as a resource. These "noisy" channels are an interesting resource. We investigate commitment characteristics _v.i.z.,_ the rate of the protocol, the (im)possibility result for different behaviours of this noise. While doing so we also explore different noise models: DMC with cost constraints, compound channels for general input. We also look at a few interesting channels specialised for binary input: Unfair Noisy Channels, Elastic Channels, Reverse Elastic Channels. An important focus is also to design capacity rate achieving computationally efficient protocols.

---
## Singleton bounds for catalytic entanglement assisted classical  quantum error correcting codes
Collaborators: [_Andreas Winter_](https://www.icrea.cat/Web/ScientificStaff/andreas-winter-556)_(guide)_

Singleton bounds are well known and serve as an important performance bound on the parameters of _classical_ error correcting codes. It's fairly simple to derive these bounds using Shannon information theoretic properties over a classical erasure channel. Now, there has been an effort to characterise similar bounds for _quantum_ error correcting codes as well. Unlike just the number of bits transferred in classical communication(or information processing), the performance of a quantum communication model has three main resource components: $q$ _qbits_ of quantum information transfer, $c$ _cbits_ of classical information transfer and $e$ _ebits_ of shared entanglement. Using protocols such as _entanglement distribution_, _super dense coding_, _elementary coding_ and _quantum teleportation_, some count(amount) of some of the above resources can be seen to be at least as powerful as some count(amount) of some other resources.

In our work, we model a generalised quantum communication setup where the communicating agents _Alice_ and _Bob_ start with some amount of quantum resources: $q'$ _qbits of noiseless quantum channel_; $c'$ _cbits of noiseless classical channel_; and $e'$ _ebits of shared entanglement_. Over some general quantum channel using some (error-correction) coding scheme they wish to perform :_q'bits of quantum information transfer_; _c'bits of classical information transfer_; and _e'bits of shared entanglement generation_. Using _Von Neumann_ entropies and Shannon style information theoretic properties, we characterise a **singleton bound capacity region** for the gain in amount of each of the three resources.

---
## Covert Communication over Quantum Channels
Collaborators: [_Ligong Wang_](https://perso-etis.ensea.fr/ligong.wang/)

