## Minutes: Session 5 Application Layer Optimisation, Caching and CDNs
* Date: 25th September
* Time: 09:00 - 10:30
* Chair: Stephen Farrell 
* Minute Taker: Kevin Smith
* Panel:
	* TA Thomas Andersen
	* SL Salvatore Loreto
	* BM Blake Matheny
	* SM Sanjay Mishra
	* RS Rich Salz
	* MW Mark Watson

### Introduction to Panellists (Stephen Farrell)
CDN is the only intermediary that respects the rules that Stephen tells us; it’s a clear intermediary and trusted to deliver content. CDNs have done a good job in the fixed network. But now, major part of traffic (spec. video) is moving from fixed to mobile. Problem is, how we trust a fixed network CDN in a mobile context. Today you need to put caches in the Gi LAN of the mobile network (or even the radio network), but the landscape is different - it is not so easy to find room in the mobile network, so need to find a way to do that. Also: sometimes operators build their own CDNs (inc. mobile CDNs) because they are also content providers. So, my idea is to leverage IETF CDNi to allow global CDNs to interoperate with mobile CDNs. Challenges: trust, and the mechanism to provide trust (don’t want to share your private key widely); could consider a session key for example. Or, as Patrick mentioned, blind cache can allow the operator to host a cache box to allow content providers to cache encrypted content, and then the customer gets the key themselves at request time (i.e. key not shared with the operator)

### Mark Watson
First, testing. We have a customer care centre (expensive to run) so we test. We assume the network is standards compliant and does not modify’ packets may be dropped etc. But when this is not the case in the field, the service breaks, because the network can modify requests in certain conditions.  Or the network can not be standards complaint, can redirect etc, and we can’t test for that. This results in customer care calls, updates, and hence real costs (including debugging which is expensive). So: when you place network intermediaries that are not standards compliant, you can impose costs on service providers. Hoping this sort of activity (the workshop) can remove this problem. We can’t test this alone, it’s too complex. Second: Adaptive streaming is different. One mode of thinking: Services/devices impose a load on the network. This can be the case for downloads, but for ABR the rate the user gets on Netflix is decided by the network (and Netflix adapts accordingly). So the network is in control of this. Third: Data caps. They can be an economic tool (not in scope), but also a resource rationing tool (incentivize user to reduce usage). User can get an email which may need to be explained to the account owner - it’s not a good idea to bring an emotional factor into a technical problem. Users do not know how many GB are needed to watch videos, check networks etc., as technologists we can solve this better

### Sanjay Mishra
One point is that the encryption at source is increasing, a reflection of the good work of the last couple of years against pervasive surveillance. Now, while that is the right way to go, there is an impact operationally - such as the ability to deploy edge solutions, and hence reduce reliance on the existing infrastructure. A way to persist encryption and store at the edge would be welcome. This would only come about if there are standards, with input from Cps and operators.

* __Aaron Falk:__ ‘serve content’ and ‘transport’ may have different contexts, please can you be more concrete?--
* __Sanjay Mishra:__ Just mean caching at edge

### Blake Methany
I joined the layer 7 load balancing team building proxies, then moved to layer 4, and then moved to mobile and now kernel team. Primary consumers for the edge infrastructure at Facebook was mobile. Problem was, ‘host name not found’ at start of connection, then more DNS errors, then TLS handshake errors - so we moved to a standard C++ problem across mobile platforms. I think there are some problems with mobile radio networks but not fatal. Much bigger problems are e.g. DNS, such as caching DNS resolution for 24 hours for performance reasons, but this can break other things. So an education needed to show what breaks downstream. When we rolled out SPDY, CRIME issue raised problem of header compression. Abstractions that are available as a developer are not always representative of the network you are on. When developers build it is often against WiFi, so they are not experiencing the mobile network problems. TLS tickets, DNS caching can be deployed wrongly. Not every company can build a cache infrastructure or in-network boxes. 2G is still dominant in emerging markets (2s RTT) and remains a bigger problem.

### Tom Anderson
First, the problem statement: propose that we look at this. Encryption is not the problem, rather a catalyst to get together to discuss network management in the broader sense. How do we jointly optimise the customer experience. Actors: application provider, network, device. Sometimes the client is tightly tied to the application provider, and can sometimes extract device information. How can they jointly improve user experience? We heard some examples (caching, CDNs etc) and we need to understand the actors concerns. So, work together, and may require some new protocols and we should get to work to help the issues raised. 

### Rich Salz
No intention to disparage anyone! Interesting point that I want to correct: the CDN is not an intermediary, rather the content provider. E.g., we have the certificate of the content source, so the CDN is the origin server. There are tight business/legal agreements with the content source. When a  network adds cookies, strips headers etc. there is a risk that there will be a challenge from a content source to ask why this content manipulation is done.

### Discussion

* __Diego Lopez:__ My understanding is that we are not doing manipulation but optimisation.  Assumption is that networks are not respecting standards - guilty (laughs). We also deal with many companies who do not respect standards, and we have to resolve that. If Amazon has a problem, it is the networks that get the customer care call. We are all interested in streaming going through. 
* __Stephen Farrell:__ not interesting is network customer care. But interesting is ‘optimisation vs meddling'
* __Salvatore Loreto__: what I was trying to say, was can we help to improve transport without any modification, for example blind cache
* __Sanjya Mishra:__ can give some examples of where operators work with CDNs, and other examples of where certificates are unverified and user is accessing malware
* __Mark Watson:__ my point was about testing. Standards compliance helps testing. The reason not to modify is because it can break things
* __Tom Anderson:__ point is, how do we fix this. Address the problem in a technical sense, e.g. a protocol to address this.
* __Joe Hildebrand:__ One of the reactions a content provider has to this modification is to add layers of encryption to prevent modification.
* __Diego Lopez:__ I wanted to state, we are all interested here and need each other. Testing for the providers will also be interesting for the operators.  Also helps networks to probe to work out what has gone wrong.
* __Blake Methany:__ First, I don’t care where the problem is, just want to resolve it. We talked to in operator who had a 486 DNS server (3 secs to resolve). How willing are people to have that same perspective of getting the problem fixed rather than the process. 
* __Dirk Kutscher:__ if there is a need to do optimisations, is there a new way to design the network layer or transport layer?
* __Tom Anderson:__ so the solution to the problem is fundamental to that layer, e.g. ICN, which has an opportunity to take requirements around this. Also SPUD, and probably more, around DNS (although there is no DNS in ICN). I think these are old problems, and we may need a new context to solve it.
* __Rich Salz:__ one of the trends is statistics (latencies, transparencies)  - there may be issues with business sensitivity (which cells are congested) - there are privacy concerns across the spectrum, but sharing between us leads to a customer win.
* __Stephen Farrell:__ I find it a puzzle how ICN can deal with cipher text
* __Phil Roberts:__ The implications of encrypted traffic in the developing world. Here there is a lot of international transit for traffic. Does encryption cause issues with CDNs and caching. What are the CDNs goals for the developing world traffic?
* __Mark Watson:__ our approach, we can provide a network cache, makes sense as we generate traffic. But, we don’t yet have a developing world service.
* __Blake Methany:__ we want crypto to work well, we may need keyless SSL in some markets. Business in certain countries can be challenging, the infrastructure is not always there, so a physical network problem rather than technical.
* __Rich Salz:__ we do have a lot of traffic, split browser models prevalent in Africa, our caches are close to the edge - but that may go away over time.
* __Kathleen Moriarty:__ there are lots of anonymity problems in the developing world, there can be much greater impacts for accessing certain content, so anonymity is really important. So encourage you to consider that point.
* __Mark Watson:__ issue there even with blind caching, some people may be interested with who downloaded what file from the blind cache, especially with the 
* __Rich Salz:__ yes, cases where accessing websites can get you killed. Personal anonymity very important focus in major groups. (#####)
* __Stephen Farrell:__ so can SNI be encrypted?
* __Rich Salz:__ yes
* __Jari Arkko:__ I was hoping we can get to concrete items today, we have potential candidates: CDN work in CDNi etc; also how can the application provider and network provider to timeslice the resource allocation per customer requirements; and third category is testing/debugging - what can be made more easily available to small Websites
* __Salvatore Loreto:__ API idea. What Google is proposing with throughput guidance is a good idea, an outbound control plane standard makes sense.
* __Mark Watson:__ our application does optimisation already, a standard way which helps us input into that optimisation, fine. Can also work other way.
* __Blake Methany:__ for application providers that value privacy, my concern is that sharing info risks privacy leak. So must not make monitoring easier.
* __Stephen Farrell:__ Jari mentioned testing/troubleshooting, any wishes there?
	* __Mark Watson:__ using standards is essential, e.g the information going up and down. 
	* __Blake Methany:__ testing has a disclosure aspect, so would like a forum on interoperability testing
	* __Sanjya Mishra:__ Mark, so developing some standards around the interconnect points has value for metrics/testing etc.?
	* __Mark Watson:__ yes, get non-standards turned into standards
* __Patrick McManus:__ What I’m hearing is how to improve applications, but not that it is a mobile-specific problem. Interested in the panel’s thoughts. HTTPbis is considering making blind cache a charter item, thoughts welcome on HTTPbis. Great that there was a mention of Keyless SSL, does the panel think a standard around that help with pop-up CDNs/caches etc and address some of the core problems?
* __Tom Anderson:__ this should apply to all networks. Would characterise mobile as a fixed network where two ends of the wire talk. LTE divides a resource block (time/frequency) and that is the limit (not bandwidth). Number of bits in resource block is variable. A fully loaded LTE sector can be 150Mb or 3Mb. Aggregate throughout of the channel is highly variable due to conditions. LTE network chats to devices to get the optimal resource blocks shared. Handoffs can happen even when you do not move. So that is ephemeral aspect of mobile. But, we should also address all networks.
* __Rich Salz:__ mobile is different in that I can get metrics from one source, not lots of middleboxes. This focus gives us opportunities for measurement. For HSM over network (Keyless SSL) Akamai would be interested
* __Blake Methany:__ we need guarantees on how to handle handshakes
* __Mark Watson:__ order of magnitude difference in variability of mobile vs fixed. Trading off bandwidth vs delay can increase capacity.
* __Salvatore Loreto__: we see trend of more video moving to mobile,  mobile throughput guidance shows we are not yet optimal. Would be good to get together to talk about 5G - LTE is history for operators
* __Patrick McManus:__ pull radio into the answer rather than creating an answer for radio
* __Benoit Clause:__ I like what you said about network management. But what do you mean by it: configuration, testing etc.? Secondly, by whom: the ISP, end user etc? I believe this workshop will be a success if we have some things that we can solve and focus on one to help matters across all the actors here. 
* __Stephen Farrell:__ (to panel) identify one thing to work on
    * __Salvatore Loreto__: caching
    * __Mark Watson:__ one bit for latency bandwidth tradeoff
    * __Sanjya Mishra:__ standard approach for interfaces to content providers
    * __Blake Methany:__ how can we work together to be productive in an all-tunnelled world
    * __Tom Anderson:__ a means to share metrics across actors to better co-operate
    * __Rich Salz:__ what Tom said
* __Vijay Devarapalli:__ caching has helped operators, with faster content delivery and reduced backhaul. Is there a plan to put your caches into the operator network (Gi LAN or RAN)
* __Vinay Kanitkar:__ answer is yes, we work with many operators to cache securely within the network, and looking at it on base stations (prototypes working but long process)
* __Rich Salz:__ as operators you have agreements with major players. Running a CDN product yourself allows that to apply across many customers of those players
* __Blake Methany:__ safe to say we all have plans to deploy with networks. But that is for a small number of major players,  but how do we do that for the rest of the Internet
* __Mark Watson:__ where justified we will provide that box
* __Sanjay Mishra:__ we want to move away from the one-off point solutions
* __Ted Hardie:__ We called this session ‘application  layer optimisation’. We have talked about application optimisations but not the application layer, There is a scaling problem as Sanjay pointed out, i,.e, an independent interface would be needed. So would like to focus on ‘shapes of traffic’ regardless of application, e.g. jitter or latency characteristics with no knowledge of the application. Needs to be standardised, cannot run multiple flavours. So I want to go back to the previous question, what’s the one thing you could do if it related to the application layer?
* __Tom Anderson:__ I gave the answer of metrics, today they will base metrics on the application e.g. via heuristics. But if exchange the metrics, we don’t worry about what the application itself is. These can allow for better resource allocation, because metrics can better inform that and raise the tide of capacity.
* __Ted Hardie:__ clarifying question, is Facebook an application or set of applications?
	* __Tom Anderson:__ set. if it’s all encrypted we may just see the application, but that is not as good for the metrics
* __Rich Salz:__ metrics
* __Blake Methany:__ wanted to say metrics, but I’ll add blind caching
* __Sanjay Mishra:__ need to make sure the network is calibrated to handle applications best. More constraints on bandwidth hogging.
* __Mark Watson:__ anything that makes it easier for the application to adapt. For video quite easy, can be measured per 5s cycle, but less easy for say a Web page
* __Salvatore Loreto__: blind cache
* __Diego Lopez:__ we are talking about collaboration and sharing, also should include the users…on the other hand were talking about not having this just for the major players.This will create a challenge for the trust model and privacy; SPUD still doesn’t have a trust model.
* __Christian Huitema:__ I’m concerned when I hear we want to standardise caching as a solution. One reason behind encryption was to obscure who was looking at what. But pushing a service to the edge in this case is not caching: e.g. cloud document editing at the edge, allows part of the application to be placed at the edge - it’s a distributed application, content server at the edge. Metrics is something we can use however. The backhaul network of a mobile operator is not all that different from that of a fixed network. But the edge of a mobile network allows for a smaller control loop.
* __Stephen Farrell:_ thanks to the panel!
