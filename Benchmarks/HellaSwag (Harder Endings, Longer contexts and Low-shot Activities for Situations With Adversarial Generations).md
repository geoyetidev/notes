Paper: [[HellaSwag- Can a Machine Really Finish Your Sentence?]]

## From [[AI - Overview of common LLM Benchmarks]]
**The goal**: To measure a model's ability to choose the most plausible ending for a given context, especially in scenarios where the context is longer, and the tasks are more challenging.

**The test**: The model is given a short story or context and must select the correct ending from a set of options. There are options that are tricky or misleading.

## From [[An In-depth Guide to Benchmarking LLMs]]

commonsense reasoning and natural language inference (NLI) capabilities of LLMs through sentence completion exercises

Successor to the [[SWAG]] benchmark

Segment of a video caption as an initial context and **four possible endings,** of which only one is correct.  Average human performance is **95%** 

Wrong answers generated through generation of adversarial endings with increasing difficulty 

#### Pros
+ Similar to ARC, it evaluates a model’s common sense and reasoning, as opposed to mere ability to recall facts
+ Thoroughly curated dataset: all easily completed contexts from the SWAG dataset were discarded and human assistants sifted through the adversarial endings and chose the best 70,000. 
#### Cons
+ General knowledge – doesn’t test common sense reasoning for specialised domains.  

