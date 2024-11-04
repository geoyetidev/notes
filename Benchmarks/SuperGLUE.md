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

### From [[SuperGLUE- A Stickier Benchmark for General-Purpose Language Understanding Systems]]

Models still generally under-performing on **WNLI** and **RTE** but otherwise at/above human performance.  SuperGLUE motivated by this fact.  Fact attributed to transfer learning from large unlabeled datasets (e.g. Chat GPT, BERT, ELMo).

Performance on the [[GLUE (General Language Understanding Evaluation)#Additional Diagnostic Dataset|diagnostic dataset]] still poor with an R_3 of 0.42 which is far below human performance at 0.80

"...even as unsupervised pretraining produces ever-better statistical summaries of text, it remains difficult to extract many details crucial to semantics without the right kind of supervision. "

Tasks weighted equally in determination of aggregate performance.

Tasks should be solvable by most college-educated English speakers.
#### Eight New Subtasks:
+ **BoolQ** Boolean Questions - QA task with short passage and yes/no question about the passage. Question submitted through Google, paired with a paragraph from Wikipedia that answers the question. 
+ **CB** CommitmentBank - short text with sentences that contain at least one embedded clause. Annotated with degree to which it appears the person is _commited_ to the truth of the clause. Taken from Wall Street Journal, fiction from British National Corpus and Switchboard. Examples have premise and corresponding hypothesis which is the extraction of that clause 
+ **COPA** Choice of Plausible Alternatives - system gets premise sentence and must determine and must determine cause or effect of the premise from two possible choices. topics from blogs and photography-related encyclopedia.
+ **MultiRC** Multi-Sentence Reading Comprehension - QA task with context paragraph and question about the paragraph and a list of possible answers. System must predict which answers are true and which are false. Inference from multiple sentences is required. paragraphs pulled form news, fiction and historical text.
+ **ReCoRD** - Reading Comprehension with Commonsense Reasoning Dataset. Multiple-choice QA Tasks using Cloze-style question where one entity is masked out. System must predict the masked entity from list of possible entities in the passage. 
+ **RTE** Recognizing Textual Entailment - Same task as in [[GLUE (General Language Understanding Evaluation)]] 
+ **WiC** Word-in-Context - word sense disambiguation task cast as binary classification of sentence pairs. Two sentences with the same word - model must determine if the word is used in the same sense (true/false).
+ **WSC** Winograd Schema Challenge - co-reference resolution task. Given a sentence with a pronoun and a list of noun phrases system must determine correct referent. Designed to require everyday knowledge and reasoning to solve 


#### Diagnostic tasks:
+ Diagnostic dataset retained but _contradiction_ and _neutral_ collapsed into binary _entailment_/_not_entailment_ classes
+ Winogender included as additional diagnostic test to detect gender bias. Coreference task with gendered pronoun. 


#### Examples
**BoolQ** 
+ Passage: Barq’s – Barq’s is an American soft drink. Its brand of root beer is notable for having caffeine.Barq’s, created by Edward Barq and bottled since the turn of the 20th century, is owned by the Barq family but bottled by the Coca-Cola Company. It was known as Barq’s Famous Olde Tyme Root Beer until 2012.
+ Question: is barq’s root beer a pepsi product 
+ Answer: No

**CB** 
+ Text: B: And yet, uh, I we-, I hope to see employer based, you know, helping out. You know, child, uh, care centers at the place of employment and things like that, that will help out. A: Uh-huh. B: What do you think, do you think we are, setting a trend?
+ Hypothesis: they are setting a trend 
+ Entailment: Unknown

**COPA** 
+ Premise: My body cast a shadow over the grass. Question: What’s the CAUSE for this?
+ Alternative 1: The sun was rising. 
+ Alternative 2: The grass was cut.
+ Correct Alternative: 1

**MultiRC** 
+ Paragraph: Susan wanted to have a birthday party. She called all of her friends. She has five friends. Her mom said that Susan can invite them all to the party. Her first friend could not go to the party because she was sick. Her second friend was going out of town. Her third friend was not so sure if her parents would let her. The fourth friend said maybe. The fifth friend could go to the party for sure. Susan was a little sad. On the day of the party, all five friends showed up. Each friend had a present for Susan. Susan was happy and sent each friend a thank you card the next week
+ Question: Did Susan’s sick friend recover? 
+ Candidate answers: 
	+ Yes, she recovered (T), 
	+ No (F), 
	+ Yes (T), 
	+ No, she didn’t recover (F), 
	+ Yes, she was at Susan’s party (T)

**ReCoRD** 
+ Paragraph: (CNN ) Puerto Rico on Sunday overwhelmingly voted for statehood. But Congress, the only body that can approve new states, will ultimately decide whether the status of the US commonwealth changes. Ninety-seven percent of the votes in the nonbinding referendum favored statehood, an increase over the results of a 2012 referendum, official results from the State Electorcal Commission show. It was the fifth such vote on statehood. "Today, we the people of Puerto Rico are sending a strong and clear message to the US Congress ... and to the world ... claiming our equal rights as American citizens, Puerto Rico Gov. Ricardo Rossello said in a news release. @highlight Puerto Rico voted Sunday in favor of US statehood
+ Query: For one, they can truthfully say, “Don’t blame me, I didn’t vote for them, ” when discussing the **placeholder** presidency 
+ Correct Entities: US

**RTE**  
+ Text: Dana Reeve, the widow of the actor Christopher Reeve, has died of lung cancer at age 44, according to the Christopher Reeve Foundation.
+ Hypothesis: Christopher Reeve had an accident. 
+ Entailment: False

**WiC** 
+ Context 1: Room and board. 
+ Context 2: He nailed boards across the windows.
+ Sense match: False

**WSC** 
+ Text: Mark told **Pete** many lies about himself, which Pete included in his book. **He** should have been more truthful. 
+ Coreference: False

#### Annotation and human performance
Existing tasks (WiC, MultiRC, RTE, and ReCoRD) have known estimates of human performance. Otherwise Amazon Mechanical Turk used to reannotate sample of each set. 

Estimated human performance:

| Task    | Metric | Performance |
| ------- | ------ | ----------- |
| BoolQ   | Acc    | 89.0        |
| CB      | F1/Acc | 95.8/98.9   |
| COPA    | Acc    | 100         |
| MultiRC | F1/EM  | 81.8/51.9   |
| ReCoRD  | F1/EM  | 91.7/91.3   |
| RTE     | Acc    | 93.6        |
| WiC     | Acc    | 80          |
| WSC     | Acc    | 100         |
* Acc - Accuracy
* F1 - harmonic mean between precision and recall
* EM - Exact Match

BERT based models are evaluated as a baseline against tasks and lag almost 20 points behind human performance. 