# Bulding a Flask app on Image Classification of Dog/Cat Dataset implemented by Convolutional Neural Network (CNN)

### Phuong T.M. Chu & Minh H. Nguyen
This is the project that we finished after the 6th week of studying **Machine Learning**.

<p align="center">
  <img width="760" height="400" src="https://miro.medium.com/max/1838/1*oB3S5yHHhvougJkPXuc8og.gif">
</p>




## INTRODUCTION
### 1. Dataset
**Dogs vs. Cats** [dataset](https://www.kaggle.com/c/dogs-vs-cats/data) provided by  Microsoft Research contains 25,000 images of dogs and cats with the labels 
* 1 = dog
* 0 = cat 

### 2. Project goals
- Building a **deep neural network** using **TensorFlow** to classify dogs and cats images.

- Making a **Flask application** so user can upload their photos and receive the prediction.

### 3. Project plan

During this project, we need to answer these following questions:

**A. Build the model**
- How to import the data
- How to preprocess the images
- How to create a model
- How to train the model with the data
- How to export the model
- How to import the model
    
**B. Build the Flask app**

**Front end**
- HTML
    - How to connetc frontend to backend
    - How to draw a number on HTML
    - How to make UI looks good

**Back end**
- Flask
    - How to set up Flask
    - How to handle backend error
    - How to make real-time prediction
    - Combine the model with the app
## SETUP ENVIRONMENT
In order to run our model on a Flask application locally, you need to clone this repository and then set up the environment by these following commands:

```sh
python3 -m pip install --user pipx
python3 -m pipx ensurepath

pipx install pipenv

# Install dependencies
pipenv install --dev

# Setup pre-commit and pre-push hooks
pipenv run pre-commit install -t pre-commit
pipenv run pre-commit install -t pre-push
```
## MODEL PERFOMANCE SUMARY

## FLASH APPLICATION

## CONCLUSION



