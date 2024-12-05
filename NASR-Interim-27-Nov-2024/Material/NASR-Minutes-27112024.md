## NASR Minutes Interim 27 November 2024
Note takers: Peter Liu Chunchi & Luigi Iannone

### Opening - Luigi Iannone & Nancy Cam-Winget

IESG raised concerns on whether or not interim meetings organized through IETF datatracker should count for the total number of BoF meetings.
To avoid issues meetings will be held using zoom and all the material (minutes, recording, transcript, etc.) will be made avalable as repository on the **[GitHub ietf-nasr Organization](https://github.com/ietf-nasr)**

### Abstract POT Mechanism - Peter Liu Chunchi 

Luigi Iannone: See two aspects in this document. 
    1. Interoperability between domains and POTs (POT attestation)
    2. Data plane requirements, no matter if you use SRv6 or MPLS, set of procedures and the outcome should be equivalent. 
Should we seperate 1 and 2, or which one should we focus on? 

Peter Liu Chunchi: Can give priority to what the community believes is reasonable

Luigi Iannone: As for the use cases. May be we should focus on the POT model, rather than the use cases. Since we have a use case document we can cite.

Yutaka Oiwa: Not sure will work for geo-fencing. Because the important part is the policy for the packet not the POT of the past. May be we need more analysis on this use case. It is not yet clear what kind of ingformation is needed for nodes to take decisions.

Peter Liu Chunchi: Agreed.

Jun Zhang: Raised similar point like Yutaka Oiwa. If the packet does not have to go out because of policy but the POT has an outside node in the list we can end up with situations where POT can be valid but policy doe snot allow packet to go outside the local domain. More concrete example of this scenario is needed.

Peter Liu Chunchi: Agreed. We can discuss it on the mailing list.


Luigi Iannone: share document on the mailing list (can even be submitted to create IETF I-D) so that everybody can provide concrete feedback. 

### NASR & IAB Statement on the Risks of Attestation of Software and Hardware on the Open Internet – Luigi Iannone

Michael Richardson and Nancy Cam-Winget suggested to simplify to a single sentence "NASR is not about client attestation (e.g. Web browsers, smartphones...)". Beyond the present minutes a crisp sentence can be added in the charter.

### Document Status & Charter - All

Luigi Iannone: Looking at the documents may be we can merge the expired terminology draft and the use-cases+requirements draft to have everything in one place. 

Peter Liu Chunchi: Good idea to have everything in one place.

Nancy Cam-Winget: Most important thing to do is to focus on a **<ins>crisp problem statement and charter</ins>**

Toerless Eckert: Concern about making the scope of NASR so small that becomes a library that can only be successful if other working groups will use it. Without going into the specification details we need to explain how NASR can be used to secure routing protocols, without depending on other working groups.

Yutaka Oiwa: Agreed there is still clarifications to be done.

From the chat:

~~~
    Michael Richardson: I think that Toerless raises an interesting scope question, which I think the charter doesn't need to solve, but the problem statement does.
    
    Nancy Cam-Winget: +1
~~~

Toerless Eckert:  Provide any form of reference solution that can be built without external dependencies and without necessarily saying: there is a magical NASR controller that solves all the problems we weren't allowed to standardize. We can specify a solution document that gives sufficiently enough details about what a NASR controller should do, so that you can build a solution. One solution with a controller and one self orchestrating solution.

Luigi Iannone: Good point. Clarify who will use NASR in the charter. 

Toerless Eckert: As an example one use for NASR could be 3rd party audit. So the banking use case. At the edge of the network, close to the clients. It's an auditing device that is auditing these these packets. It's auditing and and validating that the proof of transit for the whole path is compliance with regulations.

Yutaka Oiwa: This is also related to my previous point of who uses NASR and verifies the POT. Having the data already leaked (and have an audit result to it) is not acceptable.

**Luigi Iannone: Next meeting 11 December 2024 4:00 UTC.**