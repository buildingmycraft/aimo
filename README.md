# aimo

Developing a solution to the Artificial Intelligence Mathematical Olympiad challenge.

## Developer Notes

### Local environment setup

To install the development environment using conda:
```bash
conda env create -f environment.yml
```

### Data download

#### Kaggle

The kaggle dataset has already been committed to this repo for convenience.

However, to (re)download the kaggle dataset using the kaggle api, you'll need to set up your kaggle credentials (follow the official instructions [here](https://github.com/Kaggle/kaggle-api/blob/main/docs/README.md#api-credentials)), then run:

```bash
kaggle competitions download -c ai-mathematical-olympiad-progress-prize-2
unzip ai-mathematical-olympiad-progress-prize-2.zip -d kaggle
```