---
date: 2021-07-14
---
[Link](https://arxiv.org/abs/2107.03374)


## Authors
[[Mark Chen]], [[Jerry Tworek]], [[Heewoo Jun]], [[Qiming Yuan]], [[Henrique Ponde de Oliveira Pinto]], [[Jared Kaplan]], [[Harri Edwards]], [[Yuri Burda]], [[Nicholas Joseph]], [[Greg Brockman]], [[Alex Ray]], [[Raul Puri]], [[Gretchen Krueger]], [[Michael Petrov]], [[Heidy Khlaaf]], [[Girish Sastry]], [[Pamela Mishkin]], [[Brooke Chan]], [[Scott Gray]], [[Nick Ryder]], [[Mikhail Pavlov]], [[Alethea Power]], [[Lukasz Kaiser]], [[Mohammad Bavarian]], [[Clemens Winter]], [[Philippe Tillet]], [[Felipe Petroski Such]], [[Dave Cummings]], [[Matthias Plappert]], [[Fotios Chantzis]], [[Elizabeth Barnes]], [[Ariel Herbert-Voss]], [[William Hebgen Guss]], [[Alex Nichol]], [[Alex Paino]], [[Nikolas Tezak]], [[Jie Tang]], [[Igor Babuschkin]], [[Suchir Balaji]], [[Shantanu Jain]], [[William Saunders]], [[Christopher Hesse]], [[Andrew N. Carr]], [[Jan Leike]], [[Josh Achiam]], [[Vedant Misra]], [[Evan Morikawa]], [[Alec Radford]], [[Matthew Knight]], [[Miles Brundage]], [[Mira Murati]], [[Katie Mayer]], [[Peter Welinder]], [[Bob McGrew]], [[Dario Amodei]], [[Sam McCandlish]], [[Ilya Sutskever]], [[Wojciech Zaremba]]
## Abstract
We introduce Codex, a GPT language model fine-tuned on publicly available code from GitHub, and study its Python code-writing capabilities. A distinct production version of Codex powers GitHub Copilot. On HumanEval, a new evaluation set we release to measure functional correctness for synthesizing programs from docstrings, our model solves 28.8% of the problems, while GPT-3 solves 0% and GPT-J solves 11.4%. Furthermore, we find that repeated sampling from the model is a surprisingly effective strategy for producing working solutions to difficult prompts. Using this method, we solve 70.2% of our problems with 100 samples per problem. Careful investigation of our model reveals its limitations, including difficulty with docstrings describing long chains of operations and with binding operations to variables. Finally, we discuss the potential broader impacts of deploying powerful code generation technologies, covering safety, security, and economics. 

## Links
[[HumanEval]]
