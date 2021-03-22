# dog-vs-wolf-image-classification
It classifies if a given picture is of a dog or a wolf- this was a complicated task as dogs and wolves look alike, so this was a great challenge!

<h2>Dataset:</h2>

I have used this <a href="http://vision.stanford.edu/aditya86/ImageNetDogs/">dataset</a> from Kaggle

<p> Go to this <a href="https://medium.com/analytics-vidhya/how-to-fetch-kaggle-datasets-into-google-colab-ea682569851a">link</a> to know how to load the dataset to google colab</p>


<br>
<br>
<h2>Model Summary</h2>
<br><p>Model: "sequential_2"
  <br>
_________________________________________________________________<br>
Layer (type)                 Output Shape              Param #   <br>
=================================================================<br>
sequential (Sequential)      (None, 300, 300, 3)       0         <br>
_________________________________________________________________<br>
rescaling (Rescaling)        (None, 300, 300, 3)       0         <br>
_________________________________________________________________<br>
conv2d_3 (Conv2D)            (None, 300, 300, 16)      448       <br>
_________________________________________________________________<br>
max_pooling2d_3 (MaxPooling2 (None, 150, 150, 16)      0         <br>
_________________________________________________________________<br>
conv2d_4 (Conv2D)            (None, 150, 150, 32)      4640      <br>
_________________________________________________________________<br>
max_pooling2d_4 (MaxPooling2 (None, 75, 75, 32)        0         <br>
_________________________________________________________________<br>
conv2d_5 (Conv2D)            (None, 75, 75, 64)        18496     <br>
_________________________________________________________________<br>
max_pooling2d_5 (MaxPooling2 (None, 37, 37, 64)        0         <br>
_________________________________________________________________<br>
dropout_1 (Dropout)          (None, 37, 37, 64)        0         <br>
_________________________________________________________________<br>
flatten_1 (Flatten)          (None, 87616)             0         <br>
_________________________________________________________________<br>
dense_2 (Dense)              (None, 128)               11214976  <br>
_________________________________________________________________<br>
dense_3 (Dense)              (None, 2)                 258       <br>
=================================================================<br>
Total params: 11,238,818<br>
Trainable params: 11,238,818<br>
Non-trainable params: 0<br>
_________________________________________________________________</p>
