[Webpage](https://symbl.ai/developers/blog/an-in-depth-guide-to-benchmarking-llms/)

Collection of Questions or Tasks
Scoring Mechanism


+ [[AI2 Reasoning Challenge (ARC)]]
+ [[HellaSwag (Harder Endings, Longer contexts and Low-shot Activities for Situations With Adversarial Generations)]]
+ [[MMLU (Massive Multitask Language Understanding)]]
+ [[TruthfulQA]]
+ [[Winogrande]]
+ [[GSM8K (Grade School Math 8K)]]
+ [[SuperGLUE]]
+ [[HumanEval]]
+ [[MT Bench]]


## Leaderboards
a published list of benchmark results for each language model. The designers of each benchmark tend to maintain their own LLM leaderboards, but there are also independent leaderboards that evaluate models on a series of benchmarks for a more comprehensive assessment of their abilities.  

[HuggingFace Leaderboars](https://huggingface.co/collections/open-llm-leaderboard/the-big-benchmarks-collection-64faca6335a7fc7d4ffe974a)

## Problems with Benchmarking
* Dataset leakage (models sometimes train on dataset by accident - oops!)
* As benchmarks become popular,  models can be tuned to those benchmarks (marking incentive)
* Measure of performance happens in a controlled environment - is it representative of reality?
* Performance on specific knowledge domains is unclear because most benchmarks are against general knowledge