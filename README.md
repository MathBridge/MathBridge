# MathBridge: A Large Corpus Dataset for Translating Spoken Mathematical Expressions into $LaTeX$ Formulae for Improved Readability 🧮

## Dataset
The MathBridge dataset is available on huggingface🤗.

- [MathBridge in huggingface🤗 dataset](https://huggingface.co/datasets/aaai25withanonymous/MathBridge)

## Fine-tuned Models
We have fine-tuned a range of models on the MathBridge. These models are available for download and use on Hugging Face.

### Available Models:
- **MathBridge T5 Small**: [huggingface🤗 model](https://huggingface.co/aaai25withanonymous/MathBridge_T5_small)
- **MathBridge T5 Base**: [huggingface🤗 model](https://huggingface.co/aaai25withanonymous/MathBridge_T5_base)
- **MathBridge T5 Large**: [huggingface🤗 model](https://huggingface.co/aaai25withanonymous/MathBridge_T5_large)
- **MathBridge BART Base**: [huggingface🤗 model](https://huggingface.co/aaai25withanonymous/MathBridge_BART_base)
- **MathBridge BART Large**: [huggingface🤗 model](https://huggingface.co/aaai25withanonymous/MathBridge_BART_large)
- **MathBridge mBART**: [huggingface🤗 model](https://huggingface.co/aaai25withanonymous/MathBridge_mBART)

### Experiment Resluts:

| Models            | BLEU (↑) | sBLEU (↑) | Rouge1 (↑) | CER (↓) | WER (↓) | BLEU (↑) | sBLEU (↑) | Rouge1 (↑) | CER (↓) | WER (↓) |
|-------------------|---------|----------|-----------|-------|--------|--------------|---------------|----------------|------------|-------------|
| **BART-base**     | 0.29    | 31.3     | 0.64      | 0.51  | 0.68   | 0.26         | 38.7          | 0.64           | 0.42       | 0.58        |
| **BART-large**    | 0.29    | 31.0     | 0.61      | 0.52  | 0.69   | 0.31         | 35.2          | 0.63           | 0.48       | 0.54        |
| **T5-small**      | 0.12    | 14.9     | 0.39      | 1.25  | 1.35   | 0.31         | 38.4          | 0.75           | 0.35       | 0.55        |
| **T5-base**       | 0.05    | 6.05     | 0.21      | 2.63  | 2.53   | 0.28         | 36.6          | 0.67           | 0.50       | 0.74        |
| **T5-large**      | 0.04    | 4.77     | 0.20      | 1.92  | 1.95   | **0.36**     | **46.8**      | **0.82**       | **0.26**   | **0.49**    |
| **mBART-large-50**| 0.21    | 16.9     | 0.42      | 0.90  | 1.37   | 0.24         | 23.6          | 0.59           | 0.58       | 0.74        |
| **GPT-3.5(w/o p)**| 0.24    | 38.9     | 0.77      | 0.43  | 0.55   | -            | -             | -              | -          | -           |
| **GPT-3.5(w/ p)** | 0.44    | 52.3     | 0.88      | 0.19  | 0.37   | -            | -             | -              | -          | -           |
| **Average**       | 0.16    | 17.4     | 0.41      | 1.28  | 1.42   | 0.29         | 36.5          | 0.68           | 0.43       | 0.60        |
| **Improvement**   | -       | -        | -         | -     | -      | 76.0%        | 109.0%        | 65.9%          | 66.4%      | 57.5%       |

**Notes:** Evaluation of the performance of PLMs' original and MathBridge-enhanced responses using the test dataset. 'sBLEU' refers to sacreBLEU. The averages for the 'Original' column exclude GPT-3.5 Models.
