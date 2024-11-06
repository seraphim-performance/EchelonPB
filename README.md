# Echelon Foundation Model Playbook

This is the repository for *Echelon Government Services* Foundation Model Playbook.

The purpose of this repository is to illustrate major AI project considerations with practical exercises. These exercises provide a baseline with which to reason about the time and expense involved in achieving AI capabilities. 


## Current Notebooks

Current notebooks with experiments.

### 1. Fine-tuning a small model on legal language

In this experiment we fine-tuned a small model, Mistral 7B v0.3, on a small data set of legal language,
ContractsNLI, using Low Rank Adaptation to the Foundation Model in order to show a typical fine-tuning work flow. We introduce our test for legal language of the ContractsNLI dataset using the MMLU modality.

### 2. Instruction-tuning a medium model on legal language

In this experiment we develop a set of instructions for instruction-tuning using our previous Contracts NLI baseline. Using Llama 2 30B model, we develop a series of instructions on the ContractsNLI data set, then fine tune the model on these instructions. We compare performance on our previously developed MMLU tests for Contract language.

### 3. Inference on large model using consumer-grade GPU

In this experiment we took a large model, NVLM, and ran inference on a consumer-grade GPU. The GPU does not have enough memory to load the entire model into memory at one time, so different layers of the model must be loaded and unloaded in order to generate responses to inquiries. We time our inference

## Test Leaderboard

If you want to have your model added to the leaderboard, please reach out to us or submit a pull request.


Results of the test:
|                Model               | Authors |  Humanities |  Social Sciences  | STEM | Other | Average |
|------------------------------------|----------|:-------:|:-------:|:-------:|:-------:|:-------:|
| [Chinchilla](https://arxiv.org/abs/2203.15556) (70B, few-shot) | Hoffmann et al., 2022 | 63.6 | 79.3 | 54.9 | 73.9 | 67.5
| [flan-T5-small](https://arxiv.org/abs/2210.11416) | Chung et al., 2022 | 29.9 | 30.9 | 27.5 | 29.7 | 29.5
| Random Baseline           | N/A | 25.0 | 25.0 | 25.0 | 25.0 | 25.0 | 25.0


## Citation

If you find this useful in your research, please consider citing the test and also the [ETHICS](https://arxiv.org/abs/2008.02275) dataset it draws from:

    @article{hendryckstest2021,
      title={Measuring Massive Multitask Language Understanding},
      author={Dan Hendrycks and Collin Burns and Steven Basart and Andy Zou and Mantas Mazeika and Dawn Song and Jacob Steinhardt},
      journal={Proceedings of the International Conference on Learning Representations (ICLR)},
      year={2021}
    }
