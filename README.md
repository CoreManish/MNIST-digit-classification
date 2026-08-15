## MNIST-digit-classification
MNIST dataset is collection of gray 28x28 images.

## what has been done
digit has been firstly classified by ML classification model, then same digits dataset were classified by CNN

## Machine learning algorithm on MNIST dataset
As it is gray scale image means single channel, so each image is 28x28 grid with no depth. So it's value can be flatten to make 28x28=784 array of numbers to train any machine learning classification algorithm. These 784 numbers can be input and at output we will be having 0,1,2,3,4,5,6,7,8,9 as classes.

## CNN on MNIST dataset
Because given image is gray scale (1 color channel), so First Layer Filter Shape: (1, 3, 3) ie [1 channel, 3x3 height/width].
In an RGB image, a single $3 \times 3$ filter must look at 3 channels simultaneously, so it has $3 \times 3 \times 3 = 27$ learnable weights. In a Grayscale image, a single $3 \times 3$ filter only looks at 1 channel, so it has $1 \times 3 \times 3 = 9$ learnable weights.

## MNIST dataset trained by fully connected neural network using tensorflow library
* Here no ML classification algorithm is used.
* Installation steps
    * `python3.12 -m venv myenv312` to create virtual environment. currently tensorflow support up to python 3.12
    * `source ./myenv312/bin/activate` to activate virtual environment.
    * `pip install tensorflow[and-cuda]` install tensorflow with GPU support. takes more than 3GB data
