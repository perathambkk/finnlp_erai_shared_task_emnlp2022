# finnlp_erai_shared_task_emnlp2022
The PromptShots System to a Shared Task on Evaluating the Rationales of Amateur Investors (ERAI) @EMNLP-2022 https://sites.google.com/nlg.csie.ntu.edu.tw/finnlp-2022-emnlp/erai-shared-task?authuser=0.

The pairwise ranking code utilizes the InstructGPT language model (https://openai.com/blog/instruction-following/ -- few-shot prompts on the `text-davinci-002' model) while costs within the OpenAI API free tier budget.

For a lecture in prompt-based learning, please see https://www.youtube.com/watch?v=8HwHGGb1zpQ (UMass CS685 S22 (Advanced NLP) #12: Prompt-based learning
) or https://www.youtube.com/watch?v=TE6urdkTR4I (CMU Advanced NLP 2021 (10): Prompting + Sequence-to-sequence Pre-training). 

For an awesome list on prompts, please see https://github.com/thunlp/PromptPapers or other awesome repos around GitHub.

For the unsupervised ranking task, we utilized many financial pretrained models and (<a href="https://github.com/perathambkk/probabilistic-lexicon-classification/tree/4b4dc37ca16923bc57d7de9f81e19e9850f0d9d8">Bayesian-fitted🍴</a>) lexicons. Then, we intuitively weighed them using the MaxEnt principle. 

Presentations: https://docs.google.com/presentation/d/1-rutQf-bHpDtI_c6Y78_FFWPc53zscMis5b1y7-bzoE/edit?usp=sharing

PS. Our base submission, when using just the bayesian lexicon from the best submission, can score very similar (a little bit ~0.5% lower MPP) compared to the best submission. POS feature and tone features add only a little bit of performance. (I haven't reproduced the numbers to be aligned with the official shared task results so this is probably still roughly speaking with some comparable evidences.)
