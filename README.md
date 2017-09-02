# Semantic Segmentation
### Introduction
This project seeks to identify sections of roadway within an image using a fully connected NN (FCN). The FCN that is used is based on (this paper)[https://people.eecs.berkeley.edu/~jonlong/long_shelhamer_fcn.pdf].

The FCN uses the VGG16 recognition model as a seed and extracts layers 3,4 & 7 to feed back into the encoder process. This process described in the paper above works well to segment images based on the feature sets from the training data. 

#### Results
![Training Image](../master/results/um_000000_train.png)

![Classified Image](../master/results/um_000000_results.png)



### Setup
##### Frameworks and Packages
Make sure you have the following is installed:
 - [Python 3](https://www.python.org/)
 - [TensorFlow](https://www.tensorflow.org/)
 - [NumPy](http://www.numpy.org/)
 - [SciPy](https://www.scipy.org/)
##### Dataset
Download the [Kitti Road dataset](http://www.cvlibs.net/datasets/kitti/eval_road.php) from [here](http://www.cvlibs.net/download.php?file=data_road.zip).  Extract the dataset in the `data` folder.  This will create the folder `data_road` with all the training a test images.

### Start
##### Implement
Implement the code in the `main.py` module indicated by the "TODO" comments.
The comments indicated with "OPTIONAL" tag are not required to complete.
##### Run
Run the following command to run the project:
```
python main.py
```
