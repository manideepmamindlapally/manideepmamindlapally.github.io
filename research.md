<style>
  body {text-align: justify}
</style>

My research can be summarised into the following themes. Over the last few years of my undergrad I was working on a couple of projects in **Information Theory**. Over a couple of internships, I was also worked on two **Quantum Information Theory** projects. Recently, as a JRF (at TIFR) I have been working on a **Cryptography** related topic. Independently, I have also been reading up papers and have been interested in **Complexity theory** areas in **quantum**. This is the topic I am currently interested in for my PhD, which I am planning to apply soon.

---
## Singleton bounds for catalytic entanglement assisted classical  quantum error correcting codes
**Collaborators:** _[Andreas Winter](https://www.icrea.cat/Web/ScientificStaff/andreas-winter-556) (guide)_

Singleton bounds are well known and serve as an important performance measure of the parameters of _classical_ error correcting codes. It's fairly simple to derive these bounds using Shannon information theoretic properties over a classical erasure channel. Now, there has been an effort to characterise similar bounds for _quantum_ error correcting codes as well. Unlike just the number of bits transferred in classical communication (or information processing), the performance of a quantum communication model has three main resource components: $q$ _qbits_ of quantum information transfer, $c$ _cbits_ of classical information transfer and $e$ _ebits_ of shared entanglement. Using protocols such as _entanglement distribution_, _super dense coding_, _elementary coding_ and _quantum teleportation_, some count (amount) of some of the above resources can be at least as powerful as some count (amount) of some other resources.
# Research

In our work, we model a generalised quantum communication setup where the communicating agents _Alice_ and _Bob_ start with some amount of quantum resources: $q$ _qbits of noiseless quantum channel_; $c$ _cbits of noiseless classical channel_; and $e$ _ebits of shared entanglement_. Over some general quantum channel using some (error-correction) coding scheme they wish to perform : $q'$ _qbits of quantum information transfer_; $c'$ _cbits of classical information transfer_; and $e'$ _ebits of shared entanglement generation_. Using _Von Neumann_ entropies and Shannon style information theoretic properties over erasure channels (both i.i.d. and block erasures), we characterise a **singleton bound capacity region** for the gain in amount of each of the three resources $Q=q-q'$, $C=c-c'$ and $E=e'-e$.

---
## (Interested topics) Quantum Complexity Theory

There are a couple of topics in this area that I have recently been reading up. One is a work on "Classical Verification of Quantum Computations" by Urmila Mahadev and second is the famous "MIP* = RE" paper by Zhengfeng Ji, Anand Natarajan, Thomas Vidick, John Wright and Henry Yuen. I gave a series of seminar talks on the first topic to _[Rahul Jain](https://www.comp.nus.edu.sg/~rahul/)_ and his group at CQT, NUS (this was initially intended as a screening process for my PhD admission last year, but I withdrew midway after deciding to apply a year later. I continued to give the talks anyways). The latter topic is a long and comprehensive one, involving some operator algebra theory in addition to quantum information and complexity theory. I am currently studying some of the predecessor works and hope to read the paper up in the next few months. 

### Classical Verification of Quantum Computation 

My [notes]({{ site.baseurl }}/assets/files/prints/CQT_Seminar/report.pdf) and [scribes]({{ site.baseurl }}/assets/files/prints/CQT_Seminar/notes.pdf) (not fully complete yet)

Quantum computation many believe is a more powerful tool than classical computation. In this regard, people have wondered that if a quantum computer is actually powerful enough to solve problems a classical computer can't even verify. Are there any problems which a malicious quantum agent can solve and claim an answer to, that can go unchecked by classical parties? There were attempts to proving this is true and some other attempts which tried to prove the opposite. Recent works by Morimae and Ftizimons showed that all polynomial-time quantum computations can be verified classically in polynomial time when given access to just an extra single-qubit measurement device. The paper by Urmila Mahadev settles the answer saying that there actually exists a strategy where even this single-qubit measurement can be outsourced to the prover, thereby devising a polynomial time classical verification scheme for all polynomial time quantum computations. In doing so they use an assumption of unsolvability of the "learning with errors" problem (in order to construct a function class called the trapped door function family), which is a standard practice in many other cryptographic works.

---
## Security and Privacy - The Commitment Problem
**Collaborators:** _[Amitalok J Budkuley](http://www.facweb.iitkgp.ac.in/~amitalok/index.html) (guide), [Anuj K Yadav](https://anujkryadav.github.io/), [Pranav Joshi](), [Manoj Mishra](https://www.niser.ac.in/users/manojmishra)_

Commitment is a cryptographic protocol. To understand this, think of an example. Courtesy [[_Winter 'et al. '03_](https://arxiv.org/abs/cs/0304014)]. Say there are two kids, Alice and Bob, playing a game of chess. It gets night and they decide to continue the game in the morning from the same position they leave off. However, there is one concern. If one of the players, say Bob were to play the last move, Alice would have an entire night to think over her next move. This makes the game unfair. To do away with this problem we can ask Alice to think and write down her next move on an envelope and seal it off in the night itself. This way she _commits_ to that move. Only in the morning she _reveals_ it by playing that move. Bob then verifies by opening the seal and checking the envelope. This is a raw execution of the _commitment protocol_ where a trusted third party, the sealed envelope is used.

In our work we study and design commitment protocols that instead use certain "noisy" communication channels as the resource. These "noisy" channels are an interesting resource. We investigate commitment characteristics _v.i.z.,_ the rate of the protocol, the (im)possibility result for different behaviours of this noise over these noisy channels. While doing so we also explore different noise models: DMC with cost constraints, compound channels for general input; And also a few interesting channels specialised for binary input: Unfair Noisy Channels, Elastic Channels, Reverse Elastic Channels. Recently, we even studied a class of continuous channels called the Unfair Gaussian Channels. Apart from the commitment characteristics above, an important focus is also to design capacity rate achieving computationally efficient protocols.

---
## Proof Techniques for Security of Multiparty computations
**Collaborators:** [_Akshayaram Srinivasan_](https://www.tifr.res.in/~akshayaram.srinivasan/) _(guide)_

What is the notion of security in a general multi party computations? How would one define it? One approach some people have taken is to ensure that a cheating participant is not able to achieve anything (by achieve I mean disrupt the desired output) more than he could have done while not participating in an interactive exchange, but is given just his supposed answer by a god like trusted source. The idea is to model a "real world" where a protocol for the multi party computation gets executed; and an "ideal word". In the "ideal world", we have a trusted godlike party that can compute and deliver just the required answer to all the parties. This setup ensures that no party can disrupt the other one's output. A party, if malicious, can use any strategy they can, but just on their output. Crucially, at the most we allow this party to halt the protocol, but not disrupt the output of other parties any further. This ideal world is set as a secure benchmark. What remains to show is that the outputs for any cheating strategy in the real world can be modeled by the outputs for some strategy in the ideal world, called the simulation strategy. These proof techniques are called simulation proofs. There are some other variations of notion of security that have been studied too. I am currently reading up relevant literature.

---
## Covert Communication over Quantum Channels
**Collaborators:** _[Ligong Wang](https://perso-etis.ensea.fr/ligong.wang/) (guide)_

Covert communication (a.k.a communication wothout detection) is a secret communication model where a sender wishes to communicate some information to the receiver over some channel without the an eavesdropper ever noticing that there was an information transfer at all. It was seen in some earlier works that the maximum information transferred (_bits_) over $n$ uses of a purely classical channel, scales as $\sqrt{n}$. The same was also already studied to hold over classical-quantum channels. The focus of our work is to see if a similar relation holds for covertly transmitting information over purely quantum channels. We are also investigating different classes of quantum channels and how the behaviour varies among them.

---
## Age of Information - Markov Sources
**Collaborators:** _[Amitalok J Budkuley](http://www.facweb.iitkgp.ac.in/~amitalok/index.html) (guide)_

The most common entropic source coding methods (Eg: Hamming codes, Shannon codes) are focussed around optimising expected _"total length of information (or number of bits) transmitted"_. In some practical applications sometimes however, the _number of bits_ isn't the most important metric. As a crude example consider a communication setup like the broadcast of a live cricket match. There the _recency_ of information(how latest the information is) is viewed as more important. For simplicity in understanding, say delays in transmission are a direct function of the number of bits in that symbol packet. In such a scenario, the broadcaster choose to even drop some of the information(symbols) and transmit only the recent/latest information while they remain recent. 

In our work we formulate a metric **Peak age of information** that captures this feature very well. Accordingly, we arrive at a single letter expression and and optimisation expression for this metric using linear algebra and matrix manipulation techniques. For information sources assumed to be independent and identically distributed, after some fairly simple observations, we see that optimising for _peak age of information_ was same as optimising for _number of bits_. That said, the same is not true for Markov sources. It was infact seen that the Hamming code or the Shannon code that optimise _number of bits_ actually don't achieve the optimum _peak age of information_. We are now looking to design a computational scheme to construct a source code that optimises this metric, given the source Markov characteristics.

---

