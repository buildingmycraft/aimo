# aimo

Developing a solution to the Artificial Intelligence Mathematical Olympiad challenge.

## Developer Notes

### Local environment setup

To install and activate the development environment using conda:
```bash
conda env create -f environment.yml --no-builds
conda activate aimo
```

### Data download

#### Kaggle

We'll be downloading data from kaggle using the kaggle cli, installed already in the conda environment. However, we also need to set up our kaggle credentials, following the instructions [here](https://github.com/Kaggle/kaggle-api/blob/main/docs/README.md#api-credentials).

The kaggle dataset has already been committed to this repo for convenience, given it's small size. However, to (re)download the kaggle dataset using the kaggle api, you can run:

```bash
kaggle competitions download -c ai-mathematical-olympiad-progress-prize-2
unzip ai-mathematical-olympiad-progress-prize-2.zip -d kaggle
```

We'll also be using the `awsaf49/math-qsa-dataset` which you can download via:

```bash
kaggle datasets download awsaf49/math-qsa-dataset
mkdir external-data
unzip math-qsa-dataset.zip -d external-data/math-qsa-dataset
```