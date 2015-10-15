## Minutes: Session 7 Technical Analysis and Response to Potential Regulatory Reaction
* Date: 25th September
* Time: 11:00 - 12:30
* Chair: Barry Leiba
* Minute Taker: Istvan Lajtos
* Panel:
  * Kevin Smith (VFE)
  * Olaf Kollkman (IAB)
  * Diego Lopez (TEF)
  * Russ Housley (IAB)

### Chatham House Rule
This session is conducted under Chatham House Rule. Joe provided a heads-up on the rule, it means recording will be turned off. Anything mentioned here, it will not be attributed to the individual. 

All minutes will be taken without individuals names.

### Introduction to Session
* Purpose of the session is to talk about regulatory and policy sessions. 
* Mobile network regulations was explained. Mobile networks are regulated, non-compliance is not an option. There is also a cost involved related to regulations.
* There are different regulation of content such as
 * court order
 * adult content filtering (examples like all SIM cards are treated as child SIM cards, hence validation is required for adult content access)
 * internet watch foundation list (Interpol list - operators have no visibility of these lists)
* Lawful intercept - typically implemented in ETSI LI, operators are perceived as mere conduit. Operators are not expected to provide cleartext to regulators.
* Encryption and Net neutrality
 * Encryption has impact on adult content filters for mixed content sites, could affect court order block if the domain is not visible; 
 * operators are not expected decrypt encrypted content.
 * Net-neutrality: where interpreted as no filters, legislation needed to override. affect the opt in because of net neutrality
* Comments made about collaborative management such as throughput-guidance, operators are regulated and the internet community is not aware of that or regulated in the same fashion.
* In Europe, operators are highly regulated because of mainly privacy regulations. The other example is South America. Regarding net neutrality, all the packets on the networks has to be prioritised in the same way.
* Operators cannot deploy services without being complaint to these regulations. There has been an issue in the NFV working group where a work item had to be rescheduled because lawful intercept obligations.
* IETF has a different experience on regulations compared to GSMA. The fact is regulators ignored each other in IETF in the past.
* It is changing now, first group is communication working group for emergency services, second WAS television white space for data, third one STIR authenticating the source in a VoIP environment.
* Regulators have interest in public security. We also know it is interpreted in different ways in different parts of the world. Encryption clearly has an impact on law enforcement. Some content is set to be illegal and those are removed based on URL screening.
* In Wikipedia for example articles were encrypted, in Russia. It is a concern for this fragmenting the Internet.
* We discussed earlier on about middle boxes, to collect and share metadata, who can access these data.
* Law enforcement is certainly limiting
* The other aspect is net neutrality and same resources for everyone. There are optimisers exist on the Internet but who has access to these boxes, which can open up questions about a new net neutrality regulations.
* Transparent caches are on the radar, especially for emerging market. In those markets, spam is driving loads of traffic. There is a question again how these debates end up, regarding regulations.

### Discussion
* How serious regulators are for example about parental control? Examples are such as those filters can easily be bypassed, there are many ways to avoid these filters.
* We need to qualify / quantify seriousness. In countries, such the UK it can cause serious implications such as service license revocation etc.
* Governments would like to avoid, children accessing adult content, hence they are keen to encourage filters to be used on fixed and mobile networks.
* The issues also are around individual freedom, we should facilitate and the technology to allow for the users to have choices to limit content access. It has to be accessible for all the users and not considered as a premium service.
* Policy regulations at different levels, individual level, government level etc. We have not covered business  impact of encryption related to regulations. Business have different regulations which can be in-line or different to the two mentioned above.
* Parental control is always going to be wrong, because we need fix it. We cannot rely on a simple filtering which can be wrong.
* How do regulators respond for encrypted content or encrypted SNI etc., how are they going to comply.
* Regulators asking for data patterns but if they cannot get the necessary details, they will approach the content sources.
* There is also different expectations related to regulations between different regions, countries and operators.
* In case customers moving operators then it is an obligation to move their data accordingly. Regulators are reflecting the free will of the society.
* What regulators do, for example restrict encryption that would be in the main headlines. It would force regulators to, in an example of having an SNI encrypted, to come and join our discussions.
* European regulators are aware of the impact of encryption and willing to checksum measures.
* We as technologist can at least, developed a solution which can be switched off.
* Governments have their ability to request information on encrypted traffic they want to have access to.
* What we are doing here, developing a solution which helps to manage this solution, how does this effect what we do here.
* This is a crystal ball exercise, we can a technical and policy debates about this issue. These type of discussion are coming our way, specifically IETF areas could be compromised for deployment as an example.
* Access to all data is not scalable or sensible, as stated before. Whatsapp example was mentioned, which was providing clear access to regulators. To date operators have access to law enforcement today, internet players may consider the same thing.
* Law enforcement can look at other means to access to the data, without impacting technological areas. It should also be attractive to operators. Not being able to provide to information due to encryption, operators could clearly state information cannot be provided and law enforcement could go after to content sources.
* China has one of the strictest regulatory rules, it’s non-negotiable hence it is very little can be done. There are no alternatives to bypass these hence businesses cannot operate without being compliant.
* There are technical solutions can be considered, how it could be fulfilled because it has commercial impact. Regulations has to be dealt regionally.
* Personal tracking on cellular network happens, there is no effort to block it by operators. It can be considered a technical standard.
* Operators are not doing it because there is no demand for it, for allowing to block personal tracking.
* Examples were mentioned about social demand.
* Session was mentioned to be dealing with answering the question about regulations. Do operators have enough to take back to the regulators and has any tries been taken.
* Engagement with regulators operators have dedicated contact to discuss issues and concerns on regular basis.
* There is little influence opportunity exist with regulators but certain argument can be shared with them about privacy, network management in particular. We need to consider a token based system where personal information is not exposed as a proposal.
* Increased encryption is letting operators off the hook as it is not possible for them to be compliant.
* There has been certain concerns explained about using encrypted traffic for illegal communication, content etc.
* Only content providers can provide this information.
* There is a risk even though end to end encryption can be exacerbated. Regulators can change the criteria but this is just an assumption today.
* It is difficult to do this in a meaningful way, for operators. IAB concluded blocking and filtering can be done at the endpoint of the communication. The same applies for lawful intercept, it is not feasible to go to all the endpoints.
* Internet of things can provide different flavours of encryption, that will make operators positions more difficult to fulfil because of the level of complexity.
* We can collectively approach GSMA and 3GPP and act collectively to alleviate the risk imposed by encrypted traffic for lawful intercept.
* Encourage on operators to produce transparency report, start preparing it now.

