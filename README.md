# finnlp_erai_shared_task_emnlp2022
The PromptShots System to a Shared Task on Evaluating the Rationales of Amateur Investors (ERAI) @EMNLP-2022 https://sites.google.com/nlg.csie.ntu.edu.tw/finnlp-2022-emnlp/erai-shared-task?authuser=0.

The pairwise ranking code utilizes the InstructGPT language model (https://openai.com/blog/instruction-following/ -- few-shot prompts on the `text-davinci-002' model) while costs within the OpenAI API free tier budget. Our submission on this track ranking 3rd on the maximal loss (ML) pairwise accuracy.

For a lecture in prompt-based learning, please see https://www.youtube.com/watch?v=8HwHGGb1zpQ (UMass CS685 S22 (Advanced NLP) #12: Prompt-based learning
) or https://www.youtube.com/watch?v=TE6urdkTR4I (CMU Advanced NLP 2021 (10): Prompting + Sequence-to-sequence Pre-training). 

For an awesome list on prompts, please see https://github.com/thunlp/PromptPapers or other awesome repos around GitHub.

For the unsupervised ranking task, we utilized many financial pretrained models and (<a href="https://github.com/perathambkk/probabilistic-lexicon-classification/tree/4b4dc37ca16923bc57d7de9f81e19e9850f0d9d8">Bayesian-fitted🍴</a>) lexicons. Then, we intuitively weighed them using the MaxEnt principle. We won this shared task competition track on maximal potential profit (MPP) pairwise accuracy ranking. I just forgot to flip the sign for the maximal loss (ML) pairwise accuracy ranking submissions as I didn't even look at the scores in the training set, just submitted.

Presentations: https://docs.google.com/presentation/d/1-rutQf-bHpDtI_c6Y78_FFWPc53zscMis5b1y7-bzoE/edit?usp=sharing

PS. Our base submission, when using just the bayesian lexicon from the best submission, can score very similar (a little bit ~0.5% lower MPP) compared to the best submission. POS feature and tone features add only a little bit of performance. (I haven't reproduced the numbers to be aligned with the official shared task results so this is probably still roughly speaking with some comparable evidences.)

## Citation
A link to the [paper](https://aclanthology.org/2022.finnlp-1.pdf#page=116) and its [ArXiv](https://arxiv.org/abs/2301.06606).

### Cite this paper

Wiriyathammabhum, P. (2022, December). PromptShots at the FinNLP-2022 ERAI Task: Pairwise Comparison and Unsupervised Ranking. In Proceedings of the Fourth Workshop on Financial Technology and Natural Language Processing (FinNLP) (pp. 104-110).

```bixtex
@inproceedings{wiriyathammabhum2022promptshots,
  title={PromptShots at the FinNLP-2022 ERAI Task: Pairwise Comparison and Unsupervised Ranking},
  author={Wiriyathammabhum, Peratham},
  booktitle={Proceedings of the Fourth Workshop on Financial Technology and Natural Language Processing (FinNLP)},
  pages={104--110},
  year={2022}
}
```
