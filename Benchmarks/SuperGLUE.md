Paper: [[SuperGLUE- A Stickier Benchmark for General-Purpose Language Understanding Systems]]

## From [[An In-depth Guide to Benchmarking LLMs]]

Tests [[Natural Language Understanding]]

More diverse and challenging collection of tasks than [[GLUE (General Language Understanding Evaluation)]]

Eight subtasks:
* Boolean Questions (BoolQ): yes/no QA task
* CommitmentBank (CB): truthfulness assessment 
* Choice of Plausible Alternatives (COPA): causal reasoning task
* Multi-Sentence Reading Comprehension (MultiRC): true/false QA task
* Reading Comprehension with Commonsense Reasoning Dataset (ReCoRD): multiple-choice QA task
* Recognizing Textual Entailment (RTE): two-class classification task
* Word-in-Context (WiC): is a binary classification task
* Winograd Schema Challenge (WSC): pronoun resolution problems

Two metrics:
* Broad Coverage Diagnostics: to automatically test an LLM’s linguistic, common sense, and general world knowledge
* Analysing Gender Bias in Models: an analytical tool for detecting a model’s social biases 
#### Pros
* A thorough and diverse range of tasks that test a model’s NLU capabilities
####  Cons
* A smaller range of models are tested against SuperGLUE than similar benchmark MMLU 
