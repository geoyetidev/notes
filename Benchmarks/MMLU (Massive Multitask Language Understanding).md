Paper: [[Measuring Massive Multitask Language Understanding]]

## From [[AI - Overview of common LLM Benchmarks]]

**The goal**: To assess a model's ability to understand and respond correctly across a wide range of subjects, from elementary knowledge to advanced topics.

**The test**: The model is tested with more than 15,000 questions from over 50 different subjects, including humanities, sciences, and social sciences, with questions designed to reflect varying levels of difficulty.

## From [[An In-depth Guide to Benchmarking LLMs]]

How well a model understands language and, subsequently, its ability to solve problems with the knowledge to which it was exposed during training. 

Focused on [[Natural Language Understanding]]

15,908 questions divided into  57 tasks 
STEM, humanities,  social sciences, and other subjects from an elementary to an advanced professional level.  Departure from [[SuperGLUE]] with a focus on specialized knowledge

**Does not mention how it is quantiatively evaluated**

#### Pros

* Tests a broad range of subjects at various levels of difficulty 
* Broad corpus helps identify areas of general knowledge in which models are deficient
#### Cons

* Limited information on how corpus was constructed
* Dataset is shown to have numerous errors (See: [[Errors in the MMLU- The Deep Learning Benchmark is Wrong Surprisingly Often]])

