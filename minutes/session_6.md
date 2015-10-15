## Minutes: Session 6 Transport Layer: Issues, Optimisation and Solutions
* Date: 25th September
* Time: 11:00 - 12:30
* Chair: Spencer Dawkins
* Minute Taker: Karen O’Donoghue
* Panel:
  * Aaron Falk, Akamai
  * Zubair Shafiq
  * Jianjie You
  * Marcus Ihlar
  * Jana Iyengar

### Opening Slides (Spencer Dawkins)
* Network operators will not expose detailed information on their networks. 
* What if there is no collaboration between content providers and network operators? 
 * Will we end up in an arms race on network heuristics. 
* Buffer bloat is an issue and not just for mobile networks. 
* AQM has all the characteristics that you might want. 
* Congestion control - sprout (from MIT) ??? (University of Illinois) 
 * will change in the near future
* Do we still need these transparent boxes in the future/

### Aaron Falk
* What has changed in congestion control...
* Huge amount of innovation in congestion control 
* New ways of detection congestion as opposed to loss
* Two questions (missed second one)
 * What breaks if everything is encrypted? (I still don’t get what the problem is)

### Ted Hardie
* Push back on Aaron’s statement that he doesn’t know what the problem is?
* Resource optimization is what the problem is about
* Encryption is real and growing, wireless cellular networks ARE over subscribed

### Patrick McManus
* If we did have one bit, how are we going to carry it, how are we going to authenticate it. 

### Jana Iyengar
* It is possible to do this, the question is whether the cost is worth it. 
* I don’t know what the bit would be ultimately. 

### Discussion
* __Aaron Falk:__ Data is helpful in solving the problem. Plea to operator community to provide data to help us (the IETF) better understand the problem. 
 * We do need to hear from both content providers and network providers. What is the cost of no or reduced network management in the face of encryption. 
 * Traffic classification is not a problem, it is a solution. 
* __Wendy Seltzer:__ tussel, need to involve all the parties in the discussion
 * Any schemes that expose more meta data can be exploited for correlation and will be resisted. 
 * On the topic of deployment - new transports - if an operator has problem with this
* __Kevin Smith:__ good point as part of the GSMA group, work on a template to gather this information, perhaps anonymize it, and bring it to the IETF. 
 * Don’t discriminate on users, about application flows
 * When data is brought then the problems can be better understood and talking about one bit, don’t we already have ECN
 * ECN doesn’t work for QUIC
 * importance of having a process where we can share data and better understand each others problems
