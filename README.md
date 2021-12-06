# Understanding the Amazon from space

Tracking human activities with satellite imagery and classifying them using a CNN
The dataset were obtained from a project on Kaggle, which aims to help the global community to help understand where and how we can respond to deforestation 
and is available at [Planet: Understanding the Amazon from Space](https://www.kaggle.com/c/planet-understanding-the-amazon-from-space)


----------------------------

### Tools
The [Pytorch Framework](https://pytorch.org/) was used to create the training architecture. 
Tools such as [Pandas](https://pandas.pydata.org/), [Numpy](https://numpy.org/) and [Matplotlib](https://matplotlib.org/), among other tools, were also used.

### Structure

The process was divided into training using 80% of the total data and validation with the remaining 20% and testing at the end with 10 samples. 
64x64 size images were used, with batch size of 30 samples.

#### CNN's structure:
- Three sets of image processing and analysis layers: Convolutional layer -> ReLU activation function -> Pooling layer
- One flatten layer
- Two Layers of ReLU Activation Function
- One classification layer using a hybrid method of the Sigmoid function with Binary Cross-entropy
- Stochastic gradient descent for optimization method with 0.001 learning rate and 0.9 as momentum
- One Hot Encode for the encoding and decoding of the labels


