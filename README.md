## Latest version : https://github.com/blockchain-lab/shared_vision_towards_programmable_economy/wiki

#### Click here to Edit: https://github.com/blockchain-lab/shared_vision_towards_programmable_economy/wiki/Home/_edit

# Laws for creating trust in the blockchain age

Authors: Delft University of Technology, invite RvIG, Chamber of Commerce, Land Registry Agency. Possibly BC3, DNB/AFM, banks, optionally StartupDelta?

#### very tight deadlines
- July 10: first readable draft, distributed to partners
- July 16: partner feedback processed and alignment completed
- July 22: Scientific Journal submission!

**abstract**
_New platforms have disrupted the taxi business (Uber), hospitality (Airbnb), tourism (booking, expedia), and marketplaces (Amazon, Alibaba). We take these validated concepts to the next level, generalise their operating principles, and combined these fragmented platforms into a single infrastructure. We propose a new organisational principles for our economy, called a self-sovereign economy. Each layer in our proposed economic blueprint is designed to reinforce the strength, usability and profitability of the other layers. Our aim is to transform digital identity, money, trust, and markets. Our leading and illustrative use-case is the following value chain: the mortgage process, transfer of real-estate ownership, and selling on an open market of housing investments._

_Our blueprint is ambitious, will take years to realise, and is impossible to implement by a single organisation. Like Email, GSM, and GPS, our programmable economy facilitates new business opportunities and alters existing business practices. First, we outline a solution for the digital identity problem using a blockchain and self-sovereign identity prototype with end-to-end cryptographic integrity checks, avoiding data honeypots, and void of central gatekeepers. Second, we outline our ideas to re-architect the existing banking system for sub-second electronic business transactions, beyond the current slow and costly money transfers. Third, we provide a realistic roadmap to upgrade the trust and two-way rating system used by renting platform Airbnb and other pioneers to a global public infrastructure with ability to rate any legal entity, offering full openness, and storage on our tamper-proof blockchain. Finally, based on trustworthiness reports, trust calculations, and sub-second money transfers we demonstrate our Internet-deployed decentral marketplace can trade any asset and can be applied to any value transfer network._

### introduction
Humanity has a disposition to trust, meaning the tendency of individuals to be willing to depend on others.
Technology is altering our notion trust. Technology platforms such as Uber and Airbnb disrupt how taxi services are provided and the way in which apartments are rented out. 

Trust is essential for these platforms: people step into the car of a person they never met before or let strangers sleep in their spare room without worries.
These platforms use rating systems as the foundation for their quality and safety measures. For instance, pre-testing for potentially dangerous drivers and prescreening is [reduced](http://www.cnbc.com/2016/02/23/understanding-ubers-five-star-rating-system.html) and replaced with a continuous quality monitoring system.
The Uber smartphone app asks both driver and passengers to provide feedback on their experience. The software averages the 1 to 5-star ratings of the most recent [500 trips](https://help.uber.com/h/7b64dda6-78f5-4575-b7da-3c9e40d2c816). If this average long-term quality rating of a driver drops below a certain level, it automatically triggers [contract termination](https://www.forbes.com/sites/ellenhuet/2014/10/30/uber-driver-firing-policy/#7d29b53b1527). 
The traditional dynamics of trust are altered on such platforms. Employment regulations are under [pressure](https://www.ft.com/content/6f4ac284-362b-11e7-99bd-13beb0903fa3?mhq5j=e3), some courts found that Uber violated local taxi regulations [[1](http://www.reuters.com/article/us-uber-denmark-idUSKBN13R14G),[2](http://www.reuters.com/article/us-uber-tech-southkorea-idUSKBN17S09F),[3](http://www.reuters.com/article/us-uber-netherlands-investigation-idUSKBN0N81G620150417)].
For the UK these platforms are responsible for lowering unemployment levels, reducing fixed employment contracts by a few percent, enforce the trend towards zero-hour contracts and self-employment. A 2017 UK government report states that currently 1.1 million people work within this _[gig economy](https://www.thersa.org/globalassets/pdfs/reports/rsa_good-gigs-fairer-gig-economy-report.pdf)_.
The laws which govern trust, employment terminations, and access to marketplaces is no longer the exclusive domain of national law. The laws of trust are now partly inside commercial software.

This work aims to help transform the gig economy. We aim to institutionalize the empowerment of workers and small businesses with our software, rules and architectural principles.

First, we designed and created an operational open source prototype of the core Uber functionality, matching drivers and passengers. Our non-profit alternative aims to be more transparent, fair, and open. Second, we created a alternative set of rules and principles for the emergence of trust, using only the repeated interactions between strangers. Third, we present a blueprint of a public infrastructure and prototypes for each part of this blueprint for the gig economy. Our proposed public infrastructure in principle should be able to offer non-profit alternative to current matchmaking platforms (e.g. Uber, TaskRabbit, Amazon, Expedia, Booking, etc.). Finally, we hint at how such an infrastructure might be used to realise what has become known as the _programmable economy_.

Blockchain technology is at the core of our proposed Uber alternative and blueprint for a public gig economy.
However, Bitcoin and Ethereum are in our opinion unsuitable for this task or others such as land registration. We do not consider cybercurrency research in the remainder of this work. Our reason is that all current work based on coin creation, proof-of-work or variants thereof lack robust and effective ties to any legal system, or even the real world in general. The current generation of cybercurrency-based blockchain technology lacks a durable governance structure. Severe disagreements exists within these communities, as various fraction battle for control of ecosystems worth billions. The cybercurrency ecosystem is unsuitable for land registration as it occasionally has periods dubbed [civil war](https://www.bloomberg.com/news/articles/2017-07-10/bitcoin-risks-splintering-as-civil-war-enters-critical-month) by the media. We also do not consider private or consortium blockchains, as they do not offer any significant advantage versus classical distributed databases. We focus on the tamper-proof leaderless database type of solutions. The statements and opinions in this paper are based on our decade-long experience of deploying and gradually improving our own ledger, installed by 1.8 million users. We deployed a very primitive fully distributed ledger in [August 2007](http://news.bbc.co.uk/2/hi/technology/6971904.stm), pre-dating the launch of Bitcoin.

### Problem description

The cardinal problem is: who owns the trust?

We propose a new organisational principles for our economy, called a self-sovereign economy. Each layer in our proposed economic blueprint is designed to reinforce the strength, usability and profitability of the other layers. Our aim is to transform digital identity, money, trust, and markets. 

We will open a new direction for science by pioneering the future sharing economy (non-profit, open, and fair).

ToDo: Empowered citizens
[financial sovereignty](http://www.persee.fr/doc/ecofi_1767-4603_2009_hos_9_1_5491)

In May 1962 the vision of a "[time-sharing computer system with many
remote stations](http://dl.acm.org/citation.cfm?id=1460847)" was presented, known as The Internet today.
Nobody owns the Internet. This has been a critical factor for its decade long success story. The Internet consists of numerous Autonomous Systems which are loosely coupled and have a common numbering mechanism.
On top of this global communication infrastructure we build email, videoconferencing, entertainment platforms, search engines, marketplaces, countless cloud services, and essentially a digital economy.
However, after many decades of failures we still lack a similar infrastructure for
essential economic primitives such as: identity, money, trust, and markets.

We present a vision of a challenging nature, to re-invent our global economy based on the organisational principle of The Internet itself: self-governance. Our work is facilitated by strong identities, sub-second money transfers, digital trust, and blockchain-regulated marketplaces.

Joseph Stiglitz co-authored the "Architecture of Economic Systems" in 1985, describing how decision making units can be organized together within a system. It presents a basic framework to compare the performance of decentralized and centralized economic systems. Centralized economic systems have given away to decentralized forms.

We believe that Blockchain technology enables decentralized economies of higher efficiency and stability then currently known. We call our organisational principle a "self-sovereign economy", owned by nobody and everybody. Our work differs substantially from market-based decentralized economies. We are applying ideas fundamentally concerned with freedom of individuals, embedding a natural disposition to trust, and combining it with a very unforgiving blockchain-based mechanism for rule breaking economic actors: digital ostracism.

Our work has more architectural details, feasible laws, and operational prototypes when compared to a somewhat similar idea by consultancy firm Gartner Inc. from 2015, dubbed the programmable economy. They describe it as _"the programmable economy, enabled by metacoin platforms and smart technologies, will support new forms of value exchange, new kinds of markets (including dynamically defined on-demand markets), and new kinds of economies such as the attention economy, the reputation economy, the on-demand economy and the resource optimization economy."_[[REF](http://www.gartner.com/newsroom/id/3146018)]

ToDo: self-sovereign economy
self-governance.
We present a blueprint for creating a self-sovereign economy. Our proposal is based on experimental science, for each component within our architecture we crafted an operational prototype and conducted real-world testing.
One with full sovereignty of all decision making entities, full transparency of their past performance, and 
In this article we present an enhancement to the decentralized
New laws and principles to structure economic activity.

Rapid progress of technology has impacted our notion of trust!
We step in the car of a stranger (Uber), sleep without worries in house of a stranger (Airbnb.

ToDo: Citizen empowerment, money without banks, etc.
 
1962 advice " 'to begin is everything',
even if it is necessary at first to
build research systems along lines that
would be uneconomic for widespread application."

 architectural outline for BC3 vision.
 Existing proposals for Bitcoin and Ethereum aim to build an entire socio-economic ecosystem from cratch. So far they failed.

Stated in [[REF](https://papers.ssrn.com/soL3/papers.cfm?abstract_id=2943227)]: "the present economic systems are highly centralised in nature. They are prone to single point failures, i.e. a failure by the central authority has a cascading effect on the whole economy. Moreover, due to the centralised nature of the setup, any failures have to be corrected by the central authority alone. Local solutions can only be temporary in
nature. Thus, self-correcting mechanisms are lacking in a centralised (i.e a central bank) economic system."

First we need to address the digital identity problem. ToDo: expand.

Second we provide a roadmap to transform our usage of money. By reengineering and building upon existing antiquated payment systems we provide a realistic, legally compliant, and efficient overlay. Re-use the existing infrastructure and transform it into loosely coupled autonomous entities.
We provide a proof-of-principle for making international money transfers with sub-second speed, near-zero commissions, instant clearance, and real-time settlement. No progress is possible without a transformation of our expensive transaction network build in 1970s (swift) using a programming language from the 1950s (cobol).

We propose to re-organise parts of the global economy by using the following three rules: replace central decision making with decentral supervision {e.g. in Dutch 'horizontaal toezicht'}, and digital ostracism for rule breaking economic actors.
We propose a new decision making doctrine: uncompromising transparency, full openness, and radically decentralised. 
We believe our blueprint to take many years of effort, but still viable, realistic, and based on technology which is already partly implemented and validated.

Our programmable economy blueprint consists of a natively-digital economic system with self-governance to avoid any single-point-of-failure, security grounded upon the laws of physics (avoiding software), radical transparency, publically verifiable claims on economic actors within the blockchain, reputation tracking for each economic actor, elaborate mechanisms to establish trust between strangers, legally frinctionless enforcable contracts, and facilitate a single blockchain-regulated digital marketplace for generic economic value exchange and any-asset trading.
Digital ostracism or ecosystem banning is our cardinal mechanism to incentivise each participant to contribute towards a global desirable outcome and protect against freeriding, fraud, and abuse.

We outline a trust-based blockchain architecture, present partial implementation results, and show the possible usage, for instance, land ownership transfer. The scope of our proposal is broad, it should be usable across sectors and possibly replace paper-based procedures. In August 2007 we launched a primitive fully distributed ledger. Based our ledger deployment experience of the past decade we present a global architecture of a third generation blockchain fabric. This technology stack covers the complete range from low-level hardware with our Physical unclonable function prototypes towars our blockchain-regulated decentral marketplace.

### Increasing economic efficiency by decentralized blockchain-regulated markets

Traditionally, inter-organizational coordination is realized through one out of the following methods:
* by bilateral agreements: easy to arrange (sometimes within a single day), most often used for single transactions (buying a single product or service), not always the most economically efficient outcome; often along existing relations
* using tenders: for larger, more expensive and/or long-term contracts: more difficult to arrange (may take months), if broadly announced, possibility to obtain most economically efficient outcome; significant risk regarding trust issues
* through a specialized open market/platform (e.g. power market, AirBnB, eBay, expedia, AMT): if there is a market, this can be quite fast to arrange, and if the traded products are not too complex, often efficient matches are found: trust is taken care of by the market operator/authority; however it takes a lot of effort to set up such a specialized market place

Each of these existing methods perform poor on one of the following criteria: efficiency of allocation / time to agreement / trust-risk / initial set-up costs.

As processes within companies get more and more efficient by automation, there is also a strong demand for increasing the efficiency and reducing the time to agreement with other organizations.
For example, a demand for high frequency transactions occur when:
* logistics: exchanging transportation tasks
* information exchange: coordination of charging slots: EV routing
* coordinating use of (scarce) capacity on an infrastructure: Frits, Rens, Joris

We present a feasible system architecture for efficient, fast, and secure usage of blockchain technology to coordinate existing businesses.

### The State of the Blockchain

ToDo: keep in special issue scope
```technische uitleg en huidige technologische stavaza.```


### System architecture

![image](https://github.com/blockchain-lab/shared_vision_towards_programmable_economy/blob/master/stack_simple.png)

![image](https://github.com/blockchain-lab/shared_vision_towards_programmable_economy/blob/master/tech_stack.png)

The National Bank stated that "if the blockchain is the answer what is the question".
 
### Distributed databases for trust, value transfer, and legal registries

How to store and govern authoritative answers to ownership questions.

- cybercurrency versus blockchain database (.js)
- yet another distributed database model (Hierarchical, relational,
NoSQL, graph-based,..)
- new: permissionless, no servers, no central governance
- new ownership model: nobody owns the blockchain-database

BAG register as currently open linked data [[inspiration REF](http://discipl.org/discipl-technology-for-a-future-society/)].

To be determined: offline identificatie van mensen die bepaalde rechtspersonen mogen representeren.
Openbaar electronisch handtekeningen register; waarin elke bedrijf kan registreren welke
natuurlijke personen bepaalde authorisaties of verantwoordelijkheden dragen.
Bijvoorbeeld Onderneming X verklaart dat persoon Y tekenbevoegd is voor 
financiele verplichtingen tot bedrag Z.

### TrustChain technology stack

We now introduce our TrustChain technology stack, presented in Figure x. This stack can roughly be divided in four parts. The lower levels consists of Physical Uncloneable Functions (PUFS), biometric-based authentication and self-sovereign identity. These components are essential for the ambitious goal to create a decentralized, secure identity framework, named IPv8. These layers will be discussed in Section x.

The next two levels are defined by our blockchain data structure, TrustChain, scalable consensus and reputation mechanisms that use prior interactions between for trustworthiness estimation. Our TrustChain architecture will be elaborated in section x.

Markets and trade lie at the heart of a capitalism economy. First, a mechanism to transfer currencies in real time will be discussed. Next, we present a blockchain-regulated, decentralized market, capable of trading any asset and without a central point of control. By combining the functionality of our decentralized trading platform and real-time value transfer with conditional payments or smart contracts, essentially a programmable chain of value transfer can be created. This will be the focus of section x.

All our aforementioned components combined provide powerful tools to create trust and initiate interactions with others. Different applications, using parts of our technology stack will be discussed.

  Our BC3/Delft technology portfolio / stack / architecture consists now of:
- PUF (REF: Modeling SRAM start-up behavior for physical unclonable functions)

A physical uncloneable function (PUF) is a physical device that is easy and cheap to manufactor but practically infeasible to duplicate, due to process variation of the integrated circuit in the device. Their typical usage can be found in applications, requiring a high level of security, for instance, self-sovereign identity. The devices offers tamper-proof and safe storage of cryptographic keys. Each PUF device contains an unique fingerprint, determined by the randomness of embedded components. A PUF responds to challenges and leads to unique but unpredictable responses, together forming a challenge-response pair (CRP).

![image](https://user-images.githubusercontent.com/325224/27855788-122137a2-616c-11e7-8a8e-32f6a08f8b92.png)

A key-storage system based on a PUF can be built in the following way. The mechanism proceeds in two phases, the enrollment phase, where a key, based on a PUF fingerprint is generated and stored and the reconstruction phase, which restores the secret key that was generated during the enrollment phase. This process is displayed in Figure x.
* Enrollment phase: first, the reference response of the targeted PUF is measured. This response is used as input for the Fuzzy Extractor, which consists of a privacy amplification module and ECC encoding. The privacy amplification module converts the PUF reference response to a usable cryptographic key. Additionally, helper data is computed using error-correcting code (ECC) encoding and stored in memory attached to the device. This helper data itself is not sufficient to restore the secret key and is used during the reconstruction phase.
* Reconstruction phase: reconstruction starts by measuring the PUF response, which is used as input for the Fuzzy Extractor. The helper data, generated during enrollment, is used to perform the information reconciliation and generates the PUF reference response. After privacy amplification, the programmed key is restored.

PUFs can also be used for identification purposes. An authentication mechanism based on CRPs works as follows. The entity that aims to verify users based on a PUF, produces the device and stores an initial set of CRPs securely in his database. Next, the device is given to the user. When the user wishes to authenticate himself, he presents the PUF and the verifying party, in possession of a set of CRPs unique to this device, sends a random challenge to the device. If the PUF provides the correct response, the user is authenticated. Since cloning or mathematical modeling of the device is non-trivial, this is a secure mechanism to use for authentication.

For TUDelft publication on PUF technology: "[Modeling SRAM start-up behavior for physical unclonable functions](http://ce-publications.et.tudelft.nl/publications/1298_modeling_sram_startup_behavior_for_physical_unclonable_fun.pdf)"

- self-sovereign identity system for people, organisations and objects
- identity governance, claim verification and selective attribute revealing
- biometric-based authentication of people and legal representatives

We present a mobile biometric-based authentication system that does not involve any central authority or specialized, licensed hardware. An proof-of-principle mobile application has been developed for Android, capable of matching fingerprints using the built-in device camera. By using device-specific components like the camera, no permissioned or specialized, contractual hardware is needed. This work provides a solution for portable trust and our framework has been specifically designed to serve as a building block for a self-sovereign identity solution.

<img src="https://cloud.githubusercontent.com/assets/325224/24321615/e9771e18-1150-11e7-91bf-484d44906fea.png" width="350">

The procedure for fingerprint acquisition is divided into three components. First, the user opens the application and takes a photo of his or her finger inside an elliptic-shaped area. Next, the captured photo is processed and analyzed using a skin detection algorithm, noise reduction and contrast enhancements. A local feature detector, Oriented FAST and rotated BRIEF (ORB), is used to detect feature points which are used during the matching phase of the fingerprint. This yields the data presented in Figure x where the feature points are indicated as small dots. Finally, the captured fingerprint is matched against known ones available in the embedded database. Devices such as the Google Pixel which are equipped with 128GB of storage space, can store up to ten million fingerprints.

 [https://arxiv.org/abs/1706.03744](https://arxiv.org/abs/1706.03744)
Operational open source framework, with low accuracy (proof-of-principle).


- elastic persistent storage of data, metadata, and versioning services
- transitive trust and real-time incremental reputations for any entity
- TrustChain: transaction storage fabric and self-governance

The TrustChain transaction fabric is designed around the notion of agents performing transactions with each other. In comparison to traditional blockchain constructions like Bitcoin or Ethereum, each agent in the TrustChain network maintains and grows their own chain of historical transactions. We now discuss the creation, storage and dissemination of transactions recorded on TrustChain.

![image](https://github.com/blockchain-lab/shared_vision_towards_programmable_economy/blob/master/trustchain_tutorial_1.png)

Figure x shows a transaction record which is the output of an interaction between user A and B. Both users cryptographically sign this transaction, acknowledging that they agree with the transaction. After the signatures are placed, both users persist the transaction data to their local storage.

![image](https://github.com/blockchain-lab/shared_vision_towards_programmable_economy/blob/master/trustchain_tutorial_2.png)

A natural way to organize transactions is to chain them together. Transactions are stored in a blockchain data structure where each block contains exactly one transaction, both signatures of the interacting agents and a pointer to the prior block in the chain. This pointer is the hash value of the previous block in the chain (any secure hashing algorithm can be used for this purpose). This idea is illustrated in Figure x. Furthermore, each block is accompanied with a sequence number, uniquely identifying the specific block in the chain. Each user creates a genesis block and keeps track of their own transaction history. Every transaction block is present in the chain of both transaction participants.

The data structure in Figure x is void of any control by other users. As a consequence, a user is able to tamper with their chain of transactions by inserting, removing or reordering records, without being noticed. The integrity of this new transaction chain can be restored by recomputing all prior pointers. In this situation, users are unable to prove malicious modifications of one's chain. Users might also choose to not append a transaction to their local chain, i.e. if this transaction has a negative impact on this user.

![image](https://github.com/blockchain-lab/shared_vision_towards_programmable_economy/blob/master/trustchain_tutorial_3.png)

This vulnerability is mitigated by including an additional pointer in each block, see Figure x. This pointer is a reference to the prior block in the chain of the other transaction participants. When two users are interacting, their chains get intertwined or entangled. This mechanism strenghtens the tamper-proof property of TrustChain. As presented in Figure x, each block has two incoming and two outgoing pointers. Note that this scheme can easily be extended to support transactions between more than two participants, by incrementing the amount of outgoing pointers in a block.

![image](https://github.com/blockchain-lab/shared_vision_towards_programmable_economy/blob/master/trustchain.png)

As users complete transactions with each other, they become quickly entangled with other users. Figure x shows a part of the distributed TrustChain ledger. Seven blocks, created by seven participants are displayed, together forming a directed acyclic graph (DAG). Again, note that each block contains exactly two incoming and two outgoing pointers.

Before a new block is added to a chain, a validation process takes place to verify the consistency and integrity of the local chain. This validation includes a verification of the pointers, hash values, transaction data, and signatures <CITE GITHUB>. Only if the aforementioned checks pass, the block is appended to the chain, committed to the local storage and optionally shared with other users.

Our approach differs from second generation blockchains in various ways. Instead of a global, consistent and distributed ledger, every user maintains a personal history of interactions where in most blockchain-based systems, there exists one ledger which is acknowledged by a majority of the network participants. Consistency is achieved by a consensus mechanism like proof-of-work or proof-of-stake. While network consistency is essential for a cryptocurrency system to prevent the double spending attack, it is not a hard requirement for a generic transaction ledger. In essence, we do not aim to prevent fraudulent operations but rather be able to detect them afterwards during the verification stage when appending new transaction records to a local chain. The absence of a global consensus mechanism allows for superior scalability with regard to transaction throughput since parallel transaction processing is inherently possible in TrustChain.

TrustChain blocks are designed to be disseminated and replicated in the network. In particular, this is important when using a transaction history as input for a reputation mechanism (see Section x). Additionally, this makes the system resistant against network churn where users go on- and offline at a fast rate. Each user operates on their own bulk storage of blocks, resulting in partial storage of the global graph. Collecting information of other users is challenging due to the vulnerability to various attacks, their limited resources and the burst of their interactions. Prior work investigates this problem and propose solutions for reliable and secure record collection <CITES>.

TODO: misschien hier nog wat afsluitende woorden over TrustChain? Bijv: we envision TrustChain as a generic transaction ledger, used on a large scale bla bla...

#### Scalable Consensus

Many blockchain fabrics have a requirement for a consistent network state. This requirement holds in particular when considering digital money (cryptocurrencies) like Bitcoin or Ethereum. Consensus is usually in place to prevent the double-spending attack where users transfer the same digital asset twice in multiple transactions. Possibility of such an attack impacts reliability and trust of the system. Unfortunately, most consensus mechanisms are computationally expensive and limit the global transaction throughput of the system. For instance, the Proof-of-Work consensus mechanism implemented in the Bitcoin fabric limits the theoretical transaction throughput to around seven transactions per second which is by far not enough for a medium to large-sized trading platform. In comparison, Visa processes several thousand transactions every second.

We extend our TrustChain architecture with a fault-tolerant, horizontal scalable consensus mechanism, capable of detecting malicious activities performed by users. As far as the authors are aware, this is the first horizontal scalable blockchain fabric. We designed our system based on three important objectives:
- Reaching global consensus on a global state: global consensus renders many types of malicious activities useless since the global state has consent of honest users in the network.
- Fault tolerance: our consensus mechanism should be unaffected by the presence of adversaries, with or without purpose attempting to manipulate the outcome of the global consensus. Usually, these attacks are successful when the amount of adversary users reach a specific threshold. Additionally, each transaction must be verifiable after consensus is reached.
- horizontal scalability: in this context, horizontal scalability means that as more users participate in the network, the global transaction throughput increases. Note that the Bitcoin system is not horizontal scalable since the global transaction throughput is not dependent on the amount of users in the network.

- Business primitives: legally binding identification, authentication, signatures, irrifutable notifications, business transactions, archiving, contracts, e-invoicing, e-factoring, and IFTTT logic.
- real-time IBAN/BIC money transfer, conditional payments, currency conversion, clearing, and settlement
- decentral blockchain-regulated markets
  
  We present a feasible system architecture for efficient, fast, and secure usage of blockchain technology in existing businesses.
  
### TrustChain experiments

We have implemented TrustChain and the scalable consensus mechanism discussed in Section x. This section will focus on experimentation to assess the global transaction throughput and consensus duration. It is assumed that every node generates two transactions per second. We investigate the effect of the number of facilitators in the network; due to implementation-specific constraints, our network can host at most 32 facilitators. We investigate two modes of transaction processing. The first mode is the fixed-neighbour mode where a user only transacts with their immediate neighbours. In the second mode, called random-neighbour mode, for every transaction we select a random user in the network to transact with. The size of each transaction is approximately 500 bytes. It is assumed that every user knows the IP address and identity of all other users. All experiments are executed on the DAS-5 supercomputer.

![image](https://github.com/blockchain-lab/shared_vision_towards_programmable_economy/blob/master/throughput-vs-population-fixed.png)

![image](https://github.com/blockchain-lab/shared_vision_towards_programmable_economy/blob/master/throughput-vs-population-random.png)

The global throughput of the mechanism is displayed in Figure x and y. On the horizontal axis, the network size is shown as the amount of users whereas the vertical axis denotes the transaction throughput in transactions per second. As a first observation, note the linear relationship in both figures between the population size and transaction throughput; this strongly indicates the horizontal scalability property for a network up to 1200 users. In both figures, the throughput rate lowers when the number of facilitators in increased. This is explained by the fact that more facilitators require additional network communication between users, introducing overhead and latency.

An additional observation is that the overall throughput in Figure y where users interact with random neighbours, is lower than in Figure x, where we transact with predetermined neighbours. This is caused by a caching mechanism where network communication is saved when interacting multiple times with the same user. This caching mechanism does not provide benefits when transacting with random users, leading to more network communication. While the fixed-neighbour approach might not be an adequate representation of the real world (users also transact with strangers), it is helpful to analyse and understand the characteristics of the consensus mechanism.

### Land registration application

### Global Mortgage Finance market (application)

### Inter-personal/organizational cooperation (application)

As an example of the broad applicability of a trust network, please consider the following coordination problem.
Electric vehicles (EVs) have a limited driving range defined by their installed battery capacity, which is limited because batteries are large, heavy and costly.
Consequently, for longer drives they need to recharge, in a way similar to the refueling of fossil-fuel-based vehicles.
Very different, however, is the time it typically takes for such a refill: for EVs this can be anywhere from 30 minutes to several hours.
This is a problem in particular when the capacity at recharging stations is limited: if a driver arrives at a charging station (with an almost empty battery) and has to wait for another car to be charged first, this has a significant  effect on the total travel time.
Apart from the solution to design such charging stations for peak capacity requirements, solutions have been proposed to better coordinate the time and location where vehicles charge.

For example, a charging station could offer a reservation system where drivers can book a charging slot in advance as soon as they know at what time they will arrive at the station [].
Such a system would require only bilateral trust and systems like these have been around (without a blockchain) for many years, e.g., for administration purposes at governmental front desks, restaurants, etc..
However, this system leads to significant inefficiencies when arrival conditions are not completely certain.
In particular this holds for travel times, since these may be very uncertain especially around peak times when such reservations matter.
Reserving a larger time window introduces extra (lost opportunity) costs on the side of the charging station, or booking a later slot introduces extra costs on the side of the driver.

Another solution is a cooperative one where all drivers share and coordinate their charging plans among themselves [].
Previous work has shown which algorithmic solutions can be used to combine stochastic information based on historic travel  information with stochastic policies for routing and charging, and how this can be used for coordinating these policies.
What is still missing, though, is a system to reliably exchange this information.


### Conclusions
