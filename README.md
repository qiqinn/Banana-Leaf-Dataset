# Banana-Leaf-Diseases


This model predicts banana diseases.This model prediction accuracy is `98.75%`(test data) && `96.25%` accuracy (validation_data)
## Data preprocessing
The data_augmentation model uses for dataset preprocessing.
* Flip (horizontal)
* Roation (0.2)
* Zoom (0.2)
* Height (0.2)
* Width (0.2)
* Rescaling (0-255)-(0-1)

## Images
![screenshot](https://github.com/HSAkash/Banana-Leaf-Dataset/raw/main/related_images/original.png)

## After augmetation
![augmetation_image](https://github.com/HSAkash/Banana-Leaf-Dataset/raw/main/related_images/augmented_image.png)

## CNN model
CNN model is used to train the network.<br>
Layer parameters:<br>
* Input size (224,224,3)
* Conv2D with 20 filters
* MaxPool2D (pool_size=2)
* Conv2D with 20 filters
* MaxPool2D (pool_size=2)
* Conv2D with 20 filters
* MaxPool2D (pool_size=2)
* Conv2D with 20 filters
* MaxPool2D (pool_size=2)
* GlobalAveragePooling2D
* Output

### Compile model
Compile the model with the following options:
* Loss function (categorical_crossentropy)
* optimizer (Adam lr=0.001)
* metrics (accuracy)

### Fit model
Then fit the model with the following parameters:
* train_data
* epochs (1100)
* validation_data (test data)
* validation_steps (len of test_data)


#### 0.Input image
![layer_0](https://github.com/HSAkash/Banana-Leaf-Dataset/raw/main/related_images/test_image.png)
#### 1.Conv2D with 20 filters (output)
![layer_0](https://github.com/HSAkash/Banana-Leaf-Dataset/raw/main/related_images/layer_0.png)
#### 2.MaxPool2D (pool_size=2) (output)
![layer_1](https://github.com/HSAkash/Banana-Leaf-Dataset/raw/main/related_images/layer_1.png)
#### 3.Conv2D with 20 filters (output)
![layer_2](https://github.com/HSAkash/Banana-Leaf-Dataset/raw/main/related_images/layer_2.png)
#### 4.MaxPool2D (pool_size=2) (output)
![layer_3](https://github.com/HSAkash/Banana-Leaf-Dataset/raw/main/related_images/layer_3.png)
#### 5.Conv2D with 20 filters (output)
![layer_4](https://github.com/HSAkash/Banana-Leaf-Dataset/raw/main/related_images/layer_4.png)
#### 6.MaxPool2D (pool_size=2) (output)
![layer_5](https://github.com/HSAkash/Banana-Leaf-Dataset/raw/main/related_images/layer_5.png)
#### 7.Conv2D with 20 filters (output)
![layer_6](https://github.com/HSAkash/Banana-Leaf-Dataset/raw/main/related_images/layer_6.png)
#### 8.MaxPool2D (pool_size=2) (output)
![layer_7](https://github.com/HSAkash/Banana-Leaf-Dataset/raw/main/related_images/layer_7.png)
#### 9.Prediction (final output)
![prediction](https://github.com/HSAkash/Banana-Leaf-Dataset/raw/main/related_images/predict.png)

## Confusion Matrix
![confusion_matrix](https://github.com/HSAkash/Banana-Leaf-Dataset/raw/main/related_images/confusion_matrix.png)




# Requirements
* matplotlib 3.5.2
* numpy 1.23.1
* Pillow 9.2.0
* scikit-learn 1.1.1
* scipy 1.8.1
* tensorflow 2.9.1


# Demo
Here is how to run the banana disease program using the following command line.<br>
```bash
python banana.py
```

# Directories
<pre>
│  banana.py
│
├─env
├─banana-leaf-dataset
|   ├─train
|   ├─test
|   ├─val
|
</pre>

# Reference
* [Tensorflow](https://www.tensorflow.org/)
* [data_augmentation](https://www.tensorflow.org/tutorials/images/data_augmentation)

# Links (dataset & code)
* [Kaggle-Banana Leaf Dataset](https://www.kaggle.com/datasets/kaiesalmahmud/banana-leaf-dataset)
* [Kaggle-Code](https://www.kaggle.com/code/hsakash/banana-leaf-dataset-98-75-acc)


# Author
HSAkash
* [Facebook](https://www.facebook.com/hemel.akash.7/)
* [Kaggle](https://www.kaggle.com/hsakash)


