
General machine learning project repo structure:
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

my repo structure for learning pytorch:
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

gitignore guide:
    Easiest Solution — Use a Template
    GitHub has a ready-made Python .gitignore template. When creating a repo:
    New repo → Add .gitignore → select "Python" template
    It automatically covers most of these cases. Then you just add your project specific ones like datasets/ on top.

pytorch learning journey:
    25/02/2026: I tried using vs code jupyter to learn pytorch, but my vs code had some issues and i didn't know how to structure ML projects properly, so learned how to setup vs code, installed few extensions, used gitbash to create files and keep track of them, then learned tensors, linspace.
    27/02/2026: matrix multiplication, datasets, transform.
    28/02/2026: Saturday is a day off for me, played rdr2 for the whole day.
    01/03/2026: Sunday, learned stacking, squeezing, unsqueezing, learned how to use gpu using cuda, built a linear regression model, where i trained the data, tested it, visualized it, saved the parameters using torch.save
    02/03/2026: Monday, implemented logistic regression, saved the parameters, now i am moving on to learning CNNs and RNNs.
    ------------------------------------------------------------------------------------------------------------------------------
    12/03/2026: implemented cat or nocat dataset, strenthened my understanding, learned how to load h5 files, learned how to run the model using different hyperparameters using a user defined function for training the model and everytime you run the cell, the model is reinitialized and trained with the new hyperparameters.

