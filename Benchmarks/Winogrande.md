Paper: [[WinoGrande- An Adversarial Winograd Schema Challenge at Scale]]

## From [[AI - Overview of common LLM Benchmarks]]
**The goal**: To assess a model's understanding of common-sense reasoning and its ability to resolve ambiguous pronouns in sentences.

**The test**: The model is given sentences with ambiguous pronouns and must correctly identify which noun the pronoun refers to.

## From [[An In-depth Guide to Benchmarking LLMs]]
 Commonsense reasoning abilities. 
 
 Pronoun resolution problem where two near-identical sentences have two possible answers, which change based on a trigger word.

 Based on [[Winograd Schema Challenge (WSC)]] 

44,000 well-designed, crowdsource problems

#### Pros
* Large crowdsourced and algorithmically-curated dataset. 
#### Cons  
* The presence of annotation artefacts in the dataset. Annotation artefacts are patterns within the data that unintentionally reveal information about the target label. Although AFLITE is designed to remove this, it’s not 100% accurate due to the size of the corpus.
