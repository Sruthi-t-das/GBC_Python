# **EDA - Step by Step**

In this repo we will do a deep dive into EDA and cover each step of EDA seperately.

## Requirements

- pyenv
- python==3.11.3

## Setup
One of the first steps when starting any data science project is to create a virtual environment. For this project you have to<br> create this environment from scratch yourself. However, you should be already familiar with the commands you will need to do so.<br> The general workflow consists of...

- setting the python version locally to ```3.11.3```
- creating a virtual environment using the ```venv``` module
- activating your newly created environment
- upgrading ```pip``` (This step is not absolutely necessary, but will save you trouble when installing some packages).
- installing the required packages via ```pip```

All together, it looks like:

```
pyenv local 3.11.3
python -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```

At the end, you want to make sure that people who are interested in your project can create an identical environment on their own<br> computer in order to be able to run your code without running into errors. Therefore you can create a ```requirements file``` and add<br> it to your repository. You can create such a file by running the following command:

```
pip freeze > requirements.txt
```

_**Note:** In rare case such a requirements file created with pip freeze might not ensure that another (especially M1 chip) user <br>can install and execute it properly. This can happen if libraries need to be compiled (e.g. SciPy). Then it also depends on environment<br> variables and the actual system libraries._

## Work on the files in the following order:

1. [EDA introduction](./01_EDA.ipynb)
2. [EDA excercise 1](./02_EDA_excercise_1.ipynb) 
3. [EDA excercise 2](./03_EDA_excercise_2.ipynb) 
4. [EDA excercise 3](./04_EDA_excercise_3.ipynb) 
5. [Handling outliers](./05_handling_outliers.ipynb)
6. [Statistical tests](./06_Statistical_hypothesis_testing.ipynb)

## Unit testing (Optional)
If you write python scripts for your data processing methods, you can also write unit tests. In order to run the tests execute in<br> terminal:
```
pytest
```
This command will execute all the functions in your project that start with the word **test**.