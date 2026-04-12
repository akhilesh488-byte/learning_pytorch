
This repository consists of classic deep learning projects implemented using PyTorch. The main goal of this repository is to learn how to structure deep learning projects, and to learn how to use PyTorch for building and training deep learning models.

This repository is a work in progress, and I will be adding more projects and improving the existing ones as I learn more about deep learning and PyTorch.

This repository is not meant to be a complete guide to deep learning or PyTorch, but rather a collection of projects that I have implemented as part of my learning journey. I will be sharing my thoughts and experiences as I learn and implement these projects.

This repository consists of the following notebooks:

1. **`tensors_and_datasets.ipynb:`** Covers basic operations on tensors and datasets, and how to utilize them within PyTorch.
2. **`linear_regression.ipynb:`** Implementation of linear regression using synthetic data.
3. **`logistic_regression.ipynb:`** Implementation of logistic regression using the `make_circles` dataset from Scikit-Learn. 
   * **Loss Function:** `BCEWithLogitsLoss`
   * **Performance:** Achieved a test loss of `0.16`.
4. **`cat_or_notcat.ipynb:`** An Artificial Neural Network (ANN) built with a custom architecture to classify images as "cat" or "non-cat".
5. **`hand_signs.ipynb:`** A Convolutional Neural Network (CNN) built to classify hand signs.
   * **Performance:** Achieved a test accuracy of `90%`.
6. **`animals10.ipynb:`** A CNN model utilizing the ResNet18 architecture to classify animals from the Animals-10 dataset.
   * **Performance:** Achieved a test accuracy of `96.5%`.
7. **`face_recognition.ipynb:`** Evaluation of the FaceNet model using the Inception ResNet V1 architecture on the LFW (Labeled Faces in the Wild) dataset.
   * **Performance:** Achieved a test accuracy of `96.3%`.


ML project repository structure that works on almost all ML/DL projects:
```
    project/
        data/
            dataset.py       # your Dataset class and dataloader logic
        model/
            model.py         # your model architecture
        utils/
            transforms.py    # your transforms
            helpers.py       # any utility functions
        config.py            # all your settings in one place (paths, hyperparameters)
        train.py             # training loop
        evaluate.py          # evaluation logic
        README.md            # project overview and instructions
        .gitignore           # to ignore unnecessary files and folders

```

Since I am learning pytorch and learning to implement DL models I will be using the following repo structure:
```
    learning_pytorch/
        │
        ├── notebooks/                  ← only .ipynb files here
        │   ├── tensors_and_datasets.ipynb
        │   ├── linear_regression.ipynb
        │   ├── logistic_regression.ipynb
        │   └── cat_or_notcat.ipynb
        │
        ├── saved_models/               ← all .pth files here
        │   ├── linear_model.pth
        │   └── logistic_regression_model.pth
        │
        ├── datasets/                   ← all datasets here
        │   └── cat_or_notcat/
        │       ├── train_catvnoncat.h5
        │       └── test_catvnoncat.h5
        │
        ├── .gitignore
        ├── requirements.txt
        └── README.md
```
First thing to do when you have created a new repo is to add a .gitignore file, because you don't want to accidentally commit large files like datasets or saved models, and you also don't want to commit unnecessary files like __pycache__ or .ipynb_checkpoints.

gitignore guide:
    Easiest Solution — Use a Template
    GitHub has a ready-made Python .gitignore template. When creating a repo:
    New repo → Add .gitignore → select "Python" template
    It automatically covers most of these cases. Then you just add your project specific ones like datasets/ on top.

Second thing to do is to create a requirements.txt file to list all the packages that you are going to use along with their versions to avoid compatibility issues in your project and you can easily install the packages using pip install -r requirements.txt.

Third thing to do is create venv and install all the necessary packages to keep the repo organized and to avoid compatibility issues with other projects.

## Getting Started

1. **Clone the repo:** `git clone https://github.com/akhilesh488-byte/learning_pytorch.git`
2. **Setup Venv:** `python -m venv venv` and activate it.
3. **Install Dependencies:** `pip install -r requirements.txt`
4. **Prepare Data:** Create a `/datasets` folder and download the links provided below.

I have used datasets cat_nocat, hand_signs from my coursera assignments taught by deeplearning.ai, and animals10 and lfw datasets from kaggle.

The datasets can be downloaded from the following links:
    1. animals10 dataset: https://www.kaggle.com/datasets/alessiocorrado99/animals10
    2. lfw dataset: https://www.kaggle.com/datasets/jessicali9530/lfw-dataset

