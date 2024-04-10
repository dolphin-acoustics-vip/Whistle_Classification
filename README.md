# Species Classifiers
This repository is a collection of attempts at using machine learning models to classify the whistle contours of dolphin species.

## Set up

The easiest way to set up and run the jupyter notebook files in this folder is by creating a virtual environment for this project. This way you can avoid the so-called "dependency-hell". For a tutorial head to this [link](https://github.com/dolphin-acoustics-vip/Workflow_Tutorials#creating-a-virtual-environment-using-virtualenv-python-specific).

The Python version used in this project is Python 3.9.10

Each file is self contained, and they don't require any extra modules to import or download apart from those pippable in the requirements.txt file.

The code here is fully os-independent, so you don't have to worry whether you are running on a windows os or IOS or linux, they will all work. But do make sure you set up a virtual environment correctly before continuing.

## What does each file do?

Quick overview:

[Transfer_Learning_Xception.ipynb](https://github.com/dolphin-acoustics-vip/Whistle_Classification/blob/main/Transfer_Learning_Xception.ipynb): This jupyter notebook uses a technique called Transfer Learning to train a species classifier. The model transferred is [Xception](https://arxiv.org/abs/1610.02357). [Here](https://towardsdatascience.com/top-10-cnn-architectures-every-machine-learning-engineer-should-know-68e2b0e07201) are other models the user can try.

[whistle_classifier.ipynb](https://github.com/dolphin-acoustics-vip/Whistle_Classification/blob/main/whistle_classifier.ipynb): This jupyter notebook teaches the user the main workflow of training a CNN. It also allows the user to build and test their own CNNs. This has been the main file used to generate student-made models and classifiers.

The above files also include:
- Training, validation and testing data generators
- Building and training of models
- Evaluation of models using classification reports and confusion matrices

### CountourClassifier
[ContourClassifier.ipynb](https://github.com/dolphin-acoustics-vip/Whistle_Classification/blob/main/ContourClassifier.ipynb) is some exploratory code written as the basis for a more formal investigation of repertoire classification using unsupervised methods. It seeks to serve as an alternative to ARTWarp for unsupervised whistle clustering. See below for an exampleof its output.

![image](https://github.com/dolphin-acoustics-vip/Whistle_Classification/assets/60829930/6512a847-eb95-4df0-83e6-098ad2bc7819)

