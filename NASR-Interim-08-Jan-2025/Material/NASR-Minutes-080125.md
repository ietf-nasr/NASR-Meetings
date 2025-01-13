## NASR Minutes Interim 08 January 2024

Note takers: Luigi Iannone

### Opening - Luigi Iannone & Nancy Cam-Winget

- Any Comment on last meeting minutes?

No additional comments on published minutes.

### Overview existing Pull Requests on Charter: All
- https://github.com/ietf-nasr/NASR-Charter

Luigi Iannone: Showing slides with recent changes and pull requests for the charter.


Yutaka OIWA: Avoid using the word trust in the first sentence, since without context can mean anything.

Nancy Cam-Widget: The term "blindly" is also to avoid. New intro paragraph a bit too complex. We may prefer simpler and more direct paragraph. I am working on it and send changes later on. So,the way I would look at it is from an evolutionary path for the technology. We require more of not just the protection of the data. But and now I'm looking at your second one, and I'm harping on the word audit. What we're talking about is about enforcement from a routing/forwarding position or from an auditing and visibility, meaning, if an owner of a deployment wants to ensure that the path that's taken is using network nodes that are deemed to be compliant to a set of claims.

Luigi Iannone: I would avoid the term Internet, we are not proposing an Internet-wide deployment. The fact that we want to use a path, where the network elements are compliant to a set of claims, is a nice formulation. I am a bit concerned about the word ""enforcement". Because if we want to enforce something, then we need to have an impact on the control plane, which means do routing.

Nancy Cam-Widget:  we can leave the enforcement absolutely. It goes to the "How do we provide the right mechanisms by at least ensuring that there's some visibility or auditability that the nodes that are being used are compliant. Will provide my text later.

Luigi Iannone: There is the pull request about the central part of the background and motivation section. The changes concern mainly rephrase some sentence to avoid using the term "clients", replaced by "customers" as customers of the NASR service. Looks less confusing to me.

Nancy Cam-Widget:  "customers can be confusing as well. May be better to use "network deployments". Network deployments today require elevate security, privacy.


Yutaka OIWA: We have two mixed issue here. The first sentence introduces both the problem statement and client service model. We should be more generic in the first part and rearrange a bit the second part.

Peter Liu: Originally, I wanted to refer to clients of the connectivity service offered by the operators.

Nancy Cam-Widget:  In general terms, in network deployments, independently if done through an operator or not, there are requirements such that to ensure that the devices that are providing the connectivity are compliant, having the latest security updates, past integrity checks and so on. From a charter perspective, I don't think we want a solution just for service providers. text has to be more generic; about service.


Luigi Iannone: In this part we have as well the "out of scope" section, which I think is better at the end of the charter. Can be used to quickly address received feedback like the fact that "proof of non-transit" is out of scope (too hard to solve in the specific cases when is solvable... ). Also delete the paragraph about WG collaboration, since we have one at the end of the charter.

Luigi Iannone: Other remark received on the chat during the first BoF is the lack of a threat model. Should we have explicit document or put it in an existing document?

Yutaka OIWA: Agreed that we need a threat model to be discussed in the group.

Peter Liu: But we are not looking for vulnerabilities we are building trust.

Luigi Iannone: The point is more about what can be protected/proved and what cannot. We do not need a specific document we can put it in the problem statement and requirement document. 

Antoine Fressancourt: Yes, because, from what I heard from the last buff is that we need to be clear, not overselling what NASR. It's really about positioning what NASR is doing with regards to how to maintain secure forwarding decision over limited domain and not on the Internet. 


Meiling Chen: Why do we think compliance is more proper than security.


Nancy Cam-Widget:  Security has connotations. What could be secure to me is not necessarily secure to you.

Peter Liu: One purpose is to make the difference between devices with high and low security, by separating them and choosing only the more secure.

Luigi Iannone: This is just a type of claim. ANother could be having network elements that are located only in France, because by law the data that will be shared cannot go outside the country. So,the claim may relax the device security level as a tradeoff to make sure that the device is in located in France. So,it's a different claim.

Yutaka OIWA: Compliance is very generic word, we should use "compliance to requirements".

Nancy Cam-Widget:  I didn't think we were using security.

Peter Liu: We're not inventing some new security mechanism or anything. It's more like a visibility. But reason that we want to do this work is we want to provide more security and confidence.

Nancy Cam-Widget:  That's where the word trust is more appropriate. but, what you believe is trustworthy versus what I believe is trustworthy may be subtly different.

Michael Richardson: I made a couple of English comments.

[Michael's suggestions have been accepted and merged]

Peter Liu: Have we agreement on the work item currently listed in the charter.

Yutaka OIWA: I think that are good to set for the current moment.

Luigi Iannone: Central part of the charter about goals and scope not yet revised.  I will go over it and share update with the group by tomorrow.

BoF Request has been created on GitHub ([NASR Bof Request](https://github.com/ietf-nasr/bof-request-IETF-122)). Nancy and Luigi to refine and share with the group for discussion. 


#### 3. New Name for the group: All

Most preferred Acronyms from the mailing list:

- NASR: Network Attestation for Secure foRwarding
- FELPA: Forwarding Evidence by Local and Path Attestation 

Previous proposal:

- NASR: Network Attestation for Secured foRwarding

Keeping NASR acronym but settle on the *Network Attestation for Secured foRwarding*

### Next Meeting:
- **[22nd January 2025 - 04:00 UTC](https://www.worldtimebuddy.com/?qm=1&lid=100,5391959,5128581,2988507,1816670,1850147&h=100&date=2025-1-22&sln=4-5&hf=1)**

#### **[Postponed due to lack of time]**

##### 4. NASR Service Model: Meiling Chen

##### 5. RATS Conceptual Message Wrappers (CMW) in NASR: Henk Birkholz

