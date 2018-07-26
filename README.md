

# MNIST2PNG
This is a python scripts convert MNist sklearn datasets into png file for better visualization of the datasets to be used for convolutional Neural Network.


### Intuition
The below code is used to load the Mnist dataset which contains already extracted features of 28x28 pixels of images.

```python	
from sklearn import datasets
dataset = datasets.fetch_mldata("MNIST Original")
```	

But what if we dont need the already extracted features, what if we need the raw image so that we can also pass it through different convolutional layers and get more features about it.

That is why there is need for the dataset to be converted back to raw images so  that we can perfome our operations on it.

### Organization of the project

The project contains the root python script, an input directory and output folder.

 1. The  scripts contains the conversion code, we just a one line cli to run it.
 2. The **input** directory contains all the dataset we are able to lay our hands on, Downloaded from Yann LeCun Website [http://yann.lecun.com/exdb/mnist/](http://yann.lecun.com/exdb/mnist/). 
 you can also download the dataset from any other websites that offers this.
 
 3. You will need an **output** directory where to store the converted images, and inside the out put folder, you need to create the **training** and **testing** folder to automatically split the converted images into training and testing.

 
### Running the scripts
To run this scripts, you will need to follow the command below **<input_folder>** and  **<output_folder>** are the folder we created earlier.

`python convert_mnist_to_png.py <input_folder> <output_folder>`
 
This will iterate over the dataset extracted from Yann LeCun websites and converts them.

The converted files can be found in your ouput file supplied.

Below are sample images after conversion

<img src="https://raw.githubusercontent.com/princesegzy01/MNIST2PNG/master/output/training/4/1004.png" alt="drawing" width="200px"/>
<img src="https://raw.githubusercontent.com/princesegzy01/MNIST2PNG/master/output/training/0/1000.png" alt="drawing" width="200px"/>
<img src="https://raw.githubusercontent.com/princesegzy01/MNIST2PNG/master/output/training/9/10028.png" alt="drawing" width="200px"/>

Thanks.


contact me  @ pricesegzy01@gmail.com for more information
