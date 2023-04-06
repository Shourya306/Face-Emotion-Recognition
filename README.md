<p align="center"> 
  <img src="https://github.com/venugopalkadamba/Face_Emotion_Recognition/blob/master/All_Emotions_Detection.jpg" alt="Face Emotion Image" width="400px" height="200px">

<h1 align="center"> FACE EMOTION RECOGNITION </h1>

## Project Introduction:<br>
<p>The Indian education landscape has been undergoing rapid changes for the past ten years owing to the advancement of web-based learning services, specifically eLearning platforms.</p>

<p>Digital platforms might overpower physical classrooms in terms of content quality, but in a physical classroom, a teacher can see the faces and assess the emotion of the class and tune their lecture accordingly, whether he is going fast or slow. He can identify students who need special attention.
While digital platforms have limitations in terms of physical surveillance, it comes with the power of data and machines, which can work for you.</p>

<p>It provides data in form of video, audio, and texts, which can be analyzed using deep learning algorithms. A deep learning-backed system not only solves the surveillance issue, but also removes the human bias from the system, and all information is no longer in the teacher’s brain but rather translated into numbers that can be analyzed and tracked.</p>

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

## Objective:<br>
Our objective is to solve the above mentioned challenge by applying deep learning algorithms to live video data inorder to recognize the facial emotions and categorize them accordingly.

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

## Dataset
<b>Dataset Link:</b> https://www.kaggle.com/deadskull7/fer2013 <br>
The dataset contains 35887 images of people showing 7 unique emotions: Anger, Happy, Disgust, Sad, Surprise, Neutral and Fear. <br>

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

## Steps for running in local computer
**STEP-1:** Install all the dependencies mentioned in **requirements.txt** file. You can run the following command in your command prompt to install all the dependencies:

```python
pip install -r requirements.txt
```
**STEP-2:** After installing all the dependencies, open command prompt from the direction where main.py file is present and run the following command:

```python
python main.py
```
That's it, you can see the web application running at you localhost.<br>

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
  
## Project Overview:<br>
<p>We start with downloading the required dataset from Kaggle. Once the data is available, the training and validation sets are defined.</p>

<p>The next step is to preprocess the datasets; this includes performing one hot encoding to convert the dimensions of y_train and y_test to num_classes * m(examples) and also reshaping the X_train and X_test to m(examples) * 48 * 48 * 1.</p>

<p>After preparing the data, we construct the required CNN model using TensorFlow and Keras libraries to recognize the facial emotions of a user. This model consists of four convolutional layers and three fully connected layers to process the input image data and predict the required output. In between each layer, a Max Pooling and Dropout layer and Batch Normalization was added for downsampling the data and preventing our model from overfitting. Finally, for compiling all the layers, we have used the Adam optimizer, with loss function as Categorical Cross entropy and accuracy as the metric for evaluation.</p>

<p>Once the model was ready, we trained it using the prepared data.</p>

<p>The model achieved an accuracy of around 73% on the training set and 58-63% on the validation set after fifteen epochs.</p>  
 
 

