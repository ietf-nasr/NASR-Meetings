## NASR Side Meeting 4 November 2024 - IETF 121 Dublin

No signature taken but around XX people present in the room and online

### Draft presentations:
- **[Handling Multiple Verifiers in the RATS Architecture](https://datatracker.ietf.org/doc/draft-zhang-rats-multiverifiers/)**
    -   Houda Labiod / Zhang Jun:

 - **Main comments:**
    - Clarify how nonce ensures that all verifiers get same answer? Makes the assumption that the time the evidence is received the nonce is created, because the goal is for the verifiers to deal with the same evidence Furthermore, it is the relying party that sends the request (not the verifiers), which creates the bundle of evidence with the nonce.
    -  What is the role of the verifier manager? To create a short list of verifiers based on a template provided by the relying party.
    -  The trust model among the various elements should be clarified, as for instance the verifier manager is a single point of failure.
    - If the verifier owner provides the appraisal policy (i.e., which verifier to trust) what else is the verifier manager doing beyond generating trust anchors for the set of verifiers? It is true that you can delegate to the verifier manager the appraisal policy and then send to the verifiers. The trust model assumes all verifiers as equivalent. Yet-, the questions is what if it is not the case? This question remains open.
    - Does the relying party know the verifier owner? Yes, it will.


### General discussion on next steps:

- Limited domains seems to be the right approach. Having an Internet-wide deployment, with global trust, is not realistic.
- Connecting 2 or more limited domains seems feasible as long that there is a mean to ”share” or “transfer” the verification/trust information, via an attestation for instance, so that the verification made in one domain can be continued in another domain. This assumes that domains have specific “agreement” to do so. 
- In the hypothesis that several different requirements exists, this means that different limited domains can use different properties/solutions as long as the agree on the “cross domain attestation”.
- In case of overlays, it seems meaningful to be able to verify both the overlay and the underlay, as an untrusted underlay makes hardly possible to trust the overlay.
- We need a crisp definition of the controlled (e.g. SDN) domain boundaries, starting small but keeping in mind the cross-domain extension of the feature set to grow bigger.
- In order to accommodate the various use cases, the focus should be on generic attributes verification/attestation. The attributes can be a geographic location or a security SLA requirement or anything else. Is not just device trust, rather trust the proof that the device has the requested attributes. 
- We should give negative examples. Like the fact we can catch situation where routing would forward packets through boundaries that are not acceptable the specific use case (slide 6 untrusted black router). It is not that there is an error in routing. Traffic with no specific requirements can follow that path.

#### High priority action points:
- Refine the scope and problem statement
- Terminology: even during the side meeting terminology was somehow not completely aligned among the participants
- Start thinking about a charter proving that the problem is relevant for the IETF and that can be solved. 

