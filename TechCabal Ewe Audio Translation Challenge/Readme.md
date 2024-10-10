# 0TechCabal Ewè Audio Translation Challenge - Winning Solution 🏆

Welcome to the repository containing my winning solution for the [TechCabal Ewè Audio Translation Challenge](https://zindi.africa/competitions/techcabal-ewe-audio-translation-challenge). This solution is broken down into two notebooks that explain each step of the process, from data preprocessing to model training, inference, and pseudo labeling.

## 📑 Notebooks

### 1. [Notebook 1: Preprocessing and Initial Model Training](techcabal1.ipynb)

In the first notebook, I focus on building the foundational model:

- **Data loading and preprocessing**: Using techniques like audio trimming, normalization, and extracting MFCC features.
- **Model architecture**: Introducing **FemiNet**, a custom lightweight CNN model inspired by xresnet architecture.
- **Training**: Applying FastAI's `fit_one_cycle` method for efficient model training.
- **Inference**: Generating predictions and creating a submission file for Zindi.

[👉 View Notebook 1 here](notebook_1.ipynb)

### 2. [Notebook 2: Pseudo Labels and Enhanced Training](techcabal2.ipynb)

In the second notebook, we improve the model using pseudo labels:

- **Pseudo labeling**: Adding high-confidence predictions from Notebook 1 to the training set for improved accuracy.
- **Retraining**: Using both original and pseudo-labeled data to train a more robust model using FastAI's `fit_flat_cos`
- **Efficiency**: Calculating the inference speed to ensure real-time application viability.

[👉 View Notebook 2 here](notebook_2.ipynb)

## 🔧 Key Features

- **FemiNet**: A custom, lightweight model built specifically for this challenge, focusing on efficiency.
- **Pseudo Labels**: Leveraging confident predictions to further enhance model performance.
- **Real-time Inference**: Achieved average inference time of ~40 milliseconds per audio file on parallel processing.

## 🛠️ Dependencies

Make sure to install the necessary libraries before running the notebooks:

- `librosa`
- `fastai`
- `noisereduce`
- `torch`
- `pandas`

### 📈 Results

The final model achieved:

- **Fast inference speed**: ~40 milliseconds per file
- **Optimized for edge deployment**: 6.5MB model size, running inference on CPUs without pre-trained models.

Feel free to explore the notebooks, try out the solution, or contribute to further improvements.

### 👏 Acknowledgments

A big thanks to **Zindi**, **Umbaji** and **TechCabal** for organizing this challenge!
