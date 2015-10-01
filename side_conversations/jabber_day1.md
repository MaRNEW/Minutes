richsalz [richsalz@jabber.at/@Work] entered the room. (10:28:37 AM)

10:28:56 AM Rich Salz: hi

russhousley [russhousley@xmpp.rg.net/Russell-Housleys-MacBook-Pro] entered the room. (10:29:25 AM)

barryleiba [barryleiba@gmail.com/Adium8223CCE2] entered the room. (10:29:48 AM)

rjsparks [rjsparks@nostrum.com/unnumerable] entered the room. (10:31:03 AM)

hildjj [hildjj@jabber.org/JHILDEBR-M-N3ZF] entered the room. (10:31:58 AM)

10:33:35 AM Aaron Falk: I don't have a whole lot of jabber IDs.  Invite others who are here...

10:33:38 AM Aaron Falk: (please)

10:37:48 AM Joe Hildebrand: I sent a mail to the list.

ben [ben@nostrum.com/avalon-air] entered the room. (10:39:48 AM)

wseltzer [wseltzer@jabber.org/70c6982479f5f77c] entered the room. (10:40:37 AM)

spencerdawkins [spencerdawkins@gmail.com/androidxQT690E8B62] entered the room. (10:40:40 AM)

10:40:52 AM wseltzer: thanks Aaron and Joe

Karen O'Donoghue [odonoghue@jabber.isoc.org/ISOC-REM-MBA2187] entered the room. (10:41:21 AM)

10:41:21 AM spencerdawkins: Yes, thanks!

10:41:58 AM Joe Hildebrand: I don't think we're logging here, so anything you want to contribute, please try to say it out loud in person.  We can use this for backchannel stuff.

sftcd [sftcd@jabber.org/f61fd2b3cb324935] entered the room. (10:42:51 AM)

10:43:44 AM Aaron Falk: /subject IETF Note Well applies to this room (https://www.ietf.org/about/note-well.html)

jari.arkko [jari.arkko@gmail.com/Adium54B42D82] entered the room. (10:43:49 AM)

Ted.h [hardie@xmpp.rg.net/hardie-macbookpro2] entered the room. (10:43:49 AM)

10:43:53 AM Joe Hildebrand: huh.  that didn't work

10:44:04 AM barryleiba: It's "/topic", I think.

Aaron Falk has set the topic to: IETF Note Well applies to this room (https://www.ietf.org/about/note-well.html) (10:44:10 AM)

10:44:14 AM Joe Hildebrand: there we go

10:44:17 AM Aaron Falk: TIL

dvijay@jabber.org [dvijay@jabber.org/Vijays-MacBook-Pro] entered the room. (10:44:31 AM)

Szilveszter Nadas [szilveszter.nadas@xmpp.jp/Psi] entered the room. (10:44:40 AM)

philshere [philshere@gmail.com/Adium46A193E0] entered the room. (10:44:50 AM)

schukichan [schukichan@googlemail.com/Bulbasaur 9EEF7E6C] entered the room. (10:45:54 AM)

jari.arkko left the room. (10:47:42 AM)

jari.arkko [jari.arkko@gmail.com/Adium12CD6372] entered the room. (10:47:48 AM)

DirkKutscher [kutscher@jabber.neclab.eu/8805362841443104489693853] entered the room. (10:49:14 AM)

Olaf Kolkman (adium) [olaf@nlnetlabs.nl/Dropje] entered the room. (10:50:09 AM)

10:50:22 AM Stephen Farrell: is there much incident monitoring that happens in the RAN?

10:50:54 AM Stephen Farrell: that is, I don't know what kinds of incidents operators want to monitor for in the RAN, anyone know?

Olaf Kolkman (adium) left the room. (10:51:28 AM)

10:52:18 AM dvijay@jabber.org: Not in the RAN, but at the Gi/SGi interface

10:52:22 AM DirkKutscher: Not that I know -- normally this happens in the service network, i.e., behind the PDN-Gateway

10:52:23 AM dvijay@jabber.org: Between the packet core and the Internet

10:52:29 AM DirkKutscher: yes, exactly

10:52:35 AM Stephen Farrell: and what is the GI/SGI interface? 

10:52:55 AM DirkKutscher: this is where operator services are hosted

10:53:01 AM dvijay@jabber.org: The interface that connects the mobile network (packet core, transport and RAN) to the Internet

10:53:05 AM DirkKutscher: TCP optimizers, firewalls, load balancers

10:53:15 AM Stephen Farrell: so any impacts are the same as for any other n/w for this? or ?

10:53:30 AM dvijay@jabber.org: You have NAT, firewall, DPI, parental controls, video transcoding, etc on this interface

10:53:31 AM DirkKutscher: in principle, yes

schukichan left the room. (10:54:47 AM)

markwatson [mwatson6366@jwchat.org/jwchat] entered the room. (10:56:21 AM)

Mary Barnes [mary.h.barnes@gmail.com/AdiumC83B8D36] entered the room. (10:58:24 AM)

schukichan [schukichan@googlemail.com/Bulbasaur A2B65EF8] entered the room. (10:58:57 AM)

10:59:03 AM Ted Hardie: You can actually set up a DNS service on port 443 now using GET requests for DNS URIs; for DNSSEC signed records, you get a pretty close to equivalent experience.  the problem with the non-DNSSEC signed record set is that you must trust the server to which you are connected at the same level you'd trust a recursive resolver.

Blake Matheny [bmatheny@jabber.hot-chilli.net/oakcombs] entered the room. (11:00:25 AM)

benoit.claise [benoit.claise@gmail.com/01D9E2C8] entered the room. (11:00:48 AM)

11:00:50 AM Ted Hardie: I think it would actually get easier in the future, given ALPN as a disambiguation token, but I still support the use of the DPRIVE separate port.  In the long run, it is the right solution.

philshere left the room. (11:01:44 AM)

barryleiba left the room. (11:02:23 AM)

barryleiba [barryleiba@gmail.com/Adium4AF1DD24] entered the room. (11:02:29 AM)

philshere [philshere@gmail.com/AdiumD1D2C2BE] entered the room. (11:02:44 AM)

11:03:25 AM Joe Hildebrand: https://tools.ietf.org/html/draft-smith-encrypted-traffic-management-03

Mary Barnes left the room. (11:03:53 AM)

jari.arkko left the room. (11:03:54 AM)

Mary Barnes [mary.h.barnes@gmail.com/AdiumC93839CA] entered the room. (11:03:59 AM)

jari.arkko [jari.arkko@gmail.com/AdiumC70ECAE1] entered the room. (11:04:00 AM)

11:04:18 AM Stephen Farrell: https://tools.ietf.org/html/draft-smith-encrypted-traffic-management-03

11:06:25 AM Joe Hildebrand: (echo) 

11:07:06 AM Blake Matheny: RRC state transition delays aren't content specific as far as I know. Noted here, for question later.

11:07:34 AM DirkKutscher: This is IMO relevant background info for this discussion: https://tools.ietf.org/html/draft-ietf-sfc-use-case-mobility-01

11:10:50 AM Robert Sparks: be good to get a mike in front of Kevin

11:11:03 AM Russ Housley: +1

11:12:59 AM Stephen Farrell: I'm willing to bet a beer derived heuristics will work better than what applications would actually tell the n/w

11:13:10 AM Ted Hardie: I'll take the bet

Olaf Kolkman (adium) [olaf@nlnetlabs.nl/Dropje] entered the room. (11:13:23 AM)

11:13:29 AM Stephen Farrell: ted owes stephen a beer s

11:13:52 AM Ted Hardie: Get you app deployed and we'll talk 

philshere left the room. (11:14:41 AM)

Olaf Kolkman (adium) left the room. (11:15:04 AM)

11:15:43 AM Stephen Farrell: wrt Joe's statement - if you can verify what the application tells the n/w, then why not just use that? i.e. wouldn't it be good enough?

philshere [philshere@gmail.com/Adium083DA993] entered the room. (11:15:44 AM)

11:15:58 AM Joe Hildebrand: you might be able to act on the hint more quickly

11:16:11 AM Joe Hildebrand: assume that it's right, then run heuristics over time to verify

11:16:21 AM DirkKutscher: @sftcd, yes, but the fundamental question is IMO at what abstraction level you need to classify flows at all

11:16:23 AM Ted Hardie: An example of that is voip—you need a small udp packet train to confirm that you have voice

11:16:32 AM Ted Hardie: You can do it in one with a dscp marking.

11:17:08 AM Ted Hardie: Then, as Joe says, you can confirm to make sure that the packet train confirms, thus catching any buggy marks

11:17:40 AM Stephen Farrell: and that makes a real improvement? any public data/publications to that effect? (not doubting, just wondering)

11:18:13 AM Joe Hildebrand: it's a hypothesis.  that's one of the reasons why SPUD is a prototype is to run experiments to see if that hypothesis pans out

11:19:41 AM benoit.claise: Ted/Joe: confirm what? What is the trutht?  If an end-user wants a real-time service, and you can't confirm that the packet train looks like real-time, you're going to conclude that the application/end user tells lies?

11:20:30 AM jari.arkko: the issue is not that we are missing ability to control - the radio network has *full* control of what goes on where. the issue is how do we drive that decision engine, and based on what information?

11:20:33 AM Joe Hildebrand: perhaps.  if that is EXPLICITLY communicated to the application, it seems like it might not be awful.

11:21:30 AM Joe Hildebrand: any time the network "adds value", i'd love for the application to get notified.

11:21:42 AM Szilveszter Nadas: Another solution is to have the "right" incentives - if the user ask for a service, which requires more resources that could have also an economic consequence not only QoS.

11:22:54 AM Joe Hildebrand: i could also imagine a credit-based system.  if you I lower QoS on other traffic, would the network credit me back some user experience?

11:23:06 AM Szilveszter Nadas: see my paper 

11:23:08 AM benoit.claise: Szilveszter: that's the solution if we don't want people to abuse the system, like DSCP. 

11:23:32 AM Stephen Farrell: is it people who'd be abusing or the applications they've downloaded?

11:23:38 AM DirkKutscher: @Szilvester, yes, in https://www.iab.org/wp-content/IAB-uploads/2015/08/MaRNEW_1_paper_18.pdf we are alluding to the incentives approach (via congestion exposure)

11:23:50 AM Szilveszter Nadas: or more specifically https://tools.ietf.org/html/draft-mihaly-spud-mb-communication-00

11:25:01 AM Szilveszter Nadas: I think that people shall have the final word in what is communicated (if the consequence is on their subscription)

11:25:01 AM Joe Hildebrand: sftcd: some applications, such as bittorrent clients, have knobs that are exposed to the user.  on some OSes, it's harder to get access to the knobs from user space, which means they can't be used for good purposes even.

Blake Matheny left the room (Disconnected: closed). (11:26:01 AM)

11:26:02 AM Szilveszter Nadas: @Dirk ConEx and cong. based charging is definitely a valid alternative. 

Blake Matheny [bmatheny@jabber.hot-chilli.net/oakcombs] entered the room. (11:26:05 AM)

benoit.claise left the room. (11:26:22 AM)

benoit.claise [benoit.claise@gmail.com/D0E54116] entered the room. (11:26:37 AM)

11:26:57 AM Szilveszter Nadas: User control: again some thoughts in https://www.iab.org/wp-content/IAB-uploads/2015/08/MaRNEW_1_paper_16.pdf

11:29:11 AM jari.arkko: FYI, I published a quick blog post that this workshop is happening. The link is here: http://www.ietf.org/blog/2015/09/encryption-and-network-management/

11:29:29 AM DirkKutscher: +1 to what Christian said

11:29:46 AM Ted Hardie: Just to Christian's point, I don't think we want to expose to the network what you are doing, we want to expose what network treatment is required.

11:29:59 AM Szilveszter Nadas: +1 to Ted

11:30:18 AM DirkKutscher: yes, and even that may be doable on a high abstraction level

11:30:24 AM Ted Hardie: At the moment, we infer network treatment from content type etc., but explicit network treatment requests would be more accurate and leak less.

dvijay@jabber.org left the room (This participant is kicked from the room because he sent an error message to another participant: service-unavailable). (11:30:24 AM)

ben left the room. (11:30:39 AM)

11:30:43 AM spencerdawkins: +1 to Tef because that's what the TSV area is going to want to do anyway.

11:31:07 AM Blake Matheny: What incentive is there for the UE to not lie about required network treatment in order to achieve better end user experience?

11:31:12 AM DirkKutscher: so, that could be a good discussion topic: what level of detail is actually neded for such hints

11:31:13 AM spencerdawkins: Now, how accurate that is ...

You have disconnected (11:31:40 AM)

You have connected (11:35:34 AM)

11:31:54 AM Szilveszter Nadas: @Blacke I believe in economic consequences for that.

11:32:02 AM Ted Hardie: The "verification" in that may be mapping the request to known types of traffic, but we'd have to allow for variability.  In video delivery a-la DASH, for example, you might want real time treatment for the very beginning, but BE afterwards once cache fill had started.  But it will vary depending on whether you have a channel-changing app or a different UI for playback

11:32:45 AM Ted Hardie: @Blake if it achieves better end user experience, why do you assume it isn't what they want/need?

11:33:21 AM Blake Matheny: Ted my concern is the same with DSCP/QoS. If you know there are a setting of 0 (slow) and 11 (fast) why would people not always opt for 11?

11:33:43 AM Blake Matheny: We've seen that in FB DC, we've seen that in end user (mobile) applications as well with our request scheduler

11:35:21 AM spencerdawkins: My impression was that one of the hits on QoS WAS that people resisted paying for it historically. Has that changed (at least in the GSMA world)?

11:35:27 AM Szilveszter Nadas: Again why not charge more for 11 than 0?

Aaron Falk has set the subject to: IETF Note Well applies to this room (https://www.ietf.org/about/note-well.html) (11:35:35 AM)

11:35:55 AM Ted Hardie: @Blake  If you have constructed the categories so that it is that ordinal, "fast" vs "slow", you may well get that.  But if you construct it with something closer to queue behavior ("Drop packets instead of queueing"), then you may get closer to matching behavior.

11:36:08 AM Blake Matheny: That's not how carrier billing works.  Users don't pay more for traffic for application X than traffic for application Y.

11:36:21 AM Blake Matheny: Changing that seems, uhm, interesting.

philshere left the room. (11:36:29 AM)

Ted.h left the room. (11:36:32 AM)

dvijay@jabber.org left the room. (11:36:47 AM)

11:36:55 AM Szilveszter Nadas: Anything else sounds really challenging.

11:36:59 AM benoit.claise: What's an application? I spent quite some time on that. It gets complex quite quickly. Jabber is an app, sure. However, file download within jabber is ... a different application.

dvijay@jabber.org [dvijay@jabber.org/Vijays-MacBook-Pro] entered the room. (11:37:00 AM)

ben [ben@nostrum.com/avalon-air] entered the room. (11:37:06 AM)

11:37:07 AM Szilveszter Nadas: Again it do not have to be pay by byte.

11:37:33 AM Blake Matheny: Doing pay by stream type for UE applications seems incredibly challenging. I think there are simpler solutions.

You have disconnected (11:37:35 AM)

You have connected (12:00:29 PM)

11:38:01 AM Szilveszter Nadas: An again I refer to https://tools.ietf.org/html/draft-mihaly-spud-mb-communication-00#section-3, Incentive frameworks.

11:38:10 AM benoit.claise: Blake: +100. And the cost of the billing system will exceed the potential gain IMO

11:38:45 AM Szilveszter Nadas: For me differentiation by service type has two issues, 1 privacy, 2 not every user wants the same for the same service

Aaron Falk has set the subject to: IETF Note Well applies to this room (https://www.ietf.org/about/note-well.html) (12:00:29 PM)

12:01:10 PM Blake Matheny: Szilveszter Nadas: strong agreement here. Even if we could get broad agreement and cooperation, I worry about privacy.

Karen O'Donoghue left the room. (12:01:14 PM)

dvijay@jabber.org [dvijay@jabber.org/Vijays-MacBook-Pro] entered the room. (12:01:29 PM)

Mary Barnes [mary.h.barnes@gmail.com/Adium0036F7D9] entered the room. (12:01:49 PM)

12:03:52 PM schukichan: hello!

12:03:55 PM schukichan: it’s natasha

Kevin [sirles@jabber.cz/KEVIN-SMITHs-MacBook-Air] entered the room. (12:06:29 PM)

Natasha [schuki_@xmpp.jp/Bulbasaur] entered the room. (12:08:16 PM)

schukichan left the room. (12:08:19 PM)

12:08:31 PM Natasha: Testing name

12:08:34 PM Natasha: good good

12:08:41 PM spencerdawkins: @natasha and Aaron, the discussion in the jabber room has been useful - could it be preserved for the participants and for the report writers (whether it's published as part of the proceedings or not)?

12:08:48 PM Kevin: Related to Ted's point: stating 'give me latency' or 'give me bandwidth' to the network per service type seems better than just deliver me better'

12:12:41 PM Aaron Falk: "anonymity loves company" : https://xkcd.com/1105/

markwatson [mwatson6366@jwchat.org/jwchat] entered the room. (12:12:44 PM)

12:12:46 PM Natasha: @spencerdawkins sure will do

12:13:54 PM DirkKutscher: yes, I was thinking along these lines wrt abstraction levels. In addition, applications should be incentivized to respond to imminent congestion/disruptions within these fundamental classes.

12:14:25 PM DirkKutscher: (refering to Kevin's point)

12:24:57 PM Blake Matheny: Kevin: that's essentially what I've implemented. "Needed for view port", "Not needed for view port". I have lots of stories about where this has broken down, and the semantics aren't the issue (we've tried a number).

spencerdawkins left the room. (12:28:07 PM)

spencerdawkins [spencerdawkins@gmail.com/androidxQTB42A342E] entered the room. (12:29:19 PM)

12:30:25 PM Kevin: Blake, I may be talking about another function here (namely 3GPP QCI) which essentially just cares about latency, bandwidth and guaranteed bit rates (or not). The big problem is that these are coarse and based purely on network interpretation of the flow. Based on the comments earlier I think the operators need to better present the characteristics of 3GPP networks towards the IETF so that the specs can evolve sensibly. But - apologies if I've misinterpreted your reply!

12:30:35 PM Joe Hildebrand: what was the compression scheme name again?

12:30:44 PM Stephen Farrell: brotli 

12:30:46 PM Natasha: yes good question!

12:30:59 PM Joe Hildebrand: thx

12:31:01 PM Stephen Farrell: https://en.wikipedia.org/wiki/Brotli

12:31:16 PM Natasha: https://github.com/google/brotli

12:33:30 PM Stephen Farrell: isn't the whole idea of consent broken?

12:34:56 PM Joe Hildebrand: yeah.  almost no user has the knowledge to make an informed consent decision.

benoit.claise left the room (This participant is kicked from the room because he sent an error message to another participant: service-unavailable). (12:34:56 PM)

12:35:57 PM Stephen Farrell: and even if they did have the knowledge, every "click to accept" thing is in practice nonsense, nobody (apps, sites, operators) seems to want to actually ask a fair question ever

12:36:10 PM Joe Hildebrand: nod.

12:36:40 PM Joe Hildebrand: however, being able to ask your browser "why might this be broken", and get details that a service person can use to diagnose, would be terribly helpful

12:37:03 PM Stephen Farrell: *doesn't get the connection*

benoit.claise [benoit.claise@gmail.com/71EEB237] entered the room. (12:43:20 PM)

wseltzer left the room. (12:45:47 PM)

Ted.h [hardie@xmpp.rg.net/hardie-macbookpro2] entered the room. (12:50:30 PM)

12:51:07 PM jari.arkko: +1 to importance of choice & flexibility

12:51:56 PM Ted Hardie: Is anyone aware of any mobile operator who has halted sales of contracts/UEs because of resource constraints in a specified area? (That is, has the resource constrain in the radio resource ever resulted in a constraint on units sold?)

12:52:00 PM barryleiba: Giving users choice will help a fraction of a fraction of a milliuser.  The vast, VAST majority of the users will have no idea at all what any of it means to them.

Ted.h left the room. (12:56:00 PM)

You have disconnected (12:56:24 PM)

You have connected (1:00:08 PM)

12:56:32 PM Natasha: Line is closed. I'll announce to the room in a sec

12:57:21 PM Natasha: eh weirdly i think iOS has permissions right (as right as it can be) atm

Aaron Falk has set the subject to: IETF Note Well applies to this room (https://www.ietf.org/about/note-well.html) (1:00:08 PM)

1:00:53 PM DirkKutscher: @Natasha, yes, the analogy to this discussion is that you don't want an all-or-nothing consent approach -- instead you would want to opt-in into certain forms of (for example) sharing information with the network or application service providers. However, that's not how web pages work today.

1:00:55 PM jari.arkko: barry: not necessarily choice as in one visible in a checkbox to a user. but choice as in technology choices that both users, device vendors, and service providers can decide to adopt. an example: if your only choices are no privacy or full privacy but no interactive/background prioritization, you are in pain no matter what you do. if you had more choice maybe the pain would be smaller.

You have disconnected (1:02:04 PM)

You have connected (1:58:39 PM)

Aaron Falk has set the subject to: IETF Note Well applies to this room (https://www.ietf.org/about/note-well.html) (1:58:40 PM)

Kevin [sirles@jabber.cz/KEVIN-SMITHs-MacBook-Air] entered the room. (1:58:46 PM)

philshere [philshere@gmail.com/AdiumB5B3F5AE] entered the room. (1:58:47 PM)

philshere left the room. (2:00:28 PM)

Mary Barnes [mary.h.barnes@gmail.com/AdiumD78F8471] entered the room. (2:01:19 PM)

wseltzer [wseltzer@jabber.org/06eb87660cc2b74d] entered the room. (2:02:14 PM)

philshere [philshere@gmail.com/AdiumBBF4D8BD] entered the room. (2:02:35 PM)

richsalz left the room. (2:03:05 PM)

richsalz [richsalz@jabber.at/@Work] entered the room. (2:03:08 PM)

philshere left the room. (2:04:15 PM)

philshere [philshere@gmail.com/Adium88AA854F] entered the room. (2:05:24 PM)

2:07:00 PM Aaron Falk: TCP was designed to work over radio.  It just wasn't designed so wireless operators could be profitable.

Karen O'Donoghue [odonoghue@jabber.isoc.org/ISOC-REM-MBA2187] entered the room. (2:07:49 PM)

2:09:54 PM Szilveszter Nadas: I think that rather wireless networks were designed to work with TCP. There are some things in there just to let TCP work, e.g. RLC AM for LTE, mainly to avoid a 10^3 radio loss, which might be too high for TCP in some cases.

2:09:57 PM Stephen Farrell: did he say for what we need those middleboxes?

2:10:03 PM Blake Matheny: no

2:10:10 PM Blake Matheny: and I don't think we need middleboxes 

2:10:26 PM jari.arkko: Well… it is not black and white. The issue is that if you expose some information you optimize some things a tad better. 

2:11:18 PM Szilveszter Nadas: "If the operator can decrease his cost (and propagates that to users) it is beneficial to everyone"

2:12:07 PM Szilveszter Nadas: overprovisioning is overbuying equipment. If equipment/spectrum is cheap it is of course no problem

2:13:07 PM Stephen Farrell: that's not what I understand - isn't the msisdn the usual thing to add

2:13:55 PM jari.arkko: that arrangement reveals the user, ie. allows tracking. there might be ways to provide identifying information without revealing the user.

2:14:19 PM Stephen Farrell: but the history was adding the msisdn wasn't it?

2:14:24 PM jari.arkko: not that i'm necessarily in favour of adding IDs. i might be in favour of adding some other information (priority/available bandwidth/etc)

2:14:28 PM Stephen Farrell: I hadn't heard it had changed

2:15:07 PM jari.arkko: you keep the ID constant, you will have problems, even if the user's street address or ssn or msisdn is not part of the ID

2:15:51 PM Szilveszter Nadas: 

benoit.claise left the room. (2:16:34 PM)

benoit.claise [benoit.claise@gmail.com/71EEB237] entered the room. (2:16:39 PM)

2:16:43 PM Blake Matheny: header enrichment is too close to supporting lawful intercept for me to feel good about it

benoit.claise left the room. (2:16:53 PM)

benoit.claise [benoit.claise@gmail.com/71EEB237] entered the room. (2:17:31 PM)

2:18:27 PM dvijay@jabber.org: You should not include anything that identifies a cell or identifies the UE - IMSI, MSIDN, IP address, etc…

Kevin left the room. (2:18:31 PM)

Kevin [sirles@jabber.cz/KEVIN-SMITHs-MacBook-Air] entered the room. (2:18:38 PM)

2:18:54 PM Blake Matheny: agree. common approaches today include a part of the phone number 

2:18:55 PM dvijay@jabber.org: What ever is exposed should be just for that session - like bandwidth guidance in the context of the session

2:19:01 PM dvijay@jabber.org: Not about the user

dvijay@jabber.org left the room. (2:20:06 PM)

2:20:33 PM jari.arkko: of course we should not include anything about the UE/user identification. i'm questioning even including other stable identifiers. i'd be ok with session IDs.

Vijay Devarapalli [dvijay@jabber.org/Vijays-MacBook-Pro] entered the room. (2:20:57 PM)

2:20:58 PM wseltzer: any identifiers should be user-clearable and regularly rotated

2:21:22 PM Stephen Farrell: user-clearable isn't useful IMO, isn't it a nice fiction for 99% of users?

2:21:27 PM Natasha: i wonder whether clear-site-data should be adhered to too

2:21:37 PM dvijay@jabber.org: Depends on whether you doing it in-path or out-of-path

2:21:50 PM dvijay@jabber.org: If you do in in-path, you don't see a session id

2:21:52 PM wseltzer: a) it's an option; and b) if it becomes useful, it can be operated by a user-agent

2:21:53 PM jari.arkko: i dont think users would clear anything

2:22:06 PM dvijay@jabber.org: You just embed the information - throughput guidance for example in the session

2:22:15 PM Stephen Farrell: esp. not if browser only has v. coarse grained clearing which is the case esp on phones

2:22:24 PM dvijay@jabber.org: If it is out-of-path, you need a session id to correlate

You have disconnected (2:23:34 PM)

You have connected (2:23:44 PM)

Aaron Falk has set the subject to: IETF Note Well applies to this room (https://www.ietf.org/about/note-well.html) (2:23:44 PM)

2:23:53 PM jari.arkko: Backing away from the ID discussion… I think i agree with Andreas' points on providing additional information to endpoints.

2:24:06 PM Blake Matheny: Why is it needed?

Szilveszter Nadas left the room (Replaced by new connection). (2:24:16 PM)

Szilveszter Nadas [szilveszter.nadas@xmpp.jp/Psi] entered the room. (2:24:27 PM)

2:25:16 PM Stephen Farrell: isn't there a danger here that if someone standardises any way to push this kind of information up, then that will in fact be used to push up long term user-IDs though?

2:25:16 PM Kevin: It can help finesse the congestion controls (per Andreas/our test results on start time)

Karen O'Donoghue left the room (Replaced by new connection). (2:25:46 PM)

Karen O'Donoghue [odonoghue@jabber.isoc.org/ISOC-REM-MBA2187] entered the room. (2:25:57 PM)

2:26:09 PM Szilveszter Nadas: @Kevin: I think that an agent for the user is useful in avoiding that. That agent is really like a firewall and an important piece of security sw.

2:26:11 PM DirkKutscher: Yes, that's a risk

2:26:15 PM jari.arkko: stephen: that is certainly a danger. (and it is also a danger in current http-based traffic, as has been observed from various supercookie cases.)

2:26:35 PM Stephen Farrell: if so, then shouldn't we be doing less, and not more, of it?

2:28:21 PM Blake Matheny: I'd rather not leak anything to a middlebox. Szilveszter we should talk about some of the experiements we've done at FB that relate to the tussle stuff. We've had good success.

2:28:49 PM jari.arkko: i think we need less long-term user IDs. the question is if we can increase sending other type of info without increasing the use of long-term user IDs. needs more work, but maybe there are ways to limit information without exposing that. short bit fields, etc. but don't know if that's feasible in the end.

2:29:20 PM Stephen Farrell: right, that's a tricky one

2:29:52 PM Szilveszter Nadas: @Blake OK

2:30:49 PM Stephen Farrell: @jari: https://tools.ietf.org/html/draft-nottingham-transport-metadata-impact-00#section-3.1 talks about that issue

2:31:57 PM jari.arkko: thanks.

2:36:00 PM Kevin: I'm not in favour of any user identity/user metadata being sent up to the network from the application, or the other way. But where metadata about the network or application service can help content delivery (and not breach privacy) then it's worth testing. 

spencerdawkins left the room. (2:36:35 PM)

2:36:59 PM Stephen Farrell: *wonders if even n/w info would create new fingerprinting possibilities*

ben left the room. (2:38:08 PM)

2:38:22 PM jari.arkko: if improperly done, the answer is probably yes. but in a narrow sense… I think it woiuld also be doable safely.

2:38:33 PM Kevin: good point. certainly if it was cellId or something that hints at location then yes. Per session throughput, hopefully not.

ben [ben@nostrum.com/avalon-air] entered the room. (2:38:48 PM)

2:39:28 PM jari.arkko: point about ted's point: even if you reveal available bandwidth, you should NOT reveal that it is because you run out of money or because base station 1234 has limited capacity or any of the other actual reasons. 

2:41:14 PM dvijay@jabber.org: Yep, agree

2:41:47 PM dvijay@jabber.org: For all you know the throughput is low because there happens to be 50 consuming UEs in a single cell that can only do 20 Mbps at that time

2:42:23 PM Blake Matheny: jari.arkko: this is actually relatively easy to calculate independently. I'd be happy to share some graphs 1:1. I'd rather get the signal explicitly. I can't imagine how this would be bad for the end user, but yes I can see it being bad for the operator.

2:42:57 PM Szilveszter Nadas: +1 on the speakers point on not fixing TCP

Ted.h [hardie@xmpp.rg.net/hardie-macbookpro2] entered the room. (2:43:06 PM)

2:43:31 PM Szilveszter Nadas: I think that if we decrease the responsibility of TCP and let something else solver resource sharing, we can solve much

2:43:59 PM Szilveszter Nadas: (we are doing it often today anyway, like cellular scheduling)

spencerdawkins [spencerdawkins@gmail.com/androidxQTF24E08C6] entered the room. (2:44:44 PM)

2:45:06 PM Kevin: Blake: yes, certainly from my perspective sharing data cap info is business sensitive (plus it could risk leaking user identifiers). Cell info may be, but the session network info is not.

2:47:02 PM Szilveszter Nadas: Yeah, I think that rather the user shall be able to communicate to the app that he prefers lower data user over high QoE. Another use case for an agent of the user to solve.

2:47:42 PM dvijay@jabber.org: Can't reveal cell info

2:48:06 PM dvijay@jabber.org: Just the fact that the user is in a congested cell, but not the cell ID

Kevin left the room. (2:48:13 PM)

2:48:56 PM Stephen Farrell: so who has figured out what is and is not safe? (and including re-identification too); if nobody has, maybe that's a first step?

2:51:10 PM Blake Matheny: cell ID is already revealed to the UE and that information can be accessed if the user grants permission

2:51:31 PM Szilveszter Nadas: Are there universal answers here? Or is it like a firewall sw, which evolves and also there are different possible security levels? Shall a network be allowed to reveal anything without user consent?

2:51:59 PM Szilveszter Nadas: @Blake I think that "user grants permission" is really important there

2:52:04 PM Stephen Farrell: how might a user actually consent to exposing any of this? 

2:52:19 PM Aaron Falk: OT: no more v4 in NA.  https://www.arin.net/announcements/2015/20150924.html

2:52:20 PM Szilveszter Nadas: what do you mean?

2:53:12 PM Stephen Farrell: @szilveszter: were you asking me?

2:53:12 PM Blake Matheny: sftcd: Android (and iOS) have a permission/capability model. If you want access to the cell ID, you can get it, but access to that API will prompt the user saying, "The application is requesting X access, would you like to grant it?"

2:53:22 PM Blake Matheny: X might be voice capabilities, video, geo, etc

2:53:28 PM Stephen Farrell: *hasn't a high opinion of android's permission model*

2:53:59 PM Blake Matheny: bug Andreas 

2:54:12 PM Blake Matheny: I'm just saying this information is already available

2:54:19 PM Ted Hardie: It changed a good bit in M; do you dislike the new one, the old one, or both?

Kevin [sirles@jabber.cz/KEVIN-SMITHs-MacBook-Air] entered the room. (2:54:22 PM)

2:54:26 PM Stephen Farrell: haven't seen new one

2:54:35 PM Blake Matheny: Even if it wasn't, geo is available and isn't going anywhere. It's fairly easy to triangulate if you have enough data.

Natasha left the room. (2:57:06 PM)

2:57:12 PM Kevin: Blake:yes CellID at UE is fine, I just meant the network sharing it downstream risks leakage. 

Natasha [schuki_@xmpp.jp/Bulbasaur] entered the room. (2:57:20 PM)

2:57:27 PM Ted Hardie: It's also the case that shifting congestion controller based on which interface you're connected to can result in fairly surprising things.  For single interface devices (LTE-only) it would easier than managing both highly scheduled and listen-before-speak, especially if you ever want hand-off or multipath.

2:58:32 PM Blake Matheny: Kevin: completely agree. I'm not a fan of sharing _any_ information downstream.

2:58:50 PM Szilveszter Nadas: @Blake +1

2:59:05 PM Szilveszter Nadas: @Ted I do not get your point 

Vijay Devarapalli left the room (This participant is kicked from the room because he sent an error message to another participant: service-unavailable). (2:59:05 PM)

ben left the room. (2:59:46 PM)

ben [ben@nostrum.com/avalon-air] entered the room. (2:59:54 PM)

3:00:09 PM Ted Hardie: @Szilveszter  A WiFi + LTE UE might shift between interfaces; if its tcp stack needs to handle both, it can't assume a highly scheduled network.

3:00:45 PM Szilveszter Nadas: OK

3:02:11 PM Szilveszter Nadas: @Blake setting e.g. ECN is also sharing something downstream, is not it?

3:02:29 PM Blake Matheny: Szilveszter were you thinking downstream == "UE to UTRAN" or "UTRAN to UE"?

3:02:52 PM Blake Matheny: I work on proxies and this term is often overloaded for me 

3:02:59 PM Szilveszter Nadas: No, I was thinking NW to Server

3:03:06 PM Blake Matheny: oh, no way

3:03:11 PM Blake Matheny: ECN I'd be ok with

3:03:22 PM Blake Matheny: But nothing user specific; data plan, UUID, etc

3:03:29 PM Szilveszter Nadas: yeah.

3:03:35 PM Kevin: @Ted Also macro and femtocells on the same LTE network (aka 2-tier) adds complexity

Vijay Devarapalli [dvijay@jabber.org/Vijays-MacBook-Pro] entered the room. (3:03:35 PM)

3:04:48 PM Kevin: @Blake: how about throughout guidance?

3:05:11 PM Blake Matheny: @Kevin I don't think you need it. We've managed to this from UE to Server without the network participating. 

3:05:19 PM Blake Matheny: er, managed to do this

3:05:24 PM Szilveszter Nadas: Yeah it is an interesting question, where is the limit?

3:05:38 PM Szilveszter Nadas: You can have much better slow start with that. 

3:05:51 PM Blake Matheny: We have resumable init cwnd at FB

3:05:54 PM Szilveszter Nadas: *limit of waht is OK to say

3:06:06 PM Blake Matheny: and again, it doesn't require any interaction from the operators

benoit.claise left the room. (3:07:15 PM)

3:08:54 PM Rich Salz: @Blake, what % of your content (by items or by bytes) is video, compared-to text+images?

benoit.claise [benoit.claise@gmail.com/46DE41A9] entered the room. (3:09:02 PM)

3:09:10 PM Rich Salz: and what is the average length of FB video?

3:10:38 PM Blake Matheny: Let me see if I have that handy.

ben left the room. (3:10:42 PM)

ben [ben@nostrum.com/avalon-air] entered the room. (3:11:54 PM)

3:13:01 PM Rich Salz: What I'm implying is that your discrete content units (probably) don't cross base-stations...

3:14:07 PM Rich Salz: And I admit that base-station is at the outer limits of my knowledge of how cells work/deployed

philshere left the room. (3:14:37 PM)

philshere [philshere@gmail.com/AdiumD087BB51] entered the room. (3:16:02 PM)

3:16:20 PM Blake Matheny: richsalz: do you mean subjected to tower handoff?

3:16:31 PM Blake Matheny: (and, video > 40% of traffic)

3:16:56 PM Rich Salz: yes, that's what I meant.

philshere left the room. (3:17:39 PM)

3:17:44 PM Blake Matheny: we actually track that for mobile. how would that happening frequently or infrequently influence the need to supply information to the NW?

3:18:57 PM Rich Salz: not sure, just curious if it really is feasible to do it "without network cooperation"

philshere [philshere@gmail.com/AdiumB0D53869] entered the room. (3:19:34 PM)

3:20:08 PM Blake Matheny: it is at least in the data I have  successful radio handoffs don't impact cwnd greatly and when they do, TCP dynamics do the right thing.

3:20:12 PM Szilveszter Nadas: Also large players like Facebook can do that, but that puts small players at disadvantage.

3:20:26 PM Kevin: The network today manages the handover (pretty quickly in LTE where there is a point-ot-point base station interface). I don't think the NW needs anything from the application which would affect that.

3:20:45 PM dvijay@jabber.org: Majority of the handovers are between sectors in the same cell and between carriers in the same sector

3:20:52 PM dvijay@jabber.org: Not between cell sites

3:21:02 PM dvijay@jabber.org: Each one of the carrier is a cell

3:21:15 PM dvijay@jabber.org: If a cell site has 3 sectors with 3 carriers per sector, you effectively have 9 cells on it

3:21:22 PM dvijay@jabber.org: Each with its capacity

3:21:44 PM dvijay@jabber.org: eNodeBs frequently move users between carriers to balance load

3:22:07 PM dvijay@jabber.org: So with an video session, you can have a number of handovers - most of the intra-cell site

Mary Barnes left the room. (3:22:27 PM)

3:22:30 PM Blake Matheny: Szilveszter I agree. It's not possible for "most" of the internet to have enough telemetry data to do useful things like this. And we can't share the information, besides privacy issues it would piss off carriers. 

3:23:44 PM Szilveszter Nadas: Exactly. But the devices could do the same. Problem is that the user might have an incentive to state a higher initial window than what is "nice".

Mary Barnes [mary.h.barnes@gmail.com/Adium1340E876] entered the room. (3:25:04 PM)

3:25:15 PM Blake Matheny: I think doing the same thing might require bi-directional sharing.

3:25:50 PM Szilveszter Nadas: @Blake please explain bi-deirectional sharing more

russhousley left the room (Replaced by new connection). (3:25:55 PM)

russhousley [russhousley@xmpp.rg.net/Russell-Housleys-MacBook-Pro] entered the room. (3:25:56 PM)

Christian [huitema@nostrum.com/0bf32aa064f14e0d9edbb65db128dedc85beaf77] entered the room. (3:27:34 PM)

3:32:13 PM benoit.claise: Timely message: BCP 200, RFC 1984 on IAB and IESG Statement on Cryptographic Technology and the Internet. 

3:32:38 PM jari.arkko: I'd suggest that we are perhaps too far into the TCP redesign discussion. Strictly speaking that is not the topic of this workshop. Problems with TCP existed before encryption was added.

3:32:49 PM benoit.claise: +1 to Jari

3:34:08 PM barryleiba: Even if things aren't PI, they can become PI when they're aggregated.

3:37:15 PM barryleiba: Yeh, there.

3:37:29 PM Szilveszter Nadas: PI=?

3:37:38 PM barryleiba: personally identifiable

Christian left the room. (3:39:16 PM)

Christian [huitema@nostrum.com/0bf32aa064f14e0d9edbb65db128dedc85beaf77] entered the room. (3:39:27 PM)

Christian left the room. (3:39:54 PM)

Christian [huitema@nostrum.com/0bf32aa064f14e0d9edbb65db128dedc85beaf77] entered the room. (3:40:07 PM)

ben left the room. (3:43:44 PM)

ben [ben@nostrum.com/avalon-air] entered the room. (3:43:49 PM)

Blake Matheny left the room (Disconnected: closed). (3:44:57 PM)

Blake Matheny [bmatheny@jabber.hot-chilli.net/oakcombs] entered the room. (3:45:00 PM)

Vijay Devarapalli left the room. (3:46:48 PM)

ben left the room. (3:47:14 PM)

Kevin left the room. (3:47:20 PM)

You have disconnected (3:49:04 PM)

You have connected (4:14:59 PM)

Aaron Falk has set the subject to: IETF Note Well applies to this room (https://www.ietf.org/about/note-well.html) (4:15:00 PM)

hildjj [hildjj@jabber.org/JHILDEBR-M-N3ZF] entered the room. (4:15:02 PM)

wseltzer [wseltzer@jabber.org/67839cd92f160ca5] entered the room. (4:15:11 PM)

Karen O'Donoghue [odonoghue@jabber.isoc.org/ISOC-REM-MBA2187] entered the room. (4:15:29 PM)

Christian [huitema@nostrum.com/0bf32aa064f14e0d9edbb65db128dedc85beaf77] entered the room. (4:15:38 PM)

sftcd left the room. (4:15:48 PM)

Christian left the room. (4:16:00 PM)

sftcd [sftcd@jabber.org/34d24a470fac8a73] entered the room. (4:16:09 PM)

Christian [huitema@nostrum.com/0bf32aa064f14e0d9edbb65db128dedc85beaf77] entered the room. (4:16:12 PM)

Vijay Devarapalli [dvijay@jabber.org/Vijays-MacBook-Pro] entered the room. (4:16:52 PM)

benoit.claise left the room. (4:18:32 PM)

spencerdawkins left the room. (4:21:16 PM)

4:21:59 PM Rich Salz:  On PII integration "I know why you went to the clinic: Risks and realization of HTTPS traffic analysis" (2014) https://www.petsymposium.org/2014/papers/Miller.pdf

4:23:05 PM Ted Hardie: I guess a basic question here is whether we are trying to be significantly better than the current solution, or just matching its effectiveness.  Does the current DPI-to-network-pattern method provide a level of effectiveness equivalent to throughput sharing?  Is it better or worse?

Mary Barnes [mary.h.barnes@gmail.com/Adium016BC79C] entered the room. (4:23:43 PM)

4:24:07 PM Szilveszter Nadas: could you detail "eq. to throughput sharing"? I do not get it.

4:25:37 PM Ted Hardie: @Szilveszter, I just mean if we're replacing management method FOO with BAR, are we trying to make BAR better, or is it okay if it is just as good as FOO, but works in an encrypted world.

Alissa Cooper [coop.ietf@gmail.com/AdiumF157EBE0] entered the room. (4:25:48 PM)

4:26:23 PM Szilveszter Nadas: I think that it should be better. Main reason being that the user knows what he wants and communicates what he wants instead of what he is doing.

4:26:41 PM Szilveszter Nadas: May replace user to OTT if OTT pays, though that works better today.

4:27:11 PM Szilveszter Nadas: It is rare that anyone asks the user today. Even with good intentions it is hard to guess what the user wants.

ihlar [ihlar@alpha-labs.net/jwchat] entered the room. (4:27:39 PM)

4:28:03 PM Aaron Falk: In terms of performance, it's applications more than users that know what they want.

ihlar left the room. (4:29:37 PM)

4:30:25 PM Szilveszter Nadas: Not sue that the users wants the same. I think that all communication shall have a consequence and the consequence if for the paying party who is the user. So the app can propose something to the user's agent, but the user shall approve.

Mary Barnes left the room. (4:32:05 PM)

benoit.claise [benoit.claise@gmail.com/266F5B1D] entered the room. (4:32:15 PM)

4:32:16 PM Ted Hardie: What is an FMSS, in this slide context?

Mary Barnes [mary.h.barnes@gmail.com/Adium016BC79C] entered the room. (4:32:20 PM)

Kathleen [kathleen.moriarty@jabber.org/Kathleens-MacBook-Air] entered the room. (4:32:23 PM)

4:32:27 PM Szilveszter Nadas: Form a different perspective: if it costs the app nothing to want more, it might say more please, even if it has good intentions.

4:32:57 PM Blake Matheny: ^^ +1

4:33:28 PM Aaron Falk: Frequency Modulation Subcarrier Service?

spencerdawkins [spencerdawkins@gmail.com/androidxQT8B2D6FBB] entered the room. (4:33:49 PM)

4:33:56 PM Ted Hardie: @Szilveszter  That goes back to the discussion we had earlier. If you have a single axis ("faster" or "more"), you have to have an economic incentive.  If it is more balanced,  ("shallow queue, so faster but more drops"), you may be able to deploy without changing the billing model

4:34:06 PM Ted Hardie: Thanks, Aaron

4:34:25 PM Aaron Falk: (Google is your friend  )

4:35:06 PM Ted Hardie: @Aaron, indeed so.

4:35:12 PM Szilveszter Nadas: @Ted right. There might be cases when there is no incentive to lie. Your example is such a case. 

4:35:33 PM Szilveszter Nadas: No need for incentive there.

4:35:46 PM Ted Hardie: @Szilveszter  This is why the easiest marking to trust is scavenger class—there is no incentive to lie, so it can be trusted.

4:35:49 PM Szilveszter Nadas: Except for the NW operator to offer and implement this.

4:36:33 PM Szilveszter Nadas: @Ted: but also in mobile often there is no incentive to use it, because there might not be economic benefits.

4:36:48 PM Szilveszter Nadas: Except not starving you other parallel flows

4:37:09 PM Ted Hardie: @Szilveszter Because it can be trusted, it likely won't be bleached; that means that the incentive may be outside the RAN.

spencerdawkins left the room. (4:38:05 PM)

Mary Barnes left the room. (4:38:49 PM)

spencerdawkins [spencerdawkins@gmail.com/androidxQT23FD77EA] entered the room. (4:40:19 PM)

Mary Barnes [mary.h.barnes@gmail.com/Adium63695CF8] entered the room. (4:40:30 PM)

spencerdawkins left the room. (4:43:21 PM)

spencerdawkins [spencerdawkins@gmail.com/androidxQTEB88C33D] entered the room. (4:43:32 PM)

Mary Barnes left the room. (4:45:05 PM)

Mary Barnes [mary.h.barnes@gmail.com/Adium2690A4EA] entered the room. (4:47:59 PM)

4:54:56 PM Szilveszter Nadas: Low latency and AQM - that looks pretty manageable for fixed . For wireless there is a opportunity for better channel if we can wait. Which can be used for less latency sensitive flows.

Christian left the room. (4:59:00 PM)

wseltzer left the room. (5:07:19 PM)

benoit.claise left the room. (5:12:36 PM)

benoit.claise [benoit.claise@gmail.com/266F5B1D] entered the room. (5:12:41 PM)

5:13:59 PM Natasha:  Line is cut

5:14:54 PM benoit.claise: relationship? Like on FB: complicated 

Vijay Devarapalli left the room. (5:18:19 PM)

Vijay Devarapalli [dvijay@jabber.org/Vijays-MacBook-Pro] entered the room. (5:21:49 PM)

Kathleen left the room. (5:22:19 PM)

Kathleen [kathleen.moriarty@jabber.org/Kathleens-MacBook-Air] entered the room. (5:25:40 PM)

DirkKutscher left the room. (5:30:30 PM)
