## Session 1: Encryption Deployment Considerations
 
Chair: Kathleen 

Panelist: Kevin Smith
 
Kathleen explained she and Kevin working on IETF documentation.
 
The Effect of Ubiquitous encryption document - purpose to collect from players, the increased use of sessions in the Internet.
* increased encryption impact
* collection of current security and network management function impact
* Main purpose is what is needed for technical solution. What is the impact of not having access to metadata collecting the impacts.
* Kevin is explaining in his document more about solutions.
 
Kathleen explained the draft content on a high level.
* Introduction: Issue 1 was encryption was blocked due to operational issues. This was driven mainly for commercial perspectives. 
* Middle-box monitoring: traffic interception and pattern matching such as
     * fingerprinting
     * traffic surveys
     * deep packet inspection
     * data compression gateways
* Performance management and troubleshooting:
* Encryption in hosted SP environments:
* management access
* hosted applications
* access control management (2 tuple or 5 tuple monitoring and filtering) 
* It could be any system such as data-centre etc.
 
Comments:
* Christian (Microsoft) it would be great to consider different business environment such as Microsoft Azure etc.
* Dirk (NEC) - good example is operator cloud. Service chaining could be a good scope to include in the draft. Kathleen encouraged Dirk to make a proposal for adding this into he document.
* Spencer Dawkins (Huawei) -  it would be great if the transport people can understand what has been promised in RAN. 
* Mobile specific case has been identified. Kathleen confirmed Natasha was working with GSMA to include some radio network specific content added to the document.
* This document is not specific to mobile, hence why GSMA provided more generic mobile content to this draft.
 
Data storage:
 
Incident monitoring:

* is going to more difficult. Concern was about more limited access to hosted domain names as an example, based on the outcome from the workshop was held earlier in IETF. Deprive 
* Malware detection has been mentioned by Stephen, but URLs are used for malware protection. Malicious URLs are managed centrally and used by browser vendors. It provides end to end protection for users.
* Issues are that these URLs repositories are categorised for industries and they work in silos. 
* It can be more done in this space.
 
Comments:
* Ted Hardy (Google) do we have a sense for incident monitoring service block TLS for deprive to dedicated port?
* Kathleen explained encryption will increase security but there is monetary  motivation behind selling boxes for preventing security attacks. If connections are secure and hard to compromise the server.
* We cannot add new boxes to the network every time we have a new attack. In terms of DNS some vendors will block traffic and separate TLS port for example.
 
Summary:
* more contribution is welcomed from the team.
* some problems cannot be solved, so don't focus on those and move on.
 
Kevin presented the draft for Network management of encrypted traffic and offer some solutions.
* It may pose challenges to network operators.
* Kevin explained this is a working draft and encouraged the team to review the content and provide feedback.
* This is a very mobile centric document including broad range of topics such as 
* network management functions
* flow information visible to network
* inferred flow information
* providing hints to and from the network
* in the solution section there are effort summarised to provide some technical solutions.
 
Comments:
* Stephen - figure out traffic types via 5-tuple, could this told at app layer. Has it been compared with heuristics versus what the apps is.
* Kevin confirmed that they  compared heuristics and applications doing. 
* AP - adding to compare heuristics with real application behaviour / real traffic types
* Dirk - heuristic is best effort based, QCI in LTE is a good mechanism. 
* Kevin when the terminal switches form IDLE state we can look at in 3GPP.
* Joe H - DCSP marking and traffic analysis can be incentive to make heuristic more precise.
* Jana - load of papers focused on QoE for improving network management function which is not listed in our document. Operators summary on network management.
* Kathleen - no we are not covering it yet. Kevin is providing solutions in the document compared to summary.
* Kevin - QoE it is throughout the proposals, we can improve the content in the document.
* Jana - queue management (AQM) is not listed in the solution space in more detail.
* Kevin - please make sure the team can provide contribution to enhance content on AQM
* Humberto - eNodeB is controlling radio resources and its trusted and it can be idea for MTG which ideas could suggest to have single trusted domain. Mobile device and network could be 
* Kevin - this is a good suggestion to 3GPP to follow up.
* Dirk - what is the relationship and interop with transport protocols, congestion control etc. It can impact performance eNodeB resource control, DSCP is great and needs expanding int he document.
* Spencer - TCP over satellite has been done years ago. We need to focus on wireless and how much really? IETF need to understand wireless and what 3GPP is not covering and include some fix line specifics in the document as a long term objective.
* Jana - E2E congestion control mechanism is generally speaking missing out from the document which could be considered adding.
* TCP is cumbersome and we need to mindful of that.
* Kathleen, congestion control is covered but we would like to make sure this area is covered. Jana could take a look at the document and provide feedback.
* Andreas - new QCI requires a new bearer, which needs to spelled out from 3GPP point of view. 
* Mark (Netflix) - there is no need for a real time mechanism, suggested to provide reviews and comments on 3GPP perspective for real-time traffic type information
* Christian - shall we differentiate applications it doesn't matter user experience. We have to differentiate between capacity and quality of content. Radio networks are different based on Microsoft research, because of radio conditions, which has impact on transmission.
* Kevin - different content types have different characteristics have impact on QoE. It does matter 
* Christian - cell handover creates an event in the transmission chain which is not modelled in the TCP chain. We can include in the document about hints and the data models for the hints we can add.
* Kevin - we not sure we can include in the current scope of the document.
* Vijay - not all the bits are equal 
