## NASR Minutes Interim 26 February 2024

Note takers: Peter Chunchi Liu

### Key takeaways

- The BoF Request for IETF 122 was confirmed (2 hours session)
- A reminder will be sent to access materials via Google Drive and GitHub.


### Opening - Luigi Iannone 

- Nancy Cam-Winget excused due to conflict with other work event.

- NASR BoF Accepted and session scheduled Tuesday, March 18, 9:30 (local time). 

- Peter Chunchi Liu will send email about ANIMA presentation of NASR use case in the list -- Toerless Eckert (ANIMA Co-chair) foresees  many ways that these WGs can leverage each other. 

- IESG Pre-review will be done after slides is finalized (next week-ish). Luigi reached out for other feedback givers from last BOF for further fixing. 

#### Feedback on IAB slides and charter concerns

- IAB Feedback on Slides: Luigi contacted Alvaro regarding feedback from the IAB on the slides presented. Alvaro is satisfied with the slides addressing the IAB official feedback and has three main points regarding the charter.
    - Use Cases Definition: Alvaro prefers specific use cases to be defined rather than leaving it to the working group. Luigi argues that documenting existing use cases is sufficient and should be clear from the presentation.
    - RFC 8799 Reference: Alvaro points out that RFC 8799 does not originate from IETF consensus and suggests dropping the reference while maintaining the concept of limited domains. Luigi agrees with this approach.
    - Source Routing vs Service Path: Alvaro notes the change from 'source routing path' to 'service path' and suggests including Spring as a related working group. Luigi agrees and mentions that Spring may be necessary for traffic steering.


#### Discussion on Technical slides: All

**[Version of the Chairs' slides discussed during the call](.)**

Toerless Eckert: Seperating POT (and related header extension) and the path-attestation as equally important but different building blocks, can help other WGs (like ANIMA) to reuse. Authentication method of the elements on the path (POT, also lightweight) can be reuseable and help achieve more goals like avoid HBH encryption and more efficiency, overall improve infrastructure security.

Diego Lopez: Works like SFC/SRH. 

Toerless Eckert: That is more on the transport layer but now this WG focus on network layer.

Diego Lopez: Will work on further update to the use case and let luigi know.

Luigi Iannone: Michael Richardson should help present the architecture at a glimpse part?

Architecture slide should highlight boxes and arrows where exists in RATS and new in NASR. Peter will work on that.

This slides should be sent to Henk/Nancy (RATS people) to pre-review. Maybe they should present (like RATS state of the art) ?  Luigi: we might be redirected to RATS, so maybe no. All agrees.

Toerless Eckert: What will be the expected answer why shouldn't we work in RATS?
Luigi, Peter: 1. device attestation -> path/network attestation, 2. Proof of Transit and network level verifications.

Toerless Eckert: Which area it should be placed? 

Diego Lopez: IESG, after a lot of discussion with us, recommends us to SEC. It should be reasonable. Ned, Thomas, Roy are also important people, potential RATS supports, from whom the review should be requested. 

Peter Chunchi Liu: How should we present the use case? 

Luigi: Diego should present the lead and general use case, and mention China Mobile and China Unicom's specific cases quickly, avoid details. All agrees. 

Toerless Eckert: Explain "path attestation" is only done once, 2. is continuously every packet or flow. 

Diego Lopez: We should align terminologies. Architecture page and the general use case page. Peter will fix that. 

Diego Lopez, Toerless Eckert: we can make analogies like AI "training-inference". Peter: or in TCG terms like "measured boot-verify".

Toerless Eckert: Single path only? 

Peter Chunchi Liu: now yes to make it minimally viable. 

Problem Statement page: 
Luigi Iannone: change word:  Client --> customer, to avoid confusion of end client software.

Toerless Eckert: Put the contents in the table to a 1v1 AS-IS vs TO-BE style. Add automation to Visibility and verifiability.

Toerless Eckert & Luigi Iannone: "deterministic forwarding" might be misleading, for people to think about DETNET. Maybe change to accountable forwarding. 

Also add comparison from no assurance to service properties -->  Now provide service assurance through attestation. Traffic leakage causing security --> no traffic leakage. Change RATS to attestation technology.  NASR now drives attestation technology to go further. 

Closing: Remaining revisions are on track.  Before send out for pre-reviews.



**MAIN ACTION POINTS:**

- Refine the slides as discussed. Finish last revisions on the list. Before send out for pre-reviews.
- Update the GitHub with the proposed charter updates after the meeting.



### Next Meeting will happen @ IETF 122:

- **[18 March 2025 - 02:30 UTC](https://www.worldtimebuddy.com/?qm=1&lid=1850147,1816670,1609350,2988507,100,5128581,5391959&h=100&date=2025-3-18&sln=2.5-4.5&hf=1)**
