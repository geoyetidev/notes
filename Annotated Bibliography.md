## Overview 
## [[AI - Overview of common LLM Benchmarks]]
Provides an executive overview of a number of common benchmarks used to compare industry models.  Follows a "Goal/Test" format that makes it easy to triage the benchmarks it covers for applicability to various tasks. [Link](https://dev.to/hmcodes/ai-an-overview-of-common-llm-benchmarks-3i7b) 
## [[An In-depth Guide to Benchmarking LLMs]]
Provides links to a number of common benchmarks used to compare industry models. Gives a paragraph on each model (often with key information on the quantitative evaluation of the benchmark). Provides a generalized Pros/Cons assessment of each data set. [Link](https://symbl.ai/developers/blog/an-in-depth-guide-to-benchmarking-llms/)
## [[Benchmarking AI]]
Extensive overview of various types of benchmarks for evaluation of AI across System, Model & Data dimensions. Authors have a clear preference for raising the visibility of System metrics (e.g. memory consumption, training time, etc) [Link](https://mlsysbook.ai/contents/benchmarking/benchmarking.html)

## Academic Papers

### [[GLUE- A Multi-Task Benchmark and Analysis Platform for Natural Language Understanding]] 
A generalized benchmark for Natural Language Understanding consisting of 9 tasks mostly taken from existing benchmarks. These fall into 3 broad categories including _Single Sentence_, _Similarity and Paraphrase_ and _Inference_ tasks. Performance on each task is combined to provide a single score for model performance. Each task includes human annotation. A number of baseline models are applied and over-all performance (in 2019) is poor. 

GLUE was largely made obsolete by the emergence of ELMo, BERT, and Chat GPT models which rapidly approached (and on some sub-tasks) exceeded human performance. This motivated the creation of SuperGLUE. 

### [[SuperGLUE- A Stickier Benchmark for General-Purpose Language Understanding Systems]]

GLUE rapidly suffered from advances in models related to BERT and Chat GPT based approaches. in 2020 many of the same academics who created GLUE released SuperGLUE to compensate for these issues.  This included 8 new tasks with more complex requirements to solve them. This included more [[Natural Language Inference]] and [[Textual Entailment]] tasks. Models continued to perform poorly on these types of tasks even in the GLUE benchmarks. 

