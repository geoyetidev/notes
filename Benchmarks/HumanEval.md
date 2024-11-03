Paper: [[Evaluating Large Language Models Trained on Code]]
## From [[AI - Overview of common LLM Benchmarks]]
**The goal**: To measure a model’s ability to write correct Python code to solve programming problems.

**The test**: The model is given programming tasks, and its output is compared against expected solutions to determine correctness.

## From [[An In-depth Guide to Benchmarking LLMs]]
 Generate functionally correct code; 

HumanEval dataset
164 diverse coding challenges that include several unit tests (7.7 on average). 

pass@k metric:
Probability that at least one of k generated code samples pass the coding challenge’s unit tests, given that there are c correct samples from n generated samples.

Improves on BLEU (bilingual evaluation understudy) metric - was used to assess the textual similarity of model-generated coding solutions compared with human ones. The problem with this approach, however as it doesn’t evaluate the functional correctness of the generated solution; 
#### Pros
* A good indication of a model’s coding capability 
* Unit testing mirrors the way humans evaluate code functionality 
#### Cons
* The HumanEval dataset doesn’t comprehensively capture how coding models are used in practice. For instance, it doesn’t test for aspects such as writing tests, code explanation, code infilling, or docstring generation.