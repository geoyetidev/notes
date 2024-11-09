# NIST - AI RMF

[Landing Page](https://www.nist.gov/itl/ai-risk-management-framework)
[PDF](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-1.pdf)

![[NIST.AI.100-1.pdf]] 
# Executive Summary

Risk:
+ long-term v. short-term
+ high-probability v. low-probability
+ systemic v. localized
+ high-impact v. low-impact

Inherently socio-technical in nature - influenced by societal dynamics and human behavior

**AI-actors** - "those who play an active role in the AI system lifecycle, including organizations and individuals that deploy or operate AI" - OECD (2019)

Part I - frame risk and analyze what "trustworthiness" means in this contex
Part II - Core Framework. Specific functions **Govern**, **Map**, **Measure**, **Manage** 

See also the [[NIST AI RMF Playbook]] 



#### Background
+ [the National AI Initiative Act of 2020](https://www.congress.gov/bill/116th-congress/house-bill/6216)
+ [National Secuirty Commission on Artificial Intelligence recommendations](https://www.nscai.gov/2021-final-report/)
+ [The Plan for Federal Engagement in Developing Technical Standards and Related Tools](https://www.nist.gov/system/files/documents/2019/08/10/ai_standards_fedengagement_plan_9aug2019.pdf)
+ RFIs
+ 3 Workshops
+ public comments on concept paper
+ two drafts

# Foundational Information
## Framing Risk
**Goal** Address, Document and Manage AI Risk

Risk = probability of event X impact of event

Impact can effect individuals, groups, communities, organizations, society, the environment, the planet

Assume that humans believe AI systems work - and work well - in _all_ settings. 
Perceived as being more objective even if this is not true. 

### Risk Measurement
+ **Risks related to third-party software, hardware, and data** - is your organization's risk metric consistent with the vendor's risk metric?
	Given the generalized nature of these tools,  even if organizations' and vendors' metrics _are_ aligned on risk - how can vendors even know whether or not line users of their system are doing so _consistent_ with communicated expectations about risk
+ **Tracking emergent risks** - AI system impact assessment
+ **Availability of reliable metrics** - "The current lack of consensus on robust and verifiable measurement methods for risk and trustworthiness, and applicability to different AI use cases, is an AI risk measurement challenge. "
	Measurement problems:
	+ oversimplified
	+ gamed
	+ lack critical nuance
	+ become relied on in unexpected ways
	+ fail to account for differences in groups and contexts
+ **Risk at different stages of the AI lifecycle** - Risk profile of the vendor creating the pre-trained model vs risk profile of the developer responsible for deploying fine-tuning that model to a specific usecase
+ **Risk in real-world settings** labs vs real-world operational risks
+ **Inscrutability** - limited explainability   
+ **Human Baseline** - Cost and difficulty of establishing human baselines for the wide variety of human tasks  

### Risk Tolerance
Willingness to bear risk to achieve objectives.  Willingness at what level (individual, organizational,  enterprise, society, etc)

### Risk Prioritization
"...not all AI risks are the same, and resources can be allocated purposefully."

## Audience
Modified framework from [[OECD Framework for the Classification of AI systems]]

AI dimensions: 
+ Application Context - document system concept, objectives and underlying assumptions. Understand legal and regulatory requirements & ethical considerations
+ Data and Input - Gather, validate and clean data, document metadata and characterize dataset in light of objectives
+ AI Model - select algorithms, train, verify, validate, iteratively calibrate to objective
+ Task and Output - Pilot, verify regulatory compliance, plan organizational change management and user experience

**TEVV** - Test, Evaluation, Verification, Validation

### AI Risks and Trustworthiness

Trustworthiness means Valid & Reliable,  other characteristics include:
* Safe - requires explanation and documentation of risks, appropriate use
* Secure & Resilient - manage unexpected changes, degrade safely and gracefully where possible.
* Accountable and Transparent - degree to which information about the system is available to users.  Hierarchical in that users should be able to access varying levels of detail to address their information need
* Explainable & Interpretable - Is it understandable by what mechanism an output was generated,  and can the outputs be understood in the context of the systems purpose?
* Privacy-Enhanced - autonomy, identity, dignity
* Fair (harmful bias managed) - Several categories of bias:
	* Systemic - dataset bias, organizational norms, practices and processes of AI lifecycle
	* Computational & Statistical - non-representative samples, local minima 
	* Human-Cognitive - How humans think about purposes and functions of an AI system
* 

Valid - objective evidence that the requirements for specific intended use are met
Reliable - perform as required without failure under given conditions

# AI RMF Core

Four Functions:
+ **Govern** - culture of risk management is cultivated and present
+ **Map** - context is recognized and risks related to context are identified
+ **Measure** - identified risks are assessed analyzed or tracked
+ **Manage** - Risks are prioritized and acted upon based on projected impact



# Links
[[NIST]]
