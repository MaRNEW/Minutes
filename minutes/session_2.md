## Session 2: Trust Models and User Choice

### Chair Karen O'Donoghue

Panel:
* Wendy Seltzer
* Patrick McManus
* Szilveszter Nadas

### Wendy Intro - Security, Privacy, and Performance Considerations for the Mobile Web

* HTML design principles prioritize users over authors over implementers over specifiers over theoretical purity
* 64% of users said concerns over privacy have increased.
* 67% would like to do more to protect privacy.

w3C TAG recent findings on securing the web, e2e encryption, unsanctioned tracking.

Web security updates
*  secure contexts - certain features should only be available in secure contexts.
*  upgrade insecure requests
*  mixed content blocking
*  sub-resource integrity
*  elsewhere: HSTS, HPKP, Let's Encrypt

Emerging Privacy Model of the Web
* user expectations from contexts
* dual use privacy protections - some features may not be thought of as privacy protecting, but users may be using them that way
* Fingerprinting: at the heart of the tussle
* Transparency+

Cooperative Performance

### Szilveszter intro: Cooperative traffic management

Low trust in (mobile) operators. Mobile is different from fixed.

Traffic Management in Cellular

- Growth of data outpaces capacity
- traffic management is mainly implicit
-- fixed shares, dpi
- DPI has issues - encryption, OTT at disadvantage. Users nay perceive as
 hostile to user preferences

Cooperation and the Tussle
- Need demonstrated value and clear interfaces to achieve user cooperation.
- end user shall be able to influence, but can't be too hard

Trust and Policy Controller with middlebox cooperation
- Agent of end user, optional
- may get metadata

Example: Non-economic incentive for user cooperation

Patrick (on behalf of Richard Barnes) (No slides)
- User consent and security as a public good
- running theme in contributions: All sorts of network
 management gear, snowden happened, need consent (from someone)
 to opt in to network management. Operators feel they
 were doing useful things
- Need to think about model where good faith management strategies
 are indistinguishable from attacks. Bad actors will use those
 vectors. Users and content providers unlikely to opt-in.
- e.g. javascript injection (e.g. comcast ad injection) gives
 too much control over browser. Consider great cannon -
 turned browser into DDoS botnet.
- Cookies have been used badly (super-cookies)
- Concern over tracking from third parties. Network
 operator is more like 4th party. Concern about
 network operator tracking. Endpoints will not sign
 up.
- Ossification - more new features are encryption only
 because gear in the network breaks if you do new things.
- Jari pointed out opportunity - Not just encryption changing.
 New approaches up and down the stack.

### Discussion:

Question to Szilveszter re: policy controller. Information to
third or forth party has to be known to both endpoints. Is that considered?

The controller only considered consent from one endpoint. There may be things that need consent from both. But for example CDNs don't usually ask for user consent.

Christian Huitema (CH) - Consider cloud service knows a lot about
user preferences. User may express preference based on profile they sign
up for on cloud service. For example, maybe you ask your bank for everything to
be secured with 2-party authn

SN: Why would user not say the same thing to the network?
PM: Consider superfish. Pretend it was opt-in:-). Back end
did not authenticate data. It's hard to give all parties visibility
into info they need to fulfill policy

Ted Hardie (TH) - Parallel to security as public good is herd immunity.
Higher proportion of traffic using good practice benefits people who are not.

TH- Cooperative traffic thing- historical split browsers where part of work is done
on other side of RAN, compress and stream reduced traffic to endpoint. If
under control of end-user, you have different policy control point. May continue to use it when off of specific network. Some devices roam between wifi, etc. A couple of papers pointed out parental controls. Interesting consequence highlights that RAN operators are also service provides. This is a service. Service delivered even when you are on wifi. Need to distinguish between impact on network management and impact on service providers.

(?) - liked Patrick's statements. Encryption on rise, tussle between concerns. We should embrace crypto and think about how we can redesign around e2e, how much does the network need to know, what are correct abstractions. Difficulties finding useful APIs to express policy. Does paper consider this?

PM: Decisions that seem locally reasonable can cascade in unexpected ways.
Decision to create exception from immunization policy can have disastrouus rsults
in individual cases. E.g. when a person inserts plaintext analytics without
considering privacy issues.

Favors small amount of data from network towards user, who can make decisions on it. E.g ECN. How do you trust and authenticate. Hoped to hear more about that.

WS: Crypto forces explicit conversation about trust and explicit user choices vs
service asserted towards user. Conversation about which services are valued by
end-user opens up market for user choice. Think about crypto offering both privacy and authentication.

SM: We need to allow innovation. Do not define in advance what users can do. Allow experimentation with conversations between user and (controller?)

(?) - Choices of user are often limited within a service because they want the service. Radio networks are different due to limited spectrum. Public resource limited by government. Cannot just expand it, must manage it.

Salvatore: User had already made a choice to use the operator. Already a consent. Keeps hearing that there is a problem for end-user to provide more info for what he is doing, but people are asking for the network to provide information. Privacy of network can become at risk, encourages attacks on networks. Opportunity to use all inputs to design "new" network

Aaron Falk (AF): Informed decisions by end user are important. Choices to sacrifice privacy or not play make people give away privacy. Need finer granularity and more transparency about implications of choice. Balance different for diff communities important. We don't want all or nothing solutions.

WS: Choice does not get immediate feedback. Cost may not be revealed until far future. No real choices to regain privacy. Society needs to give people better
choices. More immediate feedback on costs and benefits. Providers of privacy protecting services give info on risk of using other provider's services. Regulators may demand greater protections if better choices are not offered.

PM: You can look at granularity at different levels. Difficult to make this very
transparent to users. Also can have granularity on how value-added services can be used. E.g. parental controls can be implicit or explicit. Should always
be explicit. Human can make granular decision to use or not, get granular feedback
on consequences. Technical argument: Too many new things break on the internet due
to something implicitly getting int he way. Can't route around them. Granularity helps.

Stephen Farrel (SF): User consent is BS, no real choices. Warning are meaningless.
Whatever direction we recommend, need to allow third policies to monitor or audig how they are being used on behalf of the users.

PM: Authentication is often missing piece in those strategies.

Robert Sparks (RS): In the context of the IETF bcps and principles, notion
of choice in geolocation ended up with 1 bit from w3c. Will we get pushback trying
to put granular choice in front of users?

WS: {w3c0 does not discuss user interface, but they are having discussion on how
to provide reasonable choices to users, knowing users will click the "show me the dancing pigs" button without considering consequences. Room for work that draws on security research and UI design.

Karen Wraps up
