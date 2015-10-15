## Minutes: Parking Lot
* Date: 25th September
* Time: 14:30 - 15:30
* Chair: Ted Hardie
* Minute Taker: Rich Salz

Speaker is Ted Hardie unless stated otherwise.

### Items In Parking Lot
Two initial items
* Metrics:How can we get information out from operators, etc, collected at GSMA, etc, anonymized, etc, to provide metrics for real data so we can test and evaluate hypotheses.
* Layer of applicability: (network<>UE at radio/MAC layer, or higher); where is the right place to do the work

### Metrics
* How is radio resource control impacted by encryption, for example?
* ECN notifications, deployment of ECN
* Suggestion to thnk about sources of information, not necessarily the items
* Interested in hearing about middlebox deployments (numbers/types) in operator networks
* We need data, but don’t now get tangled up in encodings (e.g.)
* How/what can we exchange info so that overall wireless system is best used by everyone
* Treat less as “we have a problem” and more as “how can we optimize”
* Restrict domain/space to radio, e.g and not boil the ocean for the whole internet where we can’t agree on what “fast” means
* HOPS research group wants you!
* We want virtuous cycle, more data feeds more requests for data, etc. etc
* Not unlike IPv6 deployment, such as where competitors met at IETF to exchange best practices
* Is there a need for IAB to do liaison work?   Seems to be Natasha, etc. informally is good enough, avoid the red-tape (and cant for research groups anyway)
* Get NDA’s among various parties, exchange data, and informally bilateral cooperate, bring things forth; don’t want for next IETF
* Operators can do experiments in a lab about effects of encryption and resource; don’t need live production data, should also be easier to share
* Use the marnew list to talk about test framework

### Layer of Applicability
* Risk 1: boiling the ocean – don’t try to solve 19 year old TCP-over-satellite, e.g
* Risk 2: other cases other than UE to LTE network (mobile phones, not wireless uplink on company shuttle, e.g.)
* Include 3G
* Quality of the info we get?  Can we trust it?
* What abstraction of the RAN control loop can we abstract into the transport control loop
* Should discuss types of application traffic, to make existing lab tests more “real”
* Network doesn’t know what the apps need
* Apps have local viewport, but getting end-to-end information is important
* Want to be able to do real tests on real networks with new stuff being tested
* We need to come up with something, like an I-D?, that talks about what a carrier could provide (the a & b for a/b testing); writing things down is helpful
* What’s the simplest thing we can do that gets us forward progress? Propose an operator run tests with same content plain/encrypted, and see impact and bring that data back.  Don’t build formal framework at first.
 
