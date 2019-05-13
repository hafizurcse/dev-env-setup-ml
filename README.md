
# How to set up your Dev Environment for Machine Learning/DNN/CNN etc?

## Windows Machine

1. Download and install Anaconda3 for your Windows from:
https://repo.anaconda.com/archive/Anaconda3-2019.03-Windows-x86_64.exe
2. Once Installation of Anaconda done, go to your start button and search for "Anaconda Command Prompt". Then open it.

3. Install your packages you need
```
conda install keras

conda install h5py 

conda install pandas

conda install jupyter

pip install sklearn
```
The above packages will be installed in your conda root.

5. Test Package Versions

Check your `Keras`, `TensorFlow`, `Pandas`, `h5py`, `sklearn` versions in your terminal. I have shown how to see Python version and versions of other packages in `Linux` environment. 
```
hafizur@hafizur-MacBookPro:~/dev/hafiz_dev/machine_learning/$ python
Python 3.6.1 |Anaconda custom (64-bit)| (default, May 11 2017, 13:09:58)
[GCC 4.4.7 20120313 (Red Hat 4.4.7-1)] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> import keras as kr
Using TensorFlow backend.
>>> kr.__version__
'2.1.6'
>>> import tensorflow as tf
>>> tf.__version__
'1.8.0'
>>> import pandas as pd
>>> pd.__version__
'0.21.0'
>>> exit() # to exit from command prompt
```
6. Once the above tests (step 4) pass, create a project folder (let's say `my_ml_project` ) and change directory (`cd`) to your project folder. Then write the following command in your Anaconda Command Prompt:
```
jupyter notebook
```
It will create a web server which will be listening at port 8888 in the URL: http://localhost:8888/tree

Jupyter Notebooks are a powerful way to write and iterate on your Python code for data analysis & machine learning. Rather than writing and re-writing an entire program, you can write lines of code and run them one at a time. 

To find out how to use, please visit: https://www.codecademy.com/articles/how-to-use-jupyter-notebooks

Now you can start building your Machine Learning, DNN, CNN algorithms. Congratulations!!!


The following is optional specially for one who needs a virtual environment hence can be entirely discarded if you are happy with above setting.

## Virtual Environment

But if you prefer to create a environment variable which offers flexibility in having different version of Pythons, different packages according to your project necessity.

Follow the steps in your Anaconda Command Prompt:
```
conda create --name ml_env python=3.7

activate ml_env

conda install keras

conda install h5py 

conda install pandas

pip install sklearn
```
A virtual environment called `ml_env` is created.
