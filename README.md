# CSMeD-baselines
Baseline experiments from the paper "CSMeD: Bridging the Dataset Gap in Automated Citation Screening for Systematic Literature Reviews"


## Installation

### Requirements

Assuming you have `conda` installed, run:

```zsh
$ conda create -n csmed python=3.10
$ conda activate csmed
(csmed)$ pip install -r requirements.txt
```

## Running

### CSMeD-FT

Experiments on CSMeD-FT consist of two parts: (1) fine-tuned classification Transformer models and (2) zero-shot prompting via OpenAI models.

To run the classification experiments, run:

```zsh
(csmed)$ python experiments/csmed_ft/full_text_classification.py
```

To run the zero-shot prompting experiments, run:

```zsh
(csmed)$ python experiments/csmed_ft/full_text_prompting.py
```
