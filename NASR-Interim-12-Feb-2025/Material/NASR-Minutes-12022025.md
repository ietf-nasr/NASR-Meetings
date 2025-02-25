## NASR Minutes Interim 12 February 2024

Note takers: Luigi Iannone

### Key takeaways

- The BoF Request for IETF 122 was confirmed (2 hours session)
- Revised slide structure, named "Chairs" that includes an introduction, technical presentation.
- The group agreed to align terminology with ongoing discussions in RATS to avoid confusion, specifically opting for 'network attestation' over 'remote attestation'.
- Bulk of the Chairs slides are okay. Need fez adjustments here and there to improve clarity.
- The group decided to remove the section on source routing from the proposed charter, focusing instead on path attestation and its requirements.
- The next meeting is scheduled in two weeks.
- A reminder will be sent to access materials via Google Drive and GitHub.


### Opening - Luigi Iannone & Nancy Cam-Winget

- Any Comment on last meeting minutes?

No additional comments on published minutes.

#### Discussion on Chairs' slides: All

**[Version of the Chairs' slides discussed during the call](./NASR-IETF-122-Chairs.pptx)**

- Slide Structure: Luigi suggests a new structure for the slides, including an introduction, technical presentation, and discussion. He has prepared a set of slides titled 'chairs' that includes the introduction and discussion parts.

- Contributions to Problem Statement: Peter Chunchi Liu mentions contributions to the problem formulation and suggests the Lac Leman use case as a significant example. He emphasizes the need for a European telecom operator to discuss policy drivers.

- Policy Assistance: Diego Lopez expresses willingness to assist with policy-related aspects provide slides before the next interim meeting.

- Reference to ID and Documentation: Michael Richardson stresses the importance of referencing a specific ID for the use case and mentions that Peter has a document that could be useful. He also suggests involving Diego to articulate the use case.

- Terminology Consistency: Diego Lopez  highlights the need to align terminology with ongoing discussions in RATS to avoid confusion. The intention is to ensure that the working group does not introduce additional noise into the discussions.

- Network Attestation vs Remote Attestation: Michael Richardson suggests using 'network attestation' instead of 'remote attestation' to clarify the terminology. The group agrees on the importance of aligning with existing definitions to avoid misunderstandings.

- Feedback from IAB: Luigi discusses feedback received from the IAB, including comments on terminology and the need for alignment in presentations. He plans to share the feedback with Alvaro to ensure all points are captured.

- Overlap with Other Working Groups: Luigi addresses concerns about potential overlap with SAVNET, stating that their solutions are orthogonal and can be deployed in parallel.

- Proposed Charter Structure: Background and motivation part to be split on several slides to increase readability. The group agrees on the need for clarity while ensuring that the content is not overwhelming.

- Routing Terminology: Question raised about mentioning specific source routing technologies like MPLS or SRV6 in the charter. Group agrees to avoid using it, suggesting it could lead to unnecessary debate. Toerless Eckert emphasizes the importance of validating path properties through attestation, stating that service providers must offer specific path characteristics. He notes that the method of attestation is separate from how service providers manage their routing. He also suggested the use of "service path".

- Area Director Involvement: Michael Richardson confirms that they are currently in the SEC area and assumes that Deb is their sponsoring Area Director. He also suggests the necessity of having a routing technical advisor to satisfy routing area directors. The group agrees that this is a possibility and that they can discuss it with Deb.

- Attestation in Routing Devices: Toerless Eckert raises a technical question about the potential for attestation to become common in routing devices, linking it to the success of RATS. 

- Business Case for Security Services: 
    - Luigi Iannone considers that using attestation can lead to additional security-related services, particularly in SD-WAN offerings. He emphasizes the financial benefits of integrating security into routing services.
    - Antoine Fressancourt mentions the business cases for Anapaya, which is reselling SCION platforms, indicating that there is interest in secure forwarding based on non-internet technology.


#### Discussion on Problem Statement's slides: All

**[Version of the proble statement slides discussed during the call](NASR-IETF-122-Problem-Statement.pptx)**


- Comparison of RATS and NASR: Peter Liu Chunchi illustrate how RATS operate independently of path attestation, while NASR integrates RATS for enhanced security. He suggests that a clear distinction will help in understanding their respective roles. Group agrees that Henk should have a look to the slides before the BoF.

- Architecture Overview: Peter Liu Chunchi presents an overview of the architecture, focusing on a single administrative domain to avoid confusion. 

- Inclusion of Forwarders in Diagrams: Toerless Eckert suggests adding 'Forwarder' labels in the attested boxes of the architecture diagram to clarify the role of forwarding functions in the context of RATS and NASA. 


**MAIN ACTION POINTS:**

- Update the slides with the problem statement and use case by the next interim meeting in two weeks.
- Update the GitHub with the proposed charter changes after the meeting.
- Remind about the Google Drive link to the mailing list when sharing the minutes.


### Next Meeting:

- **[26 February 2025 - 04:00 UTC](https://www.worldtimebuddy.com/?qm=1&lid=2147714,1850147,1816670,2988507,100,5128581,5391959&h=100&date=2025-2-26&sln=4-5&hf=0)**
