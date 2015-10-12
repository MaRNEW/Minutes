## Minutes: Scene Setting
* Date: 24th September
* Time: 09:20 - 10:00
* Chair: Stephen Farrell
* Minute Taker: Sanjay Mishra

Speaker is Stephen Farrell unless stated otherwise.

### Goal of this slot
* How many people here are familiar with IETF? Majority raised hands. 
* How many people know about GSMA?  Not too many raised hands.
* Stephen says, his last slide is for discussions/input for the goals of this workshop
* Read notewell – parts are highlighted 
* Goal is to get on the same page to avoid arguing about topics where prior discussions have already occurred.  No point in discussing unsolvable problems.

### Statistics and Updates
Shows stats on increasing HTTPS traffic. Stephen notes stats data is provided by:
*    Randy Bush provided stats
*    Netflix provided some data as well
*    Google provide, SMTP/TLS
*    Mozilla stated, 36% or 55% page loads are HTTPS (depending on what you are measuring)

Encryption is increasing, it will not stop…
* CDN - ~50% traffic is encrypted
* Everything is not encrypted. Traffic analysis can tell you a lot. 
* We are talking about multiple layers of encryption.

__Christian Huetima:__ stands up and raises a question. Are we talking from two sides of our mouth? 

* No that is not the case. There is encryption but information can be used and goals of the w/s are to understand/analyze what is needed?
* Stephen refers to MaRNEW email thread on Trust. Trust without qualifying? Who trusts whom for what? Need to be careful without fully qualifying. 
* Key management for end-to-end encryption. 
* Anti-spam, malware are real problems. Need use cases. Most justification and policy don’t seem to hold ground but there are some real-challenges. 
* There are transport issues. Radio network vs transport? The topic has to be discussed.
* Deployment of encryption is increasing, but there are more threatening environment, pervasive monitoring is real, motivation apart, there is reaction against it.
* Turn on encryption to discourage, and trend is there and will accelerate. It will not stop. We need to discuss how we can work

### IETF Process
Provides IETF process background by way of listing number of RFC’s (see list below):
*    RFC 1984, 2804, 3365, 3552, 6973, 7258, IAB statement on Internet confident, 7525, 1984
*    Refers to Brian Carpenter’s presentation in IETF?? In Toronto.
*    May 2015 Stepehen’s  summary of progress since IETF-88

Is there anything similar in GSMA similar to IETF processes?


### GSMA overview
* Mobile Operators worldwide (800 Operators) and 250 telecommunications communications companies are members
* GSMA started out initially to help on policies in working with regulators and governments. GSMA works on:
   *    Public Policy
   *    Technical programs
   *    Events – mobile world congress, Mobile 360 series conferences
   *    Working Groups, billing, fraud
   *    Works on network evolution
   *    Standards gets worked on 3GPP, 
   *    Bandwidth optimization standards
   *    Security on the RAN and core network (physical)
   *    GSMA promotes these new network standards
      *    Major network releases
      *    Work with operators to encourage implementation
      *    Work through issues
   *    Encrypted Data Communications

### Scope
Stephen shows a slide with Suggested Scope:
*    Assume, no broken Crypto, CipherText increasingly common
*    Aim is to analyze the situation and identify specifically what are achievable tasks that could be tacked in the IETF or GSMA (elsewhere?)
*    We should not delve into
    *    Ways of doing interception (legal or not) see RFC 2804
    *    Unpredictable political actions

Stephen invites all to comment for live updates to objectives/scope.

### Discussion
* __Aaron Falk__: It is all about tussle. ISP’s got to make money, congestion control is not the only factor, The slides do no capture precisely what is needed. Gives example that wireless spectrum is not unlimited. Suggests wording at the MIC to say something like, “efficient use of resources”
* __Jana Iyengar:__ More of a clarification. Congestion need to be controlled true for all networks, wherever you have shared resources. Would like to see how congestion control (CC) in RAN any different with transport. What CC problems are hard to solve in wireless than wireline networks?
* __3rd speaker (did not catch the name):__ What is exactly the problem that encrypted traffic would cause to the network? If we can have a clear statement, what is the problem with encrypted traffic would be useful and we can address the issue.
* __Spencer Dawkins:__ One of the things has been close to me in transport area (refers to paper from 2006). We have made progress in Transport. Refers to Stephen’s slide where Stephen had referenced to change in the mindsight. Spencer adds changes are needed not only the mind sight but protocol too.
* __Kevin Smith:__ Seeks clarification on scope. 
* __Tom Anderson:__  how/why RAN is different? From Net Op POV, network mgmt. Says RAN is very complex. Says Operators cannot give specific issues to IETF. Understanding the complexity may help move closer to the solution. Fundamental issue for Operators is that they have to manage the network that is fairly complex. Working with them to understand issues may help to move forward.
* __Aaron Falk:__ Will provide further refined statement to what he spoke earlier. Refers to  “Tussle” paper. Flexibility is needed. Useful outcome would be in identifying players, identify points of tension, particularly network management, what is the various point of interest? What is inhibiting network management?  IF we prohibit use of then they will break (let’s wordsmith afterwards
* __Jana Iyengar:__ Two points. Things are done in certain way so far. With encryption, things may look different. How the RAN works, how the user gets served, how well it affects users. It is important to understand complexities of RAN. It will be useful to make abstractions on RAN. Understand RTT timescales. Why those complexities matter, where and why?
* __Salvatore Loreto:__ Why we want to have two network mgmt?  Want better QoE and QoS and improved Internet. When there is a perceived problem in the network, first place you reach out to is Operator. It is difficult to describe in just few words why RAN is different. Put more antennas, you would end up with Radio pollution. IF we want better Internet, we want to consider, QoE for end-user as good as possible w/o infringing upon user privacy and security.
* __Gianpolo:__ Issues we see on RAN are similar on Wi-fi. Add user choices. 

### Finalised Minutes
Stephen has made some textual changes live. Asks if anyone disagrees with changes? No objections are raised.

