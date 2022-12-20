# Traffic Classification

## Data Set
The Data set I used in this model is provided By VALENTYN SICHKAR in Kaggle as shown in Kaggle data{0->8}.pickle,I used data8.pickle the main diferences between each file is:
- data0.pickle - Shuffling

- data1.pickle - Shuffling, /255.0 Normalization

- data2.pickle - Shuffling, /255.0 + Mean Normalization

- data3.pickle - Shuffling, /255.0 + Mean + STD Normalization

- data4.pickle - Grayscale, Shuffling

- data5.pickle - Grayscale, Shuffling, Local Histogram Equalization

- data6.pickle - Grayscale, Shuffling, Local Histogram Equalization, /255.0 Normalization

- data7.pickle - Grayscale, Shuffling, Local Histogram Equalization, /255.0 + Mean Normalization

- data8.pickle - Grayscale, Shuffling, Local Histogram Equalization, /255.0 + Mean + STD Normalization

Initially data is taken from German Traffic Sign Recognition Benchmarks (GTSRB)
## Model
The model used is 3 CNN layers with 2 MaxPooling layers with 2 DropOut layres and 3 Dense layers

conv2d_132 (Conv2D)                
_________________________________________________________________
max_pooling2d_82 (MaxPooling)        
_________________________________________________________________
dropout_7 (Dropout)                  
_________________________________________________________________
conv2d_133 (Conv2D)              
_________________________________________________________________
max_pooling2d_83 (MaxPooling)         
_________________________________________________________________
conv2d_134 (Conv2D)             
_________________________________________________________________
flatten_37 (Flatten)                 
_________________________________________________________________
dropout_8 (Dropout)                
_________________________________________________________________
dense_54 (Dense)                 
_________________________________________________________________
dense_55 (Dense)                
_________________________________________________________________
dense_56 (Dense)             

The accuracy on train set:0.9735
The accuracy on validation set:0.9807
The accuracy on test set:0.9663
