
# Before Deep Learning, Let's Machine Learning!

**Important to note:**

For both machine learning and deep learning, they are HIGHLY data-dependent! If your dataset is biased, the model will be biased! Hence, before constructing a model, the dataset has to be evaluated carefully to avoid any potential ethical issues and unforeseen outcomes.

In this tutorial, I will be using ```Scikit-Learn``` and this book: Hands-On Machine Learning with Scikit-Learn & TensorFlow, to give an overview of how a machine learning model is built, specifically supervised learning. 

## Setting up the environment for your machine learning project

Before we start the actual tutorial, let's setup our coding environment. Yes, you need Python 3 in your workstation. A concise note on how to get started working with Python 3 from [Real Python](https://realpython.com/):

-   Python can be obtained from the Python Software Foundation website at python.org. Typically, that involves downloading the appropriate installer for your operating system and running it on your machine.
-   Some operating systems, notably Linux, provide a package manager that can be run to install Python.
-   On macOS, the best way to install Python 3 involves installing a package manager called Homebrew. You’ll see how to do this in the relevant section in the tutorial.
-   On mobile operating systems like Android and iOS, you can install apps that provide a Python programming environment. This can be a great way to practice your coding skills on the go.

Full tutorial on installing Python 3 can be found on [Real Python site](https://realpython.com/installing-python/).

Next, install ```pip```, a Python package manager:

### Install Pip on MacOS

Install ```pip``` on ```MacOS```, using ```easy_install``` command and upgrade pip to the latest version:

```
$ sudo easy_install pip
$ sudo pip install --upgrade pip
```

### Install Pip in Ubuntu

Install ```pip``` in ```Ubuntu```, using ```apt-get``` package manager:

```
$ sudo apt-get update
$ sudo apt-get install python-pip
$ sudo pip install --upgrade pip

```

### Install a virtual environment

Quoting from KDnuggets

> We use virtual environments in order to separate our coding set ups. 
> Imagine if at some point you wanted to do 2 different projects on your computer, which required different libraries of different versions. 
> Having them all in the same working environment can be messy and you’ll likely run into the problem of conflicting library versions. 
> Your ML code for project 1 needs version 1.0 of numpy, but project 2 needs version 1.15. Yikes!

A virtual environment allows us to isolate our working areas to avoid those conflicts.

```
sudo pip install virtualenv
```


### Create a virtual environment

To create a virtual environment, you must specify a path. For example to create one in the local directory called 'mypython', type the following:

```
virtualenv mypython
```

### Activate the virtual environment
You can activate the python environment by running:

1.   Mac OS / Linux

```
source mypython/bin/activate
```
OR

```
source activate mypython
```
2.   Windows

```
mypthon\Scripts\activate
```

You should see the name of your virtual environment in brackets on your terminal line e.g. (mypython). Any python commands you use will now work with your virtual environment.



### Installing the essential packages

After activating your virtual environment, you can start to install the essential packages for machine learning:

1.   numpy
2.   scipy
3.   pandas
4.   sklearn
5.   jupyter
6.   matplotlib

```
pip install --upgrade numpy scipy pandas scikit-learn jupyter matplotlib    
```

### To check the installatio of the packages

```
python -c "import jupyter, matplotlib, numpy, pandas, scipy, sklearn"
```

There should be no output and no error. 

### Deactivate the virtual environment

To decativate the virtual environment and use your original Python environment, simply type ```deactivate```.

```
deactivate 
```


### Getting started

Let's start by activating your virtual environment
1.  ```source activate mypython```
2.  ```jupyter notebook```
3.  Now create a new Python notebook by clicking on the New button and selecting the Python 3

YES! You're now ready to rock!

Quoting from the book: Hands-On Machine Learning with Scikit-Learn & TensorFlow,

> A notebook contains a list of cells. Each cell can contain executable code or formatted text. 

Right now the notebook contains only one empty code cell, labeled “In [1]:”. Try typing print("Hello world!") in the cell, and click on the play button (see Figure 2-4) or press Shift-Enter. 


### Brief Overview

There are four major components in most machine learning and deep learning system:

1.  Data Construction
2.  Feature Extraction
3.  Model Construction
4.  Model Evaluation

### Data Construction

Data collection is a crucial step in building a robust model.

> Garbage in, garbage out.

As the quote suggested, poor quality of training data will lead to an inaccurate output. In other words, the performance of the model is heavily reliant on the quality of the training data. Hence, the quality and correctness of the data have to be validated before training. In general, data collection is the process of gathering and labeling a collection of ground truth data. It usually involves data acquisition and data labeling, or simply using an existing dataset. For the purpose of this tutorial, I'll be using the [breast cancer Wisconsin dataset](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_breast_cancer.html) and at the same time showing you how to visualize and evaluate the data.


```python



```
