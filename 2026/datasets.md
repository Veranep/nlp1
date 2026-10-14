---
layout: default
title: Datasets
permalink: /2026/datasets/
tagline: 2026
---

Here is a list of datasets/tasks from which you can choose what to work throughout the practicals. You should keep your choice throughout all 3 practicals. 

Other datasets are also possible, but a) it should be possible to frame the task as a form of K-way classification, and b) your TA should explicitly approve your choice and add it to this list (this is to minimise situations in which the choice of dataset seriously compromise your ability to achieve the course's learning goals).


- **Sentiment Classification**: Determines the overall sentiment expressed in a piece of text, typically as positive, negative, or neutral. Some datasets you could use: [SST-2 (Stanford Sentiment Treebank)](https://huggingface.co/datasets/stanfordnlp/sst2) or [IMDb](https://huggingface.co/datasets/mteb/imdb) which focus on binary sentiment classification (positive/negative) of movie reviews.
IMDb: Binary sentiment classification of movie reviews.
- **Emotion Classification**: Identifies the specific emotion conveyed in text, such as joy, anger, sadness, fear, or surprise. You could use the [GoEmotions](https://www.kaggle.com/datasets/debarshichanda/goemotions/data) dataset, which provides fine-grained emotion classification across 27 emotion categories based on Reddit comments. Another option is the [ISEAR (International Survey on Emotion Antecedents and Reactions)](https://huggingface.co/datasets/gsri-18/ISEAR-dataset-complete) dataset which contains personal accounts of emotional experiences, labeled with 7 different emotions.
- **Natural Language Inference (NLI)**: Determines the logical relationship between two pieces of text—typically whether one entails, contradicts, or is neutral with respect to the other. Some datasets you could use [MNLI (Multi-Genre Natural Language Inference)](https://huggingface.co/datasets/nyu-mll/multi_nli) or [SNLI (Stanford Natural Language Inference)](https://huggingface.co/datasets/stanfordnlp/snli), which provide premise-hypothesis pairs, and whether they are entailing, contradicting or neutral to each other.
- **Bias Classification**: Determines whether word choice to refer to (groups of) individuals consists of biased language use, and/or can be used to uncover biases present in the architecture. The [Dutch Government Data for Bias Detection (DGDB)](https://huggingface.co/datasets/milenamileentje/Dutch-Government-Data-for-Bias-detection) dataset is a dataset of texts from the Dutch House of Representatives which enables binary (biased vs. unbiased) bias classification. Note that even though the classification is binary, the dataset is imbalanced and examples are quite tricky. The [Bias in Bios](https://huggingface.co/datasets/LabHC/bias_in_bios) dataset provides short gendered bios of people and their occupations, which can be used to evaluate whether models are more/less successful at selecting the correct occupation for certain gender-occupation pairs.
- **Stance Detection**: Identifies the stance on a particular issue or about a particular topic expressed in a piece of text, typically as in favor, neutral or against. A dataset you could use is [TweetEval](https://huggingface.co/datasets/cardiffnlp/tweet_eval), a dataset of tweets labeled with their stance on a set of topics, such as atheism, climate change and feminism, as well as sentiment and emotions.
- **Paraphrase Detection**: Determines whether two sentences are paraphrases of each other or one has a different meaning than the other. You could use the [Quora Question Pairs](https://huggingface.co/datasets/AlekseyKorshuk/quora-question-pairs) or the [PAWS: Paraphrase Adversaries from Word Scrambling](https://huggingface.co/datasets/google-research-datasets/paws) dataset. Note that the second one is extra difficult: It contains sentence pairs that use (nearly) the exact same words.
- **Multiple Choice Question Answering (MCQA)**: Selects the correct answer from a set of candidate options based on the information provided in a question and, when applicable, a supporting passage. You could use the [MMLU (Massive Multitask Language Understanding)](https://huggingface.co/datasets/cais/mmlu) dataset (or its multilingual counterpart [MMMLU](https://huggingface.co/datasets/openai/MMMLU)) which covers multiple-choice questions across a broad range of academic and professional subjects.

> MCQA _can_ be framed as classification, but it requires a change in the architecture presented in tutorial 1; this is not to discourage you from this choice, but you should be aware of it, perhaps discuss this with your TA to see if you are comfortable with the level.


