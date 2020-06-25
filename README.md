# Potato Dieses Detection System #

This repo contains the code for Potato Dieses Detection System with the help of transfer learning over pretrained model. altough we can use various models but we are providing results of only mobilenet model you can experiment with all other models.

### Key Points of the project ###
* Models used     - **Xception, Inception-v3, OverFeat, ResNet50, VGG16, VGG19, InceptionResNetv2 and MobileNet.
* Weights used    - **ImageNet**
* Classifier used - **Logistic Regression**


### Dependencies ###
* Theano or TensorFlow `sudo pip install theano` or `sudo pip install tensorflow`
* Keras `sudo pip install keras`
* NumPy `sudo pip install numpy`
* matplotlib `sudo pip install matplotlib` and you also need to do this `sudo apt-get install python-dev`
* seaborn `sudo pip install seaborn`
* h5py `sudo pip install h5py`
* scikit-learn `sudo pip install scikit-learn`

### System requirements
* This project is trained and tested on ubuntu 18.04 but you can also use windows 10 for the same.

### Licence
MIT License

### Usage ###
* arrange dataset serial wise           - `python nameSerializer.py`
* Organize dataset                      - `python name_data_spliter.py`
* Feature extraction using CNN          - `python extract_features.py`
* Train model using Logistic Regression - `python train.py`

### Folders ###
* features   - it contains the google drive link for features extracted during training.
* Data 		 - it contains the link for pre processed data
* conf       - it contains the common config that you can use ommonly for all models by changing model name.

### Statistics ###
The below tables shows the accuracies obtained for every Deep Neural Net model used to extract features from potato leaves dataset over customized settings.

* Result-1
  
  * test_size  : **0.10**
  * classifier : **Logistic Regression**
  
| Model             | Rank-1 accuracy | Rank-5 accuracy |
|-------------------|-----------------|-----------------|
| Xception          | 97.06%          | 99.26%      	|
| Inception-v3      | 96.32%          | 99.26%          |
| VGG16             | 85.29%          | 98.53%          |
| VGG19             | 88.24%          | 99.26%          |
| ResNet50          | 56.62%          | 90.44%          |
| MobileNet         |98.53%           | 100.00%         |
| InceptionResNetV2 | 91.91%          | 98.53%          |


* Result-2
  
  * test_size  : **0.30**
  * classifier : **Logistic Regression**

| Model              | Rank-1 accuracy | Rank-5 accuracy |
|--------------------|-----------------|-----------------|
| Xception           | 93.38%          | 99.75%          |
| Inception-v3       | 96.81%          | 99.51%          |
| VGG16              | 88.24%          | 99.02%          |
| VGG19              | 88.73%          | 98.77%          |
| ResNet50           | 59.80%          | 86.52%          |
| MobileNet          | 96.32%          | 99.75%          |
| Inception ResNetV2 | 88.48%          | 99.51%          |


### Steps to done prediction ###
1. dowlnoad pre trained features using g-drive link in features folder or from link given below

https://drive.google.com/file/d/1WjqX1Y6YRlWtL1Ze1Aqba3zkdKj9tK9h/view?usp=sharing

2. run test.py python package


### Steps to training ###
1. either download dataset from the link in data folder or from link given below

https://drive.google.com/drive/folders/1f4o5VdMfdy1qihaO0YkOe-ciwcQuuXnE?usp=sharing
or,
you can use your own pre-processed data

2. modify conf file in conf folder 

3. run conf file