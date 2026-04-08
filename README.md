# ITW-dataset

## Dataset

This repository includes a local research copy of the **In-the-Wild (ITW) framing dataset** introduced in:

[**Valeria Pastorino, Jasivan Alex Sivakumar, and Nafise Sadat Moosavi. _Decoding News Narratives: A Critical Analysis of Large Language Models in Framing Detection_.**](https://arxiv.org/abs/2402.11621)

If you use this dataset, please cite the paper above.

### Contents

The dataset file used in this repository is:

- `dataset_ITW_26.xlsx`

It contains news headlines and binary framing labels used for the experiments in this project.

### Dataset summary

The ITW dataset contains:

- **157** news headlines
- **83** framed headlines
- **74** non-framed headlines

The headlines span diverse topics, including weather, public health, migration, and European affairs. :

### Provenance

Headlines were
- collected from the **NewsFrames** website
- sampled from mainstream news outlets, including **BBC**, **The Guardian**, and **Daily Mail**

### Annotation

All headlines in the ITW dataset were annotated and checked by domain experts following the framing definition used in the study. 

### Use in this repository

This repository includes the dataset as a working research copy for reproducibility of the experiments and analyses implemented here.

# Prompts

This repository includes the prompt set used for framing-detection experiments:

- `prompts.txt`

The prompt file contains the evaluation prompts organised by prompting setup, including:

- zero-shot prompts
- zero-shot prompts with alternative wording
- zero-shot prompts with a framing definition
- few-shot prompts with 2 examples
- few-shot prompts with 8 examples
- mixed-domain, in-domain, and cross-domain few-shot variants
- explanation-based versions of each prompt

These prompts are intended for experiments on binary framing detection, where the model is asked to decide whether a headline or claim is framed and, in some variants, provide an explanation in JSON format.
