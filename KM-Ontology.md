---
layout: default
---

# Ontology Practice 1: Knowledge Management
## Contents
- [My KM ontology](#My-KM-ontology) <br>
- [Ontology details](#Ontology-details) <br>
- [Challenges & key decisions](#Challenges) <br>
- [Left undone](#Undone) <br>
- [Acknowledgements](#Acknowledgements) <br>

As mentioned in the [Introduction](https://thomas-m-chapman.github.io/Ontology-Practice.html#Introduction), the Knowledge Management (KM) ontology that I created is a sample conceptualization of the knowledge management domain based on my experience leading KM programs at Dell EMC and BECU. There is no ISO standard for a KM ontology. If you were to create a KM ontology based on your experience in knowledge management, it might differ considerably from what you see here.

<a name="My-KM-ontology"></a> 
## My KM ontology
For this ontology, I chose to define eight facets (as classes) that are common to many knowledge management programs, including the roles that KM team members might play, the many different kinds of knowledge assets that might populate your knowledge base, the content types that might best describe each of your knowledge assets, standard stages of the KM lifecycle, a handful of audience types, various processes common to the KM function, a governance retention policy, and several professional disciplines that often overlap with the KM practice.






<a name="Ontology-details"></a> 
## Ontology details
The KM ontology includes detailed *annotations* (in the form of RDF labels and comments) that describe each class, subclass, and individual defined in the ontology. For example, the Runbook knowledge asset is defined as:



<a name="Challenges"></a> 
## Challenges & key decisions
### The “Deleted” lifecycle stage

### Lifecycle stages


### Governance & retention policies

### Access rights hierarchy


<a name="Undone"></a> 
## Left undone
Upon reflection, I realize that even this relatively lightweight ontology could be made much more robust. If I return to this exercise, I might take on the following work.

1.	Model content types more completely to account for outputs compiled from modular components. This might include, for instance, a new subclass of knowledge assets to distinguish between Atomic Asset and Compiled Asset. **Atomic Asset** would be supported with a *hasContentType* object property, while **Compiled Asset** would be supported with an *aggregates* property that points to one more Atomic Assets. 

2.	Model resolution outcomes for Feedback (Accepted, Rejected, Updated, Retired) as controlled vocabulary on the Resolve activity, or as a separate Feedback Disposition class.

3.	Add more object properties for Legal documents, including: *hasSignatory*, *requiresWetSignature*, *hasParty*, *isLegallyEnforceable*, *hasEffectiveDate*, *hasExpirationDate*, *requiresNotary*, *requiresOath*, and so on.

4.	Define explicit audience types to account for onboarding, such as *AllPractitioners* and *NewPractitioner*, as well as various stages of the learning journey: *Novice, Intermediate, Advanced*.



<a name="Acknowledgements"></a> 
## Acknowledgements
*This work was conducted using Protégé.*

Ontology editing and reasoning were performed using Protégé Desktop, an open-source ontology editor developed and maintained by the Stanford Center for Biomedical Informatics Research.

Musen, M.A. [The Protégé project: A look back and a look forward. AI Matters](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC4883684/). Association of Computing Machinery Specific Interest Group in Artificial Intelligence, 1(4), June 2015. DOI: 10.1145/2757001.2757003.


