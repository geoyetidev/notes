Paper: [[TruthfulQA- Measuring How Models Mimic Human Falsehoods]]

## From [[AI - Overview of common LLM Benchmarks]]

**The goal**: To measure a model's ability to generate truthful and factually accurate responses.

**The test**: The model is given more than 800 questions that could easily lead to incorrect or misleading answers, and it is evaluated on how truthful its responses are.

## From [[An In-depth Guide to Benchmarking LLMs]]

Deals with [[Imitative Falsehoods]]

 817 questions across 38 categories, such as finance, health, and politics. 
 
 Two Tasks:
 * requires the model to generate answers to a series of questions. response is scored between 0 and 1 by **human evaluators**, where 0 is false and 1 is true. 
 * instead of generating an answer, the LLM must choose true or false for a series of **multiple-choice questions**, which are tallied. 
Task scores are combined

#### Pros
* Diverse dataset
* Tests LLMs for hallucinations and encourages model accuracy

### Cons
* Corpus covers general knowledge, so not a great indicator of truthfulness for specialised domains
