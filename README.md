# Laws for creating trust in the blockchain age

Authors: Johan Pouwelse, Martijn de Vos, Delft University of Technology

invite RvIG, Chamber of Commerce, Land Registry Agency. Possibly BC3, DNB/AFM, banks, optionally StartupDelta?

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
However, Bitcoin and Ethereum are in our opinion unsuitable for this task or others such as land registration. We do not consider cybercurrency research in the remainder of this work. Our reason is that all current work based on coin creation, proof-of-work or variants thereof lack robust and effective ties to any legal system, or even the real world in general. The current generation of cybercurrency-based blockchain technology lacks a durable governance structure. Severe disagreements exists within these communities, as various fraction battle for control of ecosystems worth billions. The cybercurrency ecosystem is unsuitable for land registration as it occasionally has periods dubbed [civil war](https://www.bloomberg.com/news/articles/2017-07-10/bitcoin-risks-splintering-as-civil-war-enters-critical-month) by the media. We also do not consider private or consortium blockchains, as they do not offer any significant advantage versus classical distributed databases. We focus on the tamper-proof leaderless database type of solutions. The statements and opinions in this paper are based on our decade-long experience of deploying and gradually improving our own ledger, installed by 1.8 million users. We deployed a very primitive fully distributed ledger in [August 2007](http://news.bbc.co.uk/2/hi/technology/6971904.stm), pre-dating the launch of Bitcoin. In 2017 we mathematically proven that our TrustChain scales linear and surpasses 10k transactions per second [[REF](https://github.com/Tribler/tribler/issues/2457)].

### Problem description

Contracts, transactions, and the records of them are among the defining structures in our economic, legal, and political systems [REF](https://hbr.org/2017/01/the-truth-about-blockchain). They protect assets and set organizational boundaries. 
These authentic records create ownership, determine citizenship, and define partnerships between entities.
It establishes a goverance layer in which states, economic actors, and citizens interact.
They create trust.

For thousands of years trusted guardians kept authentic ownership records of land and assets in general. These centralized bureaucracies which govern these records have not changed much, while the world is slowly being filled with self-driving cars, trucks, drones, and barges. 
This difference in innovation speed is creating increasing levels of friction around data governance, for instance, the debate "Land registration systems: public, private or privately public?" debate [[REF](https://www.degruyter.com/view/j/eplj.2017.6.issue-1/eplj-2017-0001/eplj-2017-0001.xml)]. 
The legal world might be at the beginning of a transition towards full digitization, additional standardization, and further automation. 
Already 22 years ago the book "Law in a Digital World" was published, however deeds of land transfer are rarely pure bits.

Blockchain enthousiasts claim this technology offers an alternative to any trusted guardian and central bank. It offers us another way to organise society, with a high degree of decentralisation. The resilience of Bitcoin together with the rising gig economy endorses this claim.
The breakthrough that made the gig economy possible was the use of reputation systems to build trust between strangers. Reputation systems collect and process information about past interactions, to help people evaluate the trustworthiness of others [REF](http://www.emeraldinsight.com/doi/pdfplus/10.1016/S0278-0984%2802%2911030-3). However, an individual’s reputation on a platform such as eBay is owned by a profit-driven entity. This leads to the following problems for the social good:
- Lock-in. A solid reputation on one platform is locked into that platform: you cannot move your reputation. Like other forms of lock-in, this inhibits competition and encourages monopoly behavior. Ironically, companies in the "sharing economy" do not share reputations. Users are increasingly being protected by European Union law from such data silos. The newly defined right to data portability allows individuals to obtain and reuse their personal data for their own purposes across different services. 
- Fragmentation. Each company operates its own closed market, only accessible through their smarphone app. This leads to lower overall efficiency, compared to a single open market. For example, the taxi market is fragmented into numerous closed markets operated by companies such as Uber, Lyft, BlaBla Car, Didi Kuaidi, GrabTaxi, Karhoo, etc. Each isolated marketplace tries to match drivers and customers in real-time.

Centralized approaches are ultimately always influenced by the goals and the reliability of the central entity or authority that controls them. 
For this reason central platforms can never be truly generic and universal. With a decentralized approach, multiple independent individuals cooperate in some manner to build a single ecosystem and no one entity has control over the entire environment. This is the model we envision for the future programmable economy: trust relations are not locked to a single profit-driven entity.

The cardinal problem is: "who owns trust"? Creating trust within a public infrastructure has proven to be a hard unsolved problem.

In May 1962 the vision of a "[time-sharing computer system with many
remote stations](http://dl.acm.org/citation.cfm?id=1460847)" was presented, known as The Internet today.
Nobody owns The Internet. This has been a critical factor for its decades long success story. The Internet consists of numerous Autonomous Systems which are loosely coupled and have a common numbering mechanism.
On top of this global communication infrastructure we build email, videoconferencing, entertainment platforms, search engines, marketplaces, countless cloud services, and essentially a digital economy. These examples often contain a single central point of control and authority.
It has proven hard to create a decentralized governance layer for such vital public infrastructure.

Joseph Stiglitz co-authored the "Architecture of Economic Systems" in 1985, describing how decision making units can be organized together within a system. It presents a basic framework to compare the performance of decentralized and centralized economic systems. Centralized economic systems have given way to decentralized forms. The current challenge is to further refine the decentralized form: storage and governance 
of authoritative answers to ownership questions use a public and transparent infrastructure.

Trust, accountability, and reputation mechanisms are closely tied.
Transparency can be used to make an authority accountable in order to establish trust. 
It promotes integrity of operations by monitoring the correct behavior of economic actors [[REF](https://www.petsymposium.org/2017/papers/issue4/paper87-2017-4-source.pdf)].

Creating trustworthy, public, transparent, and decentralized infrastructures is hard. We lack a decentral infrastructure for essential economic primitives such as: identity, money, trust, and markets. 

### Architecture for creating trust

We propose an architecture to create a decentralized infrastructure for four economic primitives.
The novelty of our work is the application of the Internet architecture throughout our architecture, owned by both everybody and nobody. Our work is academically pure. It relies on self-governance, and weak coupling between autonomous entities. 
Each of the four economic primitives are meticulously designed without relying on any middleman, they are void of any central authority, make traditional intermediaries optional, do not require any central server, remove the need for central databases, and even do not depend on Internet connectivity.

Our blueprint builds heavily on the concepts proven within the gig economy and combines it with blockchain technology.
It contains four layers: strong digital identities, sub-second money transfers, digital trust, and blockchain-regulated marketplaces.
We believe our proposal is the first proposal with real-world viability, as it is the only detailed proposal based on rigorous experimental science: running code.
This work is based on a decade of experimentation, for each component within our architecture we crafted various generations of operational prototypes and conducted Internet-deployment tests.
Each of the four layers in our proposed economic architectural blueprint is designed to reinforce the strength, usability and efficiency of the other layers. 

Upcoming sections present how we applied and validated our architecture by creating a decentralized alternative for Uber and an open decentral market for mortgages.

We believe that Blockchain technology enables decentralized economies of higher efficiency and stability then currently known. 
This work broadens the applications of the organisational principle behind The Internet. 
Offering full sovereignty to all decision making entities, full transparency on their past performance, and openness in general.
We are applying ideas fundamentally concerned with freedom of individuals, embedding a natural disposition to trust [[REF](www.socsci.uci.edu/~duffy/papers/trustamongstrangers.pdf)], and combining it with a very unforgiving blockchain-based mechanism for rule-breaking economic actors: digital ostracism. 
The threath of being banned forever from an ecosystem may seem to lack compassion and forgiveness, but boosts trust. 
Game theory shows that the "shadow of the future" removes cheating incentives. Note that fraud differs from blunders by economic actors, which merely impact their reputation (e.g. star rating).
In our architecture we apply the grim trigger defined in 1971 to punish dishonesty, lying, cheating, and fraud [[REF](https://www.jstor.org/stable/2296617)]. In other words, mistakes can be forgiven, but intentional digital manipulations are not.

Our work establishes a blueprint for creating a trustworthy programmable economy.
The term programmable economy was introduced by consultancy form Gartner Inc. in 2015. 
We expand upon their ideas with various architectural details, propose feasible rules, show operational prototypes, and in general mature this concept.
They describe it as _"the programmable economy, enabled by metacoin platforms and smart technologies, will support new forms of value exchange, new kinds of markets (including dynamically defined on-demand markets), and new kinds of economies such as the attention economy, the reputation economy, the on-demand economy and the resource optimization economy."_[[REF](http://www.gartner.com/newsroom/id/3146018)]


![image](https://github.com/blockchain-lab/shared_vision_towards_programmable_economy/blob/master/stack_simple.png)

The Figure above shows the four layers which define our architecture.
First we need to address the digital identity problem, shown as the bottom layer.
A wealth of applications require strong authentication and long-lived secure identities. The Internet requires a common continuously evolving strong identity layer. This would make the Internet safer, better and more efficient. A single common identity layer also needs full decentralisation and self-governance. This blocks progress, for instance, a single standard for globally legally valid electronic signatures does not yet exist.

However, we lack control over our identity, as formulated [within the proposed WebDHT documentation](https://opencreds.org/specs/source/webdht/).
"The Web currently does not have a mechanism where people and organizations can claim identifiers that they have sole ownership over. Identifiers, such as those rooted in domain names like emails addresses and website addresses, are effectively rented by people and organizations rather than owned. Therefore, their use as long-term identifiers is dependent upon parameters outside of their control. One danger is that if the rent is not paid, all data associated with the identifier can be made temporarily or permanently inaccessible. This document specifies a mechanism where people and organizations can cryptographically claim ownership over identifiers such that they control them and the documents that they refer to."

Self-sovereign identities require that users are the rulers of their own identity. This idea was presented in 2012 by Moxie Marlinspike [[REF](http://www.moxytongue.com/2012/02/what-is-sovereign-source-authority.html)].
With this concept people and businesses can store their own identity data on their own devices, and present it efficiently to anyone who wants to validate it. The decentralized storage within concept removes the need for any central database of identity data.
This might be important with the upcoming EU General Data Protection Regulation.

This approach to identity is a complete overhaul to the approach used today by governments using central controlled identity administration frameworks. Users become autonomous by using self-sovereign identities and are free to store their digital passport inside their own smartphone device. Instead of your government assigning you citizen number "0013" or your telecommunication provider renting you cell phone number "0-013" you can claim ownership of cryptographic key "8A4D48B" as you worldwide identity.
Together with cryptographic techniques it becomes possible to identify and authenticate people, members of organisations and objects without even requiring Internet access. A large list of worldwide claimed identities by citizens could replace all central identity administration frameworks.

Being the ruler of your own identity is closely related to the core concept of Bitcoin.
Bitcoin creates money without banks, but also provides users with an exceptional level of control.
The novelty of Bitcoin is: a system where nobody can stop me spending my own money. [REF](http://www.r3cev.com/blog/2016/4/4/introducing-r3-corda-a-distributed-ledger-designed-for-financial-services)
Identity autonomy provides a new level of citizen empowerment and enables [financial sovereignty](http://www.persee.fr/doc/ecofi_1767-4603_2009_hos_9_1_5491).

Second layer is our TrustChain fabric, a blockchain design with loose coupling and linear scalability. 
Our work differs radically from the current generation of cybercurrency, which does not scale beyond several transactions per second. 
We specifically avoid the concept of coins.
TrustChain exclusively focusses on the emergence of trust through repeated interactions.
Instead of using complex mathematical puzzles, our basic building blocks are the interactions between untrusted entities.
Each actor within our ecosystem operates a their own unique database which contains measures against tampering and make prior agreed transactions irrefutable.
Within TrustChain each actor is completely autonomous, owns their own chain, and publishes new electronic business transactions in a tamper-proof append-only manner.
TrustChain introduces a new governance model: self-governance.
It is an ecosystem where ordinary users self-organise into a large-scale Internet-based collective which can be freely joined by anyone, with the special strong property that all authority is temporary.
We define a self-governance system as: a distributed system in which autonomous individuals
can collectively exercise all of the necessary functions of power without intervention from any authority
which they cannot themselves alter.
Self-governance implies a mechanism for peaceful transfer of power. Users ether directly vote on appoint those responsible
for the daily administration of the community through some voting process. Distributed systems with
self-governance have no external overseers and no central controlling servers.


Third we provide a roadmap to transform our usage of money. By reengineering and building upon existing antiquated payment systems we provide a realistic, legally compliant, and efficient overlay. Re-use the existing infrastructure and transform it into loosely coupled autonomous entities.
We provide a proof-of-principle for making international money transfers with sub-second speed, near-zero commissions, instant clearance, and real-time settlement. No progress is possible without a transformation of our expensive transaction network build in 1970s (swift) using a programming language from the 1950s (cobol).

We propose to re-organise parts of the global economy by using the following three rules: replace central decision making with decentral supervision {e.g. in Dutch 'horizontaal toezicht'}, and digital ostracism for rule breaking economic actors.
We propose a new decision making doctrine: uncompromising transparency, full openness, and radically decentralised. 

In a recent economics publication it is stated that with blockchains, "marketplaces can be bootstrapped without the need of traditional trusted intermediaries, lowering the cost of networking.", furthermore they challenge "existing revenue models and incumbents's market power, and opens opportunities for novel approaches to regulation, auctions and the provision of public goods, software, identity and reputation systems" [[REF](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=2874598)].

Our programmable economy blueprint consists of a natively-digital economic system with self-governance to avoid any single-point-of-failure, security grounded upon the laws of physics (avoiding software), radical transparency, publically verifiable claims on economic actors within the blockchain, reputation tracking for each economic actor, elaborate mechanisms to establish trust between strangers, legally frinctionless enforcable contracts, and facilitate a single blockchain-regulated digital marketplace for generic economic value exchange and any-asset trading.
Digital ostracism or ecosystem banning is our cardinal mechanism to incentivise each participant to contribute towards a global desirable outcome and protect against freeriding, fraud, and abuse.

We outline a trust-based blockchain architecture, present partial implementation results, and show the possible usage, for instance, land ownership transfer. The scope of our proposal is broad, it should be usable across sectors and possibly replace paper-based procedures. In August 2007 we launched a primitive fully distributed ledger. Based our ledger deployment experience of the past decade we present a global architecture of a third generation blockchain fabric. This technology stack covers the complete range from low-level hardware with our Physical unclonable function prototypes towars our blockchain-regulated decentral marketplace.


### Land registration application

### Global Mortgage Finance market (application)

### Inter-personal/organizational cooperation (application)

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


### Distributed databases for legal signatures ?

To be determined: offline identificatie van mensen die bepaalde rechtspersonen mogen representeren.
Openbaar electronisch handtekeningen register; waarin elke bedrijf kan registreren welke
natuurlijke personen bepaalde authorisaties of verantwoordelijkheden dragen.
Bijvoorbeeld Onderneming X verklaart dat persoon Y tekenbevoegd is voor 
financiele verplichtingen tot bedrag Z.

### Trust creation technology portfolio

System architecture

![image](https://github.com/blockchain-lab/shared_vision_towards_programmable_economy/blob/master/tech_stack.png)

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

Most blockchain fabrics have a requirement for a consistent state which is agreed upon by (a part of) the network. This requirement holds in particular when considering digital money (cryptocurrencies) like Bitcoin or Ethereum. Consensus is usually in place to prevent the double-spending attack where users transfer the same digital asset twice in multiple transactions. Possibility of such an attack impacts reliability and trust of the system. Unfortunately, most consensus mechanisms are computationally expensive and limit the global transaction throughput of the system. For instance, the Proof-of-Work consensus mechanism implemented in the Bitcoin fabric limits the theoretical transaction throughput to around seven transactions per second which is by far not enough for a medium to large-sized trading platform. In comparison, Visa processes several hundreds of transactions every second. In April 2017, SWIFT recorded an average of 28.38 million FIN messages per day, around 328 per second. This motivates the need for scalability.

We designed, implemented and evaluated a fault-tolerant, horizontal scalable consensus mechanism, capable of detecting malicious activities performed by users. As far as the authors are aware, this is the first horizontal scalable blockchain fabric. We built our system based on three important objectives:
- Reaching global consensus on a global state: global consensus renders many types of malicious activities useless since the global state has consent of honest users in the network.
- Fault tolerance: our consensus mechanism should be unaffected by the presence of adversaries, with or without purpose attempting to manipulate the outcome of the global consensus. Usually, these attacks are successful when the amount of adversary users reach a specific threshold. Additionally, each transaction must be verifiable after consensus is reached.
- horizontal scalability: in this context, horizontal scalability means that as more users participate in the network, the global transaction throughput increases. Note that the Bitcoin system is not horizontal scalable since the global transaction throughput is not dependent on the amount of users in the network.

![image](https://github.com/blockchain-lab/shared_vision_towards_programmable_economy/blob/master/trustchain_cp.png)

We extend the TrustChain data structure with a new type of block, called a checkpoint block. This is displayed in Figure x, showing a transaction block (described in Section x) and a checkpoint block. A checkpoint block consists of a pointer to a previous block in the same chain, a number indicating the consensus round after which the specific checkpoint block has been created, a cryptographic hash of the consensus result and a digital signature, generated by the owner of the chain. We modify the data structure such that the first block in a chain (the genesis block) is always a checkpoint block. The available checkpoint blocks in a chain are used during detection of malicious activities.

Our consensus mechanism proceeds in rounds. The outcome of each round is a set of checkpoint blocks agreed by the facilitators of that round. Facilitators are special user, selected during the first phase in a round of consensus. These facilitators reach consensus not on the individual transactions like in Bitcoin or Ethereum but on the state of every chain. There are two scenarios. If a specific user is not a facilitator, it sends its most recent checkpoint block to all facilitators. When the facilitators received a sufficient number of checkpoint blocks, they start to reach consensus on all received checkpoint blocks using an Asynchronous Subset Consensus (ACS) algorithm. When this algorithm is finished, the facilitators send two messages to all nodes, first the consensus result and second a signature message where the facilitator signed the consensus result, adding authenticity to the consensus result. When a user receives the consensus result and a sufficient amount of valid facilitator signatures, a new checkpoint block is created and appended to the chain. Finally, the new set of facilitators is computed from the new consensus result and the round number is increased. The process starts over now.

- Business primitives: legally binding identification, authentication, signatures, irrifutable notifications, business transactions, archiving, contracts, e-invoicing, e-factoring, and IFTTT logic.
- real-time IBAN/BIC money transfer, conditional payments, currency conversion, clearing, and settlement
- decentral blockchain-regulated markets
  
  We present a feasible system architecture for efficient, fast, and secure usage of blockchain technology in existing businesses.
  
### TrustChain experiments

We have implemented TrustChain and the scalable consensus mechanism discussed in Section x. This section will focus on experimentation to assess the global transaction throughput and consensus duration. It is assumed that every node generates two transactions per second. We investigate the effect of the number of facilitators in the network; due to implementation-specific constraints, our network can host at most 32 facilitators. The size of each transaction is approximately 500 bytes. It is assumed that every user knows the IP address and identity of all other users. All experiments are executed on the DAS-5 supercomputer.

![image](https://user-images.githubusercontent.com/1093806/28093480-c16898e2-6697-11e7-9c7b-3afd03374a21.png)

The global throughput of the mechanism is displayed in Figure x. On the horizontal axis, the network size is shown as the amount of users whereas the vertical axis denotes the transaction throughput in transactions per second. In this experiment, each user transacts with another user in a fixed set of neighbours. As a first observation, note the linear relationship in the figure between the population size and transaction throughput; this strongly indicates the horizontal scalability property for a network up to 1400 users. The throughput rate lowers when the number of facilitators in increased. This is explained by the fact that more facilitators require additional network communication between users, introducing overhead and latency.

Figure x indicates that we have indeed created a scalable consensus mechanism, not bounded by a wasteful, expensive consensus mechanism like Proof-of-Work. With only a few servers, our consensus mechanism is able to reach global throughput rates surpassing that of Visa or SWIFT. Together with components higher in our technology stack, we enabled trusted trade at a large scale.


### Conclusions
