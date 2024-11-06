# 1. Fine-tuning a small model on legal language

In this experiment we fine-tuned a small model, Mistral 7B v0.3, on a small data set of legal language,
ContractsNLI, using Low Rank Adaptation to the Foundation Model in order to show a typical fine-tuning work flow. We introduce our test for legal language of the ContractsNLI dataset using the MMLU modality.

## Citation

    @article{mistral7b,
      title={Mistral 7B},
      author={Albert Q. Jiang, Alexandre Sablayrolles, Arthur Mensch, Chris Bamford, Devendra Singh Chaplot, Diego de las Casas, Florian Bressand, Gianna Lengyel, Guillaume Lample, Lucile Saulnier, Lélio Renard Lavaud, Marie-Anne Lachaux, Pierre Stock, Teven Le Scao, Thibaut Lavril, Thomas Wang, Timothée Lacroix, William El Sayed},
      link={https://arxiv.org/abs/2310.06825},
      year={2023}
    }

    @article{lora,
      title={LoRA: Low-Rank Adaptation of Large Language Models},
      author={Edward J. Hu, Yelong Shen, Phillip Wallis, Zeyuan Allen-Zhu, Yuanzhi Li, Shean Wang, Lu Wang, Weizhu Chen},
      link={https://arxiv.org/abs/2106.09685},
      year={2021}
    }

    @article{mmmlu,
      title={Measuring Massive Multitask Language Understanding},
      author={Dan Hendrycks, Collin Burns, Steven Basart, Andy Zou, Mantas Mazeika, Dawn Song, Jacob Steinhardt},
      link={https://arxiv.org/abs/2009.03300},
      year={2020}
    }
