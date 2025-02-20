---
date: 2023-12-24
---
[Link](https://arxiv.org/abs/2306.05685)



## Authors
[[Lianmin Zheng]], [[Wei-Lin Chiang]], [[Ying Sheng]], [[Siyuan Zhuang]], [[Zhanghao Wu]], [[Yonghao Zhuang]], [[Zi Lin]], [[Zhuohan Li]], [[Dacheng Li]], [[Eric P. Xing]], [[Hao Zhang]], [[Joseph E. Gonzalez]], [[Ion Stoica]]

## Abstract
Evaluating large language model (LLM) based chat assistants is challenging due to their broad capabilities and the inadequacy of existing benchmarks in measuring human preferences. To address this, we explore using strong LLMs as judges to evaluate these models on more open-ended questions. We examine the usage and limitations of LLM-as-a-judge, including position, verbosity, and self-enhancement biases, as well as limited reasoning ability, and propose solutions to mitigate some of them. We then verify the agreement between LLM judges and human preferences by introducing two benchmarks: MT-bench, a multi-turn question set; and Chatbot Arena, a crowdsourced battle platform. Our results reveal that strong LLM judges like GPT-4 can match both controlled and crowdsourced human preferences well, achieving over 80% agreement, the same level of agreement between humans. Hence, LLM-as-a-judge is a scalable and explainable way to approximate human preferences, which are otherwise very expensive to obtain. Additionally, we show our benchmark and traditional benchmarks complement each other by evaluating several variants of LLaMA and Vicuna. The MT-bench questions, 3K expert votes, and 30K conversations with human preferences are publicly available at this https URL. 
## Links
[[MT Bench]]
