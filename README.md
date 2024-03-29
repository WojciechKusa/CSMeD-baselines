# CSMeD-baselines
This repository contains baseline experiments from the paper "CSMeD: Bridging the Dataset Gap in Automated Citation Screening for Systematic Literature Reviews".
CSMeD dataset is described and available at: [WojciechKusa/systematic-review-datasets](https://github.com/WojciechKusa/systematic-review-datasets).

## Installation

Tested with Python 3.10.

### Requirements

Assuming you have `conda` installed, run:

```zsh
$ conda create -n csmed python=3.10
$ conda activate csmed
(csmed)$ pip install -r requirements.txt
```

## Running

### CSMeD-Cochrane

To run the experiments on CSMeD-Cochrane, run:

```zsh
(csmed)$ python experiments/csmed_cochrane/csmed_cochrane_retrieval.py
```

Results of the baseline experiment are available under the following URL [csmed-cochrane-baseline-results.zip](https://www.dropbox.com/scl/fi/a1a4jr1wh0gwari5sqvcw/csmed-cochrane-baseline-results.zip?rlkey=7yi1dk2wpw6nb4gnaccbp6191&dl=0)

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
