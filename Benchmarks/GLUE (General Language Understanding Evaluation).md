Paper: [[GLUE- A Multi-Task Benchmark and Analysis Platform for Natural Language Understanding]]

### From [[AI - Overview of common LLM Benchmarks]]

**The goal**: To measure a model's ability to perform a variety of natural language understanding tasks.

**The test**: The model is tested on a suite of language tasks, including sentiment analysis, textual entailment, and sentence similarity.

#### Definitions
_Sentiment analysis_ is the process of determining the emotional tone or opinion expressed in a piece of text, typically categorizing it as positive, negative, or neutral.

_Textual entailment_ is the task of determining whether a given piece of text (the hypothesis) can be inferred or logically follows from another piece of text (the premise).

Here's an example of textual entailment:

	Premise: "The cat is on the mat."
	Hypothesis: "There is a cat."

This is a positive textual entailment because the second sentence (hypothesis) can be inferred from the first sentence (premise).


### From [[GLUE- A Multi-Task Benchmark and Analysis Platform for Natural Language Understanding]]

**NOTE** - paper provides citations for each of the underlined tasks. If these come up more frequently we should include them as baseline benchmarks.


GLUE is a platform for evaluating and analyzing [[Natural Language Understanding]] systems. Attention mechanisms shown to beat state of the art models at the time but not particularly successful on the benchmark (room for improvement)

#### Tasks
Nine English sentence understanding tasks:
_Single Sentence Tasks_
+ **CoLA** The Corpus of Linguistic Acceptability - English acceptability judgments from books and journal articles on linguistic theory.
+ **SST-2** The Stanford Sentiment Treebank - movie reviews with human annotations on their sentiment

_Similarity and Paraphrase Tasks_
+ **MRPC** The Microsoft Research Paraphrase Corpus - sentence pairs extracted from news sources, human annotation for whether sentences are semantically equivalent
+ **QQP** The Quora Question Pairs - Taken from Quora website. Determine if questions are semantically equivalent. 
+ **STS-B** The Semantic Textual Similarity Benchmark - Sentence pairs from news headlines, video and image captures. Human annotated with similarity score between 1 and 5

_Inference Tasks_
+ **MNLI** The Multi-Genre Natural Language Inference Corpus - crowd sourced sentence pairs with entailment annotations. Given a premise and a hypothesis annotate whether the premise entails, contradicts or "neithers" the hypothesis. sentences taken from speeches, fiction, government reports. (Cross trained with SNLI corpus)
+ **QNLI** The Stanford Question Answering Dataset - question answer paragraph examples taken from Wikipedia. One sentence in the paragraph answers the question. _Slightly different use than original paper that creates the dataset_
+ **RTE** The Recognizing Textual Entailment - annual text entailment challenges. Combines RTE1, RTE2, RTE3 and RTE5. News and Wikipedia text. Classifies into neutral, contradiction and no_entailment. 
+ **WNLI** The Winograd Schema Challenge - Reading comprehension task. Sentence with pronoun, resolve the pronoun from a list of choices. Re-purposes dataset by creating sentence pairs by replacing ambiguous pronoun with each possible referent and then test if the replaced sentence is entailed by the first sentence.

#### Additional Diagnostic Dataset
Cites [[#Robin Cooper, Dick Crouch, Jan Van Eijck, Chris Fox, Josef Van Genabith, Jan Jaspars, Hans Kamp, David Milward, Manfred Pinkal, Massimo Poesio, Steve Pulman, Ted Briscoe, Holger Maier, and Karsten Konrad. Using the framework. Technical report, The FraCaS Consortium, 1996| FraCas]] and [[#Allyson Ettinger, Sudha Rao, Hal Daum´e III, and Emily M Bender. Towards linguistically generalizable NLP systems A workshop and shared task. In First Workshop on Building Linguistically Generalizable NLP Systems, 2017.| Build-it-Break-it]] competition as inspirations.

Focuses on predefined set of linguistic features of interest,  at a high level these are
+ Lexical Semantics
+ Predicate-Argument Structure
+ Logic
+ Knowledge

"We ensure the data is reasonably diverse by producing examples for
a variety of linguistic phenomena and basing our examples on naturally-occurring sentences from several domains (news, Reddit, Wikipedia, academic papers)"

Uses [[Natural Language Inference]] tasks. Given two related sentences the produce one label of _entailment_ (E), _neutral_ (N), or _contradiction_ (C).  For example:

1. The timing of the meeting has not been set, according to a Starbucks spokesperson.
2. The timing of the meeting has not been considered, according to a Starbucks spokesperson

One has a "Neutral" relationship with two.  Two has an "Entail" relationship with One. 

550 total sentence pairs creating 1100 total examples
+ 42% entailment
+ 35% neutral
+ 23% contradiction
Metric is "R_3, a three-class generalization of the Matthews correlation coefficient" [[#Jan Gorodkin. Comparing two k-category assignments by a k-category correlation coefficient. Comput. Biol. Chem., 28(5-6) 367–374, December 2004. ISSN 1476-9271. |Gorodkin, 2004]]

Human baseline performance between **6** NLP researchers annotating 50 samples (100 examples) randomly sampled form the dataset. Inter-annotator agreement is high with a Fleiss's k of 0.73. Average R_3 score among annotators is 0.80 - much higher than baseline systems

**Intended Use**: "The diagnostic examples are hand-picked to address certain phenomena, and NLI is a task with no natural input distribution, so we do not expect performance on the diagnostic set to reflect overall performance or generalization in downstream applications. Performance on the analysis set should be compared between models but not between categories." 

#### Analysis
Coarse Categories - overall performance is low for all models
Fine-Grained Subcategories - good performance on "Universal Quantification" task - looks like presence of "all" is a strong indicator

Overall poor performance but some indication that attention models with more context will show improvements in performance.

#### Citations

#papers_to_process 
##### Robin Cooper, Dick Crouch, Jan Van Eijck, Chris Fox, Josef Van Genabith, Jan Jaspars, Hans Kamp, David Milward, Manfred Pinkal, Massimo Poesio, Steve Pulman, Ted Briscoe, Holger Maier, and Karsten Konrad. Using the framework. Technical report, The FraCaS Consortium, 1996


##### Allyson Ettinger, Sudha Rao, Hal Daum´e III, and Emily M Bender. Towards linguistically generalizable NLP systems: A workshop and shared task. In First Workshop on Building Linguistically Generalizable NLP Systems, 2017.

##### Jan Gorodkin. Comparing two k-category assignments by a k-category correlation coefficient. Comput. Biol. Chem., 28(5-6):367–374, December 2004. ISSN 1476-9271.