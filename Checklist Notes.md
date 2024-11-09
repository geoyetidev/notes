

LLM verification has dramatically outpaced validation and is actively introducing unmanaged risk into organizational processes.  To review, _verification_ is the process of ensuring a capability meets a set of design specifications,  while _validation_ is the process of ensuring a capability meets the operational needs of a set of users. While a dramatic over simplification, the "design specifications" of LLMs is to process and generate natural language text. If we agree to this characterization, it is immediately obvious to anyone who has interacted with a chat bot or generated an image from a description that modern models can both process and generate language at the level of a native speaker. LLM Verification? Check. 

Validation on the other hand,  remains a dubious and fundamentally qualitative. Whether or not a model has met our needs hard to qualitatively describe, and arguably impossible to epistemologically quantify. It is, among other things, particularly vulnerable to **satisficing**; where we accept an answer as "good enough" based on some arbitrary and context-dependent threshold.  


Casual use of LLMs leads to casual validation "metrics" like _feelings_; as in "I _feel_ like the model is doing a good job of addressing my operational need."  This approach to user acceptance is individual, ad-hoc and heterogeneously dispersed across the workforce.  This "vibes" based assessment of the contexts in which a model can or cannot be trusted 

that likely, as of today, operates outside of any organization policy or governance structure.

"Prompt engineering" as a concept demonstrates the chasm that exists between verification and validation.  While the interface is natural to begin with,  if the produced content is not exactly what we're interested in we're forced to adopt increasingly non-natural language to achieve our goal. 

Production of desired content almost always involves...


Frame questions of validity as essentially an exercise in information literacy. Here is an information resource that purports to address my operational need for information. How can I approach this resource in a principled way? 

Tension between your operational need and the original intent of the corpus creation. 


#### Data Suitability
_The model is, at least in some part, a reflection of the corpus of text its been trained on_. 
#### Model suitability
Characterizing the corpus is necessary but insufficient for understanding model validity because model behavior also matters.  Concrete metrics  

#### Workforce suitability
Model quality and trust depend on the context and operational goals in which that model is being used.  Model's that are trustworthy in one context may be deeply problematic in another. While Data & Model suitability are important factors in determining the contexts and operational goals in which a model excels,  communicating this to the workforce and ensuring LLMs are not being used contexts that are inconsistent with organization risk postures is its own set of challenges.

E.g. Relying on a model to **do** research rather than **assist** in research.  

#### Governance and Policy




### Questions inspired by [[Framework for Information Literacy for Higher Education]]
#### Authority
+ Topics on which the dataset has authority?
	+ What are the origins of this text and the motivations of the individuals who produced it?
	+ In what context was this information produced and what is the relationship between that context and your information need or purpose?
	+ What types of credentials convey authority within the dataset?
	+ What schools of thought exist within the dataset and how do they confirm or deny the premise on which your information need is founded?
+ Where are there conflicting perspectives within the schools of thought represented in the dataset? 
#### Information Creation
+ Can you articulate the capabilities and constraints that produced the underlying dataset?
	+ Are there inconsistencies between the creation process and the operational need?
	+ Have there been substantive changes in the creation process over time? 
+ What motivates the underlying dataset's creation?
+ To what degree does persuasion play into the underlying corpus?
+ What interests are and stakeholders are underrepresented in your corpus? 
+ What information sources related to your operational purpose are not represented in your corpus? 
+ Who were the various audiences for the initial creation of this corpus?
	+ What were their original interests?
	+ To what degree does your current operational need align with the interests of the original audiences?
	+ Can you characterize whether or not the audience(s) feel the documents in the corpus met/meet their needs? What gaps exist from their perspective? 

#### Research as Inquiry
+ How well the corpus represent the process by which knowledge about operationally relevant information was refined?
+ Are there specific information needs, or research questions that informed the creation of the corpus?
+ Does the corpus have an explicit scope? 
	+ What is the relationship between the corpus scope and the operational need?

#### Scholarship as Conversation
+ What are the sources of evidence in your corpus and to what degree are they expressed?
+ What are the methods of investigation/collection that produced your corpus? Can those methods address your operational need?
+ To what degree does your dataset contain specific modes of discourse or jargon?
	+ Does your corpus contain supporting information that bridges common language uses with the specialized information in your dataset?
+ Are there aspects of the discourse contained within your corpus that are largely considered resolved? 
+ What are the open areas of knowledge within the corpus that are unresolved or still contested?  
+ With what fluency does your end user operate given the jargon and discursive communities represented in your dataset?
	+ Is there specialized knowledge that they lack?
	+ Are there confounding issues with their own understanding of specific discursive idiosyncrasies? 

#### Strategic exploration
+ Is your operational need for engaging with the corpus foundationally fact based?
+ Do your operational outcomes rely on "insight" of some kind? 
	+ If so do you expect this insight to come from the model?
	+ Is the insight limited in scope or apart of a closed information need? (e.g. what are the relationships between the entities as described in this text? e.g. Something verifiable).
	+ Is the insight broad and based on an open information need? (e.g. predictive or probability based. e.g. "how likely is this entity to do x?" "if entity A does X, what will entity B do?") 
+ Does the corpus support identifying entities that have an interest in your operational need? (e.g. organizations,  governments, industries) 
+ Does the corpus contain information about additional resources related to its intended use? to your operational need? 







# Scratch Ides
+ its impossible to train a model exclusively on your data. You do not have enough textual examples.  You must begin with a model that has been trained broadly on a dataset you don't have access to assess.  How much of that dataset "leaks" through your fine tuned data? 

People, process, technology
Multi-stakeholder engagement and planning

Its going to take longer than you think
Don't have shared language
People don't have empathy for each others day jobs
Risk posture/tolerance not the same
Lack shared language to assess whether or not the risk posture is consistent

