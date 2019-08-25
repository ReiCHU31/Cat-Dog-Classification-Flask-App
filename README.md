# Building a Flask app on Image Classification of Dog/Cat Dataset implemented by Convolutional Neural Network (CNN)

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
    - How to connect frontend to backend
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

```shell
python3 -m pip install --user pipx
python3 -m pipx ensurepath

pipx install pipenv

# Install dependencies
pipenv install --dev

# Setup pre-commit and pre-push hooks
pipenv run pre-commit install -t pre-commit
pipenv run pre-commit install -t pre-push
```
Run the model by 

```shell
pipenv run flask run
```

## HOW IT WORK: CONVOLUTIONAL NEURAL NETWORK CNN

> In deep learning, a [convolutional neural network](https://en.wikipedia.org/wiki/Convolutional_neural_network) (CNN, or ConvNet) is a class of deep neural networks, most commonly applied to analyzing visual imagery. (Wiki)

For this project, we used **pre-trained model [MobileNetV2](https://keras.io/applications/#mobilenetv2)** from keras. MobileNetV2 is a model that was trained on a large dataset to solve a **similar problem to this project**, so it will help us to save lots of time on buiding low-level model and focus on the application.

* **Note:** You can learn more about CNN architecture in this [link](https://medium.com/@RaghavPrabhu/understanding-of-convolutional-neural-network-cnn-deep-learning-99760835f148).  

![](https://www.datascience.com/hs-fs/hubfs/CNN%202.png?width=650&name=CNN%202.png)

### 1. Load and preprocess images:

- Import **path, listdir** from **os library**.
- Find and save all the image path to **all_image_path** dataset is in folder `train`. 

## MODEL PERFOMANCE SUMARY
Our model has the accuracy of **97.79 %** for the train dataset and **97.32 %** for the test dataset. 

## FLASH APPLICATION
### Homepage
![](https://i.imgur.com/4CGnSNo.png)
### Example of results

![](https://i.imgur.com/PJ4f39B.png)

![](https://i.imgur.com/59cKpJQ.png)



## CONCLUSION

We successfully **built a deep neural network model** by implementing **Convolutional Neural Network (CNN)** to classify dog and cat images with very high accuracy **97.32 %**.
In addition, we also **built a Flask application** so user can upload their images and classify easily.
