Dataset - Sketch
<br>
Sketch Classification<br>
Initial Dataset had around 125 classes.<br>
aeroplane, bird, box etc.... <br>
500 images per class.<br>
Problem Statement we picked 10 
classes out of those 125.
because our aim was to study the effects of various machine learning techinques like 
cross validation, data preprocessing(feature extraction) and Dimensionality reduction.<br>
[0,0,0,0,1,0,0,0,0] - Y (10)<br> 
One Hot encoding<br>
X - (224, 224)<br>
Algorithm - Random Forest, Naive Bayes,SVM<br>
2D data -> 1D data (There might be chances of data loss while converting data from 2D to 1D)<br>
Flatten<br>
We used all three algorithms. our accuracy was around 8-10%<br>
Feature extraction -<br>
2D image -> pretrained model -> 1D array (features preserve)<br>
VGG16 Model -> feature extractor model trained by google.(224, 224, 3) -> 4096<br>
4096 let's train our models on this <br>
it took almost infinite time!!!!!!<br>
Due to 4096 feature our model is taking too much time and wasn't even performing good.<br>
Dimensionality Reduction -<br>
Too many features -> merge some of them -> less features<br>
Principal Component Analysis - PCA<br>
4096 features -> PCA -> 100 features<br>
X - 5762, 100<br>
Y - 5762, 10Standarizing Dataset almost no effect on 
accuracy!!<br>
10 1000000 -10 ->>>>> 10 500 -10<br>
Read dataset - feature extraction - dimensionality reduction - standarization - train model<br>

We trained models on this preprocessed data
- Splitted the dataset into train and test
1. Random Forest Classifier - 54%
2. Naive Bayes with cross validation - 79%
3. SVM model - 85%
10 classes - 85% accuracy is very nice :)<br>

We have taken 25 classes i!!!
Read dataset - feature extraction - train model 
We used a neural network - 97% accuracy!!
