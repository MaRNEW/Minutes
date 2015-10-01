
Aaron Falk has set the subject to: IETF Note Well applies to this room

 (https://www.ietf.org/about/note-well.html) 

 (9:05:36 AM)Aaron Falk: Good morning!jari.arkko left the room

 (This participant is kicked from the room because he sent an error message to another participant: service-unavailable).

 (9:05:44 AM)Ted Hardie: Good morning, Aaron!Aaron Falk: TCP TCP TCP TCP TCP TCP TCP TCP TCP TCP TCP TCPhildjj [hildjj@jabber.org/JHILDEBR-M-N3ZF] entered the room.

 (9:06:43 AM)Karen O'Donoghue [odonoghue@jabber.isoc.org/ISOC-REM-MBA2187] entered the room.

 (9:06:54 AM)wseltzer [wseltzer@jabber.org/95ba7c5ee85e99d5] entered the room.

 (9:07:12 AM)ben [ben@nostrum.com/avalon-air] entered the room.

 (9:07:16 AM)Aaron Falk: sorry, wrong room.  Olaf Kolkman [kolkman@jabber.isoc.org/Dropje] entered the room.

 (9:07:32 AM)Aaron Falk: *looks for bad-attitude...*mcmanus [mcmanus@jabber.org/413740a34beeb14c] entered the room.

 (9:07:35 AM)Olaf Kolkman: The second Chatham House rule: Remind people who use plural that there is only one rule.ihlar [ihlar@alpha-labs.net/jwchat] entered the room.

 (9:08:58 AM)jari.arkko [jari.arkko@gmail.com/AdiumC83F931C] entered the room.

 (9:09:28 AM)Joe Hildebrand: https://www.chathamhouse.org/about/chatham-house-rule/translationsNatasha [schuki_@xmpp.jp/Bulbasaur] entered the room.

 (9:10:07 AM)ihlar left the room.

 (9:10:57 AM)jari.arkko left the room.

 (9:11:24 AM)wseltzer left the room.

 (9:11:26 AM)wseltzer [wseltzer@jabber.org/063c1fcef1bf2fd6] entered the room.

 (9:11:45 AM)Jari Arkko [jariarkko@jabber.org/Jaris-MacBook-Pro] entered the room.

 (9:11:59 AM)Natasha: lolmcmanus: https://httpworkshop.github.io/workshop/presentations/thomson-cache.pdfbenoit.claise [benoit.claise@gmail.com/54711855] entered the room.

 (9:13:56 AM)Joe Hildebrand: https://tools.ietf.org/html/draft-hildebrand-middlebox-erosion-01wseltzer: and that's why Netflix doesn't ask us to pay for their videos, right?Szilveszter Nadas: ￼Szilveszter Nadas: I think the issue is not paying, it is how simple a payment mode is.Szilveszter Nadas: *modelTed Hardie: It's an interesting conflict.  If adaptive streaming can give you HD in some spot, you burn through cap faster, but the trade-off in resolution vs. resource utilization is opaque to the user, who has no idea what the HD vs. SD balance is.Jari Arkko: yeah, i think there will always be "big pipe" and "small pipe" pricing. in finland there are generally no data caps, but there are different account types. i don't see that as being harmful, and it is still relatively simple to understand by the users. despite the difficulty of estimating gigabytes. and I think it is certainly better than some more fine grained per-session pricing.DirkKutscher left the room.

 (9:24:23 AM)DirkKutscher [kutscher@jabber.neclab.eu/2920066018144318758941263] entered the room.

 (9:26:34 AM)wseltzer: does anyone understand that example?wseltzer: "sites that don't use CDNs are malicious?"Blake Matheny left the room

 (This participant is kicked from the room because he sent an error message to another participant: service-unavailable).

 (9:44:26 AM)Aaron Falk: Wendy: I *think* that is a criticism of transparent caches.Ted Hardie: Is there a privacy analysis of named data networking floating around anywhere?Aaron Falk: I know it is a concern they are aware of.  I've asked folks about it and was told there is a story.Ted Hardie: Google returns things like this: http://named-data.net/publications/cache_privacy-icdcs13/ but nothing comprehensive.Aaron Falk: Ask Dirk.Ted Hardie: @Dirk, ping?Kathleen left the room.

 (9:55:27 AM)Kathleen [kathleen.moriarty@jabber.org/Kathleens-MacBook-Air] entered the room.

 (9:59:34 AM)DirkKutscher: There has been some work on anonymity preservation, and Mark Stapp has started a discussion in ICNRG around ICN privacy.Ted Hardie: Thanks for the pointer Dirk; I'll look for his work.Natasha: thank-you @Jari Arkko!ihlar [ihlar@alpha-labs.net/jwchat] entered the room.

 (10:00:29 AM)Natasha: that was the point i wanted someone to makeDirkKutscher: http://www.ccnx.org/pubs/private-communication-ccnx-2015.pdfDirkKutscher: http://conferences.sigcomm.org/sigcomm/2011/papers/icn/p19.pdfYou have disconnected

 (10:02:17 AM)You have connected

 (10:08:34 AM)Aaron Falk has set the subject to: IETF Note Well applies to this room

 (https://www.ietf.org/about/note-well.html)

 (10:08:34 AM)richsalz left the room.

 (10:08:35 AM)richsalz [richsalz@jabber.at/@Work] entered the room.

 (10:08:37 AM)ben left the room.

 (10:09:30 AM)richsalz left the room.

 (10:14:09 AM)ben [ben@nostrum.com/avalon-air] entered the room.

 (10:15:46 AM)Jari Arkko: i missed mark Watson's one point. What was it?ben: Is mark the person next to salvatore?barryleiba: yesben: He talked about a 1 bit bandwidth vs latency tradeoffben:

 (iiuc)DirkKutscher: the point was about mechanism to control latency/bw tradeoffsphilshere left the room.

 (10:25:13 AM)russhousley left the room.

 (10:26:50 AM)russhousley [russhousley@xmpp.rg.net/Russell-Housleys-MacBook-Pro] entered the room.

 (10:26:54 AM)Jari Arkko: what kinds of metrics is he talking about?philshere [philshere@gmail.com/AdiumDBF9780D] entered the room.

 (10:27:19 AM)Ted Hardie: Mark also wanted the single bit to be re-settable during the flow, so that a flow that was latency sensitive to push to bandwidth over latency

 (useful for streaming video, but a big piece of http/2 multiplexing over time) Blake Matheny [bmatheny@jabber.hot-chilli.net/oakcombs] entered the room.

 (10:36:08 AM)Ted.h left the room.

 (10:36:09 AM)Karen O'Donoghue left the room.

 (10:36:24 AM)Kathleen left the room.

 (10:36:28 AM)ben left the room.

 (10:37:03 AM)You have disconnected

 (10:37:15 AM)You have connected

 (12:29:13 PM)Blake Matheny: FWIW I'm not sure how feasible anonymous

 (privacy preserving) caches are, but I think that would be a requirementSzilveszter Nadas: What were the two proposals Jana said?barryleiba: sprout and pccSzilveszter Nadas: thxbarryleiba:

 (for the record)Szilveszter Nadas: http://alfalfa.mit.edu/
http://modong.github.io/pcc-page/

Ted.h: I don't think they need to know it is a browser session; that's the point I was making.  They don't need know that it's a javascript app in a webkit framework—they need to know what network treatment is desired.Jari Arkko: Can we get past this there-is-a-problem-there-is-no-problem? it seems logical that no matter what we are doing, being able to multiplex traffic in a smart fashion onto a finite resource is better than a random multiplexing.Ted.h: That's what they will changedvijay@jabber.org: Agree Jaridvijay@jabber.org: But I am not sure everyone sees the problemdvijay@jabber.org: I meant everyone on the panelJari Arkko: can I get more information about what the zero bit solution would be, and how would that impact the 3GPP architecture? not trying to make an argument, I'm just trying to understand.dvijay@jabber.org: Getting tired of the current discussionJari Arkko: yeah. we're not all yet seeing the issue. again, the point is, if you have demand >> capacity

 (and we do), it is a good idea to optimise resource usage. while of course being fair across users.Jari Arkko: jana has a point in that we need to start from the high level requirement

 (optimise resource alloc) rather than a solution

 (classification).  but if we need data, it should not be about proving that there's an "issue". It would be much more helpful to find data that helps differentiate alternative solutions, for instance.wseltzer: and encryption helps to assure that all parties whose resources are being allocated are necessary participants in their allocationSzilveszter Nadas: I believe that at the end of the day the gain with dynamic

 (non-equal among users) resource allocation is higher than the loss with its complexity. It does not seem that we have a consensus about this. Jari Arkko: i'd argue it would be helpful to have a header in QUIC that can carry some simple ￼ bits) information.Szilveszter Nadas: What data can help in deciding this?Aaron Falk has set the subject to: IETF Note Well applies to this room

 (https://www.ietf.org/about/note-well.html)

 (12:29:13 PM)Kathleen left the room.

 (12:29:30 PM)Vijay Devarapalli left the room.

 (12:29:30 PM)ben left the room.

 (12:34:29 PM)Christian left the room.

 (12:40:34 PM)You have disconnected

 (12:40:38 PM)You have connected

 (1:02:06 PM)Aaron Falk has set the subject to: IETF Note Well applies to this room

 (https://www.ietf.org/about/note-well.html)

 (1:02:06 PM)Vijay Devarapalli left the room.

 (1:03:30 PM)russhousley [russhousley@xmpp.rg.net/Russell-Housleys-MacBook-Pro] entered the room.

 (1:06:00 PM)wseltzer [wseltzer@jabber.org/73e38e3ba7f513a2] entered the room.

 (1:08:46 PM)russhousley left the room

 (Replaced by new connection).

 (1:09:07 PM)Alissa Cooper [coop.ietf@gmail.com/Adium26628E28] entered the room.

 (1:09:07 PM)russhousley [russhousley@xmpp.rg.net/Russell-Housleys-MacBook-Pro] entered the room.

 (1:09:08 PM)Vijay Devarapalli [dvijay@jabber.org/Vijays-MacBook-Pro] entered the room.

 (1:09:40 PM)ben [ben@nostrum.com/avalon-air] entered the room.

 (1:10:23 PM)You have disconnected

 (1:18:03 PM)You have connected

 (1:27:28 PM)Aaron Falk has set the subject to: IETF Note Well applies to this room

 (https://www.ietf.org/about/note-well.html)

 (1:27:28 PM)ben [ben@nostrum.com/avalon-air] entered the room.

 (1:27:30 PM)Vijay Devarapalli left the room.

 (1:28:30 PM)ben left the room.

 (1:29:26 PM)Karen O'Donoghue [odonoghue@jabber.isoc.org/ISOC-REM-MBA2187] entered the room.

 (1:29:29 PM)hildjj [hildjj@jabber.org/JHILDEBR-M-N3ZF] entered the room.

 (1:29:43 PM)Vijay Devarapalli [dvijay@jabber.org/Vijays-MacBook-Pro] entered the room.

 (1:29:49 PM)mcmanus [mcmanus@jabber.org/efefcc7d2e8d3227] entered the room.

 (1:30:14 PM)Mary Barnes left the room.

 (1:31:09 PM)Mary Barnes [mary.h.barnes@gmail.com/AdiumB798D79D] entered the room.

 (1:31:13 PM)Christian [huitema@nostrum.com/b169d1a3d414265bd928c1e8915eb67ac8ba64c0] entered the room.

 (1:31:39 PM)Ted.h [hardie@xmpp.rg.net/hardie-macbookpro2] entered the room.

 (1:33:20 PM)ben [ben@nostrum.com/avalon-air] entered the room.

 (1:34:18 PM)ihlar [ihlar@alpha-labs.net/jwchat] entered the room.

 (1:38:12 PM)ihlar left the room.

 (1:40:11 PM)Vijay Devarapalli left the room.

 (1:48:30 PM)ihlar [ihlar@alpha-labs.net/jwchat] entered the room.

 (1:51:17 PM)ihlar left the room.

 (1:53:16 PM)ihlar [ihlar@alpha-labs.net/jwchat] entered the room.

 (1:53:35 PM)ihlar left the room.

 (1:55:35 PM)Vijay Devarapalli [dvijay@jabber.org/Vijays-MacBook-Pro] entered the room.

 (2:03:16 PM)philshere left the room.

 (2:26:26 PM)Christian left the room.

 (2:28:10 PM)Vijay Devarapalli left the room.

 (2:31:00 PM)Olaf Kolkman left the room.

 (2:31:01 PM)Vijay Devarapalli [dvijay@jabber.org/Vijays-MacBook-Pro] entered the room.

 (2:31:32 PM)Vijay Devarapalli left the room.

 (2:32:00 PM)ben left the room.

 (2:36:28 PM)Christian [huitema@nostrum.com/b169d1a3d414265bd928c1e8915eb67ac8ba64c0] entered the room.

 (2:37:01 PM)Christian left the room.

 (2:37:27 PM)Christian [huitema@nostrum.com/b169d1a3d414265bd928c1e8915eb67ac8ba64c0] entered the room.

 (2:37:41 PM)ben [ben@nostrum.com/avalon-air] entered the room.

 (2:39:39 PM)wseltzer left the room.

 (2:43:31 PM)Ted.h left the room.

 (2:43:54 PM)Vijay Devarapalli [dvijay@jabber.org/Vijays-MacBook-Pro] entered the room.

 (2:44:25 PM)Kathleen left the room.

 (2:44:30 PM)Mary Barnes left the room.

 (2:47:55 PM)Kathleen [kathleen.moriarty@jabber.org/Kathleens-MacBook-Air] entered the room.

 (2:48:20 PM)Olaf Kolkman [kolkman@jabber.isoc.org/Dropje] entered the room.

 (2:48:27 PM)Mary Barnes [mary.h.barnes@gmail.com/AdiumEEA97283] entered the room.

 (2:48:53 PM)spencerdawkins left the room.

 (2:49:21 PM)spencerdawkins [spencerdawkins@gmail.com/androidxQTCFE2FAD4] entered the room.

 (2:49:22 PM)spencerdawkins left the room.

 (2:50:33 PM)spencerdawkins [spencerdawkins@gmail.com/androidxQT4E3D55E4] entered the room.

 (2:50:33 PM)Vijay Devarapalli left the room.

 (2:52:31 PM)spencerdawkins left the room.

 (2:52:53 PM)spencerdawkins [spencerdawkins@gmail.com/androidxQT04361021] entered the room.

 (2:52:53 PM)You have disconnected

 (2:58:58 PM)You have connected

 (2:59:51 PM)Aaron Falk has set the subject to: IETF Note Well applies to this room

 (https://www.ietf.org/about/note-well.html)

 (2:59:51 PM)Vijay Devarapalli [dvijay@jabber.org/Vijays-MacBook-Pro] entered the room.

 (3:02:20 PM)Karen O'Donoghue left the room.

 (3:08:14 PM)Vijay Devarapalli left the room.

 (3:09:30 PM)You have disconnected

 (3:14:37 PM)You have connected

 (3:22:18 PM)Aaron Falk has set the subject to: IETF Note Well applies to this room

 (https://www.ietf.org/about/note-well.html)

 (3:22:18 PM)Vijay Devarapalli [dvijay@jabber.org/Vijays-MacBook-Pro] entered the room.

 (3:29:27 PM)Vijay Devarapalli left the room.

 (3:31:00 PM)You have disconnected

 (3:33:13 PM)You have connected

 (3:37:33 PM)Aaron Falk has set the subject to: IETF Note Well applies to this room

 (https://www.ietf.org/about/note-well.html)

 (3:37:33 PM)ben [ben@nostrum.com/avalon-air] entered the room.

 (3:41:18 PM)Mary Barnes left the room.

 (3:45:28 PM)russhousley left the room.

 (3:48:05 PM)Christian left the room.

 (3:49:05 PM)Ted.h [hardie@xmpp.rg.net/hardie-macbookpro2] entered the room.

 (3:50:53 PM)hildjj left the room.

 (3:51:00 PM)hildjj [hildjj@jabber.org/JHILDEBR-M-N3ZF] entered the room.

 (3:51:18 PM)ben left the room.

 (3:51:58 PM)ben [ben@nostrum.com/avalon-air] entered the room.

 (3:52:48 PM)philshere [philshere@gmail.com/AdiumA07C9146] entered the room.

 (3:54:06 PM)You have disconnected

 (3:56:44 PM)You have connected

 (3:58:41 PM)Aaron Falk has set the subject to: IETF Note Well applies to this room

 (https://www.ietf.org/about/note-well.html)

 (3:58:41 PM)russhousley [russhousley@xmpp.rg.net/Russell-Housleys-MacBook-Pro] entered the room.

 (4:00:11 PM)Mary Barnes [mary.h.barnes@gmail.com/AdiumA9B29FCA] entered the room.

 (4:00:14 PM)Kathleen [kathleen.moriarty@jabber.org/Kathleens-MacBook-Air] entered the room.

 (4:00:17 PM)Jari Arkko: This is my summary of what I saw in the workshop:russhousley left the room.

 (4:00:45 PM)Jari Arkko: MAIN OBSERVATIONS
- The world does not end when there's more encryption, but some current
   solutions may need to change to work better with encrypted traffic
- The problem is not just about enryption, the issue is how do we 
   optimise customer experience across a number of players?
- Identified a number of potential technical items to pursue in the short-term
- Co-operative resource management ideas gained a lot of interest in the workshop,
   along some other ideas
- 5G is an opportunity to do things better, together, more long-term


TECHNICAL ITEMS TO PURSUE
- Develop co-operative resource management by sending
   data up or down

 (very little)
- Create a new protocol for keyless SSL to make distributed CDN deployments easier
- Make other CDN improvements

 (CDNI, blind caches, certs, et.)
- Build better testing and debugging tools
- On the 3GPP/GSMA side, I know I am interested in identity privacy and dealing with
   the NSA theft of SIM card secrets, but that's not an IETF activity.


IMMEDIATE ACTIONS
- Develop ideas on what information would be useful in Kevin's data, 
   use the marnew list, no need to wait for IETF meetings
- CROWN as a BOF in BA on co-operative resource management
- Create a new working group for Keyless SSL, start by creating a mailing list,
   plan to have the WG in place

 (probably no BOF needed) in BA
- TBD actions for other CDN improvements
- TBD actions for testing and debuggingrusshousley [russhousley@xmpp.rg.net/Russell-Housleys-MacBook-Pro] entered the room.

 (4:00:54 PM)Vijay Devarapalli [dvijay@jabber.org/Vijays-MacBook-Pro] entered the room.

 (4:02:39 PM)Vijay Devarapalli left the room.

 (4:03:31 PM)Alissa Cooper left the room.

 (4:06:06 PM)Alissa Cooper [coop.ietf@gmail.com/Adium99FF39AD] entered the room.

 (4:06:13 PM)Alissa Cooper left the room.

 (4:06:16 PM)Alissa Cooper [coop.ietf@gmail.com/Adium6B88387E] entered the room.

 (4:06:23 PM)ben left the room.

 (4:08:12 PM)
