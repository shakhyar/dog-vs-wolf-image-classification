# dog-vs-wolf-image-classification
It classifies if a given picture is of a dog or a wolf- this was a complicated task as dogs and wolves look alike, so this was a great challenge!

<h2>Dataset:</h2>

I have used this <a href="http://vision.stanford.edu/aditya86/ImageNetDogs/">dataset</a> from Kaggle

<p> Go to this <a href="https://medium.com/analytics-vidhya/how-to-fetch-kaggle-datasets-into-google-colab-ea682569851a">link</a> to know how to load the dataset to google colab</p>


<br>
<br>
<h2>Model Summary</h2>
<p>Model: "sequential_2"
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
sequential (Sequential)      (None, 300, 300, 3)       0         
_________________________________________________________________
rescaling (Rescaling)        (None, 300, 300, 3)       0         
_________________________________________________________________
conv2d_3 (Conv2D)            (None, 300, 300, 16)      448       
_________________________________________________________________
max_pooling2d_3 (MaxPooling2 (None, 150, 150, 16)      0         
_________________________________________________________________
conv2d_4 (Conv2D)            (None, 150, 150, 32)      4640      
_________________________________________________________________
max_pooling2d_4 (MaxPooling2 (None, 75, 75, 32)        0         
_________________________________________________________________
conv2d_5 (Conv2D)            (None, 75, 75, 64)        18496     
_________________________________________________________________
max_pooling2d_5 (MaxPooling2 (None, 37, 37, 64)        0         
_________________________________________________________________
dropout_1 (Dropout)          (None, 37, 37, 64)        0         
_________________________________________________________________
flatten_1 (Flatten)          (None, 87616)             0         
_________________________________________________________________
dense_2 (Dense)              (None, 128)               11214976  
_________________________________________________________________
dense_3 (Dense)              (None, 2)                 258       
=================================================================
Total params: 11,238,818
Trainable params: 11,238,818
Non-trainable params: 0
_________________________________________________________________</p>
