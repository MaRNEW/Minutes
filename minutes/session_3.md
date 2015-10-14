## Minutes: Session 3 Sending Data Up for Network Management Benefits
* Date: 24th September
* Time: 14:00 - 15:45
* Chair: Joe Hildebrand
* Minute Taker: Diego Lopez
* Panel:
  * Humberto La Roche (Cisco)
  * Andreas Terzis (Google)
  * Patrick McManus (Mozilla)

### Introduction (Joe Hildebrand)
* Short statements from the participants and leave room for conversation
* Consider SPUD, though just being a prototype so far… 

#### Humberto La Roche
* The radio environment is extremely complex. TCP is a very difficult protocol to be used there. They are living in different realities
* Middleboxes are not going to work well when encryption becomes commonplace, but there is an entity who knows everything in a mobile network: the base station. Information from the base station can be of high value for any other entity in the communication path. Middleboxes will be necessary in the mobile networks, at least as a boundary between the two worlds. They are not necessary a good or bad thing
* There are clear use cases for collaborative frameworks between content providers and mobile operators
* Enhanced content distribution (with costs shared by both parties)
* The case of header enrichment
* Objections among the audience to this particular case, associated with enrichment being a super-cookie
* Parental control
* Throughput guidance is a great idea

#### Andreas Terzis
* Throughput guidance is part of a bigger effort about the network sharing information with the end points
* Apart from real-time improvements, it can help in getting a better idea on how well transport protocol behave in improving user experience
* It needs evolution (think of security implications, for example) but it points to a promising direction
* With info from the network applications can actually change their behavior explicitly and immediately
* An API for operators to share congestion status and the general state of a cell before the application starts sending any data
* Usable to shift traffic or change application behavior
* Another API defined to make the applications aware of the user data plans and their limitations and change application behavior accordingly

#### Patrick McManus
* This is an easier problem than data from the application to the network. The direction of the information flow matters
* There are trust issues for sure. Authentication is a key aspect
* Explicitness and authentication are a great improvement from “transparent” behaviors
* Serious concerns about certain information being shared (like the limits of data plans)
* Don’t forget about net neutrality
* Expand the notion of network-to-app or network-to-user (“you tell me what you know about me") and bring it to a real E2E Internet
* This is not a radio problem, but a TCP problem
* Do not forget great parts of the world where privacy is not the first concern at all

#### Discussion
* __Aaron Falk:__
    *    I’d challenge the assumptions the wireless connection goes to the endpoint where the app sits
    *    Cell phones are more essential for Internet access in the developing world
* __Ted Hardie:__
    *    We are trying to find a way of information sharing that is collaborative, and to identify who needs the information to change its behavior
    *    Certain information can reveal very much about the user and/or the network to the providers
* __Andreas Terzis:__ The application can provide back to the network information on QoE
* __Humberto La Rouche:__ There is somebody in the network very much aware of everything: the base station. Whatever the answer we come up with, the base station is going to have a key role
* __Tom Anderson:__ Fixing TCP may not be the answer to a broken TCP. What we may need to do is talking about a different Internet: SPUD, and especially ICN could have the solution
* __Joe Hildebrand:__ This one of the reasons why the IAB is here, as it has to continuously think of the Internet architecture and its evolution
* __Patrick McManus:__ There is hope in the TCP front. There are up-the-stacks solutions like blind caches. We don’t need to reinvent the wheel
* __Dirk Kutscher:__
    *    We should not specialize this too much on the base station. There are many potential problem points in the network
    *    There are many things to optimize, at different layers, and we’d need to have a more holistic view
* __Humberto La Rouche:__ Could be interesting to have a hop-by-hop throughput guidance
* __NAME__: Anything that exposes the network condition can expose competitive information
* __Humberto La Rouche:__ Make sure you do it in a way that can help TCO to evolve
* __Andreas Terzis:__ Endpoints can measure the performance of the network anyway
* __Joe Hildebrand:__ All have something to gain in this game
* __Jana Iyengar:__
    *    TCP is based on a very specific network model and that’s the cause for the problems it suffers under other conditions. We need new abstractions for making transport protocol evolve
    *    I like throughput guidance because it provides hints to be used by the new control abstractions
* __Humberto La Rouche:__ You say you can characterize the radio environment so you can derive a congestion control that fits it. I disagree. The radio environment is impossible to characterize because is too complex in that respect
* __Jana Iyengar:__ It is not about characterizing every possible variation, only the essential properties over the appropriate timescales
* __Andreas Terzis:__ TG is not a magic bullet. It is up to the endpoints to react
* __Patrick McManus:__ The core point is whether we can build a controller that can adapt to a radio environment and provide a better experience, and preserve E2E
* __Christian Huitema:__ Sawtooth is a tradeoff to solve a generic problem providing a robust solution. The same way TCP is not carved in stone, we don’t need to assume the wireless lower layers protocols are. We could try to fix them as well
* __Andreas Terzis:__ TCP has improved in the last years, since we started talking about improving it
* __Natasha Rooney:__ Bring the reasons why you like or don’t like the idea of network sending information to the app (trust issues, etc.)
* __Jari Arkko:__
    *    The question is whether we can make a protocol used by billions of people better
    *    Can we make use of things like TG without exposing personal information (any permanent ID should be considered personal)?
    *    And do we need need protocols for this? Can we rely on existing ones, like in the case of IPv6?
* __NAME (Cisco):__
    *    We must separate the discussion on why we share the information from where the implement the control based on this. Radio is one of the ends, and there is a great heterogeneity in the E2E path. We should think about hop-by-hop or similar approaches
    *    The radio network is evolving well beyond current uses, think of IoT
* __Patrick McManus:__ I believe we can build something working over multiple-lins
* __Joe Hildebrand:__ I think we have to think of other inputs to the controller, including power consumption 
* __NAME (Huawei):__
    *    I agree application can do better with the help of the network, but the other way must be used as well
* __Joe Hildebrand:__ That’s the next panel
* __Andreas Terzis:__ The exchange must be bidirectional. We have to think about what is the right granularity
* __Jana Iyengar:__ I work on QUIC, and many of the problems we are talking here are not only TCP problems, but general problems, and we are trying to solve them in QUIC. It is important we identify the required information to be exchanged
* __Joe Hildebrand:__ Discussing about the interesting information can help us in improving current protocols without needing a  dramatic change in them
* __Salvatore Loreto:__
    *    TG has shown that collaboration between network and content provider requires a strong trust framework
    *    I am not as pessimistic as Humberto about characterizing radio networks, as many of the problems comes from different approaches to design and implement them. Higher uniformity would bring an easier characterization
* __Humberto La Rouche:__ A general congestion control applicable to mange the whole path would be impractical
* __Stephen Farrell:__
    *    Sending information from the network to the app must be done with a sense of privacy. We need to very conservative in that respect
    *    The baseline here should be to avoid anything that can be considered a personal identifier. Common practice is to share data that can be used as such
    *    The major challenge we have is to identify the best practices with respect to privacy
* __Humberto La Rouche:__ We indeed need to document where we want to be in the industry in this respect, because those data are being required
* __Patrick McManus:__ Common practices are not necessarily requirements
* __Joe Hildebrand:__ One of the reasons for content providers to like encryption is to avoid in-network modifications that translate into customer complaints
* __NAME (Huawei):__
    *    Declaring the nature of goods helps in their delivery
    *    The loop of control shall be in the network
* __Wendy Seltzer:__ Just to wrap up with respect to privacy. As Patrick said even actions done in good faith by good actors can have undesirable effects
* __Blake Methany:__
    *    End users has an agreement with endpoints not with intermediaries
    *    Humberto: Why cannot the consumer have the same agreement with its network provider?
* __Ted Hardie:__ We have to very careful to design mechanisms that cannot be used for other purposes. to avoid the risk of further ossification 
