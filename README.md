# traffic-ai
I wrote an AI to identify which traffic sign appears in a photograph. Using **TensorFlow**, I built a **neural network** to **classify road signs based on an image of those signs**. 

Starter code was provided for this project, which I completed in the context of Harvard UniversityX's [CS50 Introduction to Artificial Intelligence with Python](https://cs50.harvard.edu/ai/2020/) course.

## Specification
This program uses a **labeled dataset**: a collection of images that have already been categorized by the road sign represented in them. More specifically, the [German Traffic Sign Recognition Benchmark](http://benchmark.ini.rub.de/?section=gtsrb&subsection=news) (GTSRB) dataset, which contains thousands of images of 43 different kinds of road signs.

In the *main* function, we accept as command-line arguments a directory containing the data and (optionally) a filename to which to save the trained model. The data and corresponding labels are then loaded from the data directory (via the *load_data* function) and split into training and testing sets. After that, the *get_model* function is called to obtain a compiled neural network that is then fitted on the training data. The model is then evaluated on the testing data. Finally, if a model filename was provided, the trained model is saved to disk.

Visit the [Harvard CS50AI]([https://cs50.harvard.edu/ai/2020/projects/0/tictactoe/](https://cs50.harvard.edu/ai/2020/projects/5/traffic/)) for more information about the specifications for the project. Please **do not** directly use the source code as it is **only** for reference. Plagiarism is strictly prohibited by both Harvard University and the edX platform. See [academic honesty](https://cs50.harvard.edu/ai/2020/honesty/) for details.

## Implementation

I implemented the:
- *load_data*, and 
- *get_model* 
functions.

--> Click here to view a short [video demo](https://youtu.be/Q3UIadopdmY) of my implementation. 

### Building the model
In order to lower the loss and increase the accuracy of my model, I tweaked and fine-tuned the hyperparameters: I iteratively changed the number of layers, the number of neurons per layer etc.

## Getting started
Inside of the traffic directory, run **pip3 install -r requirements.txt** to install this project’s dependencies: *opencv-python* for image processing, *scikit-learn* for ML-related functions, and *tensorflow* for neural networks. Download the [data set](https://cdn.cs50.net/ai/2020/x/projects/5/gtsrb.zip) for this project and unzip it. Move the resulting gtsrb directory inside of your traffic directory.
