# First EDA Project Template
Template for creating ds simple projects. 

- From README.md file, navigate to other ```.md``` files in the order: [assignment.md](./assignment.md), [workflow.md](./workflow.md) and then [column_names.md](./column_names.md).

## Requirements
- set up pyenv
- python==3.11.3

## Setup

One of the first steps when starting any data science project is to create a virtual environment. For this project you<br> have to create this environment from scratch yourself. However, you should be already familiar with the commands you will<br> need to do so. The general workflow consists of...

- setting the python version locally to 3.11.3
- creating a virtual environment using the ```venv``` module
- activating your newly created environment
- upgrading ```pip``` (This step is not absolutely necessary, but will save you trouble when installing some packages.)
- installing the required packages via ```pip```

At the end, you want to make sure that people who are interested in your project can create an identical environment on<br> their own computer in order to be able to run your code without running into errors. Therefore you can create a requirements<br> file and add it to your repository. You can create such a file by running the following command:

```
pip freeze > requirements.txt
```

_Note: In rare case such a requirements file created with pip freeze might not ensure that another (especially M1 chip) user can install and execute it properly. This can happen if libraries need to be compiled (e.g. SciPy). Then it also depends on environment variables and the actual system libraries._

## Unit testing (Optional)
If you write python scripts for your data processing methods, you can also write unit tests. In order to run the tests <br>execute in terminal:

```
pytest
```
This command will execute all the functions in your project that start with the word test.

```
Feel free to update and make this README file according to your needs!!!
```

