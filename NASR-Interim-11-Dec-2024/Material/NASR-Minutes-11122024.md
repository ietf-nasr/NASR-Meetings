## NASR Minutes Interim 11 December 2024

Note takers: Peter Chunchi Liu & Luigi Iannone

### Opening - Luigi Iannone & Nancy Cam-Winget

- Quick tour on the resources available on GitHub, namely:
    - [NASR Meetings Repository](https://github.com/ietf-nasr/NASR-Meetings)
    - [NASR Charter Repository](https://github.com/ietf-nasr/NASR-Charter)
        - Contributions to charter can be submitted as [Pull Request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests), either by [forking the repository](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork) or [directly from your local copy](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request) if you have write permission.
        - TOrequest write m=permission on charter repository send an email to [nasr-chair@ietf.org](mailto:nasr-chair@ietf.org)


### Peter Chunchi Liu presented recent proposed changes to the charter:

1. Goal update: 
    - From *"route data on trusted elements"* to *"provide proofs that data forwards on security-satisfying network elements, which includes security statuses, attributes, functions*." The point is to collect and present these information.
2. Wording:
    - From *"trustworthy"* to *"security-qualifying (devices)."*
3. Scope: 
    - *"simple source routing paths in/in between limited domains"*
and corresponding proposed work documents. 
 
### General Discussion on Charter progress


Luigi Iannone: Leaving routing out of scope is good, makes the group focus.

Yutaka Oiwa: Still interested in considering inter-domain solution. We do not need routing but orchestration to some extent.

Diego Lopez: The point is to expose data path properties to the clients and operators we can also discuss (in use case document or a separate document) the logic of how to use NASR-produced information to help orchestration or routing, but not in charter that may confuse people.

Yutaka Oiwa: Yes, we are not standardizing the orchestrator behavior. 

Luigi Iannone: Yutaka can provide text for the use case document so that his use case is documented. Yutaka can suggest some text for the charter to make sure in the future the use case can be addressed, but not right away so to have an initial limited scope.

Yutaka Oiwa: Yes, may be for the meeting on 22 January 2025.

Ray Atarashi: We need elements to exchange information between operator and client, what specific information to be exchanged is of ISP interest. I would like to contribute to the service model from an ISP perspective and also for the use cases. 

Peter Chunchi Liu & Diego Lopez: That is the service model draft (security item requested from client to operator, and information back) Meiling Chen is working on, you can contribute to her repo. 

Luigi Iannone (reporting Meiling Chen on the chat): Meiling Chen will share repo on the mailing list.
 
Luigi Iannone (reporting Meiling Chen on the chat): Where does the path information data come from? My suggestion is to collect the security attributes of nodes through BGP-LS. We only need some extensions. Who decides the forwarding path? We use the controller to decide. Of course, this is in the same domain. Do we need to clarify what specific functions are needed to implement the NASR controller?

Diego Lopez: It is wise to start with base mechanism (how data of the path is built and delivered), then have the details like BGP-LS extension stuff later. Exposing technical details now might confuse the IESG.
 
Luigi Iannone (reporting Meiling Chen on the chat): Do we need to consider multi-domain, just two-domain? N to N is more complex, we can just focus on 1 to 1 domain, right?

Diego Lopez: I would focus for the moment the charter on the single domain environment. Once once we have the group running, we have a clear view. How we do this, we can extend the charter.

Yutaka Iowa: I can help on the common consensus of single domain, but i want to work on interdomain too.

Luigi Iannone: Doing work on inter-domain as individual submission can be done, but doing it in the WG is different. That work can be added later in the charter and adopt the individual submission. For now, you can contribute to the use case document.
 
Diego Lopez: Better to change from *"simple source routing path"* to  *"simple paths"*, otherwise we are limiting the use cases only to source routing.

Peter Chunchi Liu: Agreed.
 
Luigi Iannone summarizing the discussion:
- PR from Peter: discussion made on the list and in the meeting make the suggested changes good progress. PR will be merged and continue discussion from there.
- Inter-domain: Is an important item. We do not need necessarily text in the charter to avoid critics or confusing the IESG. Yutaka, to propose text in the use case document. Goal is to create simple and feasible 
- Routing: Giving elements and information to choose a path VS performing actual routing. The balance point between is key. 

Nancy Cam-Winget: On the last point [Eric Voit's Trustworthy Path Routing draft](https://datatracker.ietf.org/doc/draft-voit-rats-trustworthy-path-routing/) is a good reference of how a trusted topology can be achieved. 
 
Diego Lopez: The point is to obtain security status/attribute information from the path. Making routing decisions is another goal. 

All agrees!


