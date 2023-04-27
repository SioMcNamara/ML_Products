# Repo Name: ml_product_template

## 🧐 About <a name = "about"></a>
Write about 1-2 paragraphs describing the purpose of this code base.

## 🔖 Repo structure

```
Project_folder/
|- bin/          # contains scripts and main files that should be run
|- config/       # config files
|- notebooks/    # notebooks for EDA and exploration
|- src/          # source code - contains functions
|- tests/        # Test files should mirror the src folder
|- Makefile      # automatize taks through make utility
```

## Things to Review
Makefile: https://medium.com/@sabman/dear-data-scientist-add-a-makefile-to-your-projects-top-level-directory-55715b8dfe79

https://towardsdatascience.com/using-make-for-data-science-projects-changed-my-life-23de1597e2e

Pytest: https://towardsdatascience.com/pytest-for-data-scientists-2990319e55e6

Pylint: https://www.youtube.com/watch?v=fFY5103p5-c

Black: https://www.youtube.com/watch?v=A6S2nZAXgT8

## 🏁 Getting Started <a name = "getting_started"></a>
Clone this repo and make all the necessary changes to generate your own.

These instructions will get the project up and running on your local machine for development and testing purposes.

### Prerequisites
Setup your environement and install project dependencies
```
conda create -n my_project python=3.10
source activate my_project

python -m pip install pip-tools
pip-compile --output-file requirements.txt requirements.in requirements_dev.in
python -m pip install -r requirements.txt
```

### Installing

## 🔧 Running the tests
Tests are implemented in ./tests, you need to run the following command to run them.
```
make tests
```

## 🚀 Deployment
Need to add more here & dockerize this too

## 🎈 Pushing changes
To contribute in this project, please setup locally the project following the steps  in Getting started section.
We use few packages to guarantee high quality code. Before commiting you can run:
To format you code using black
```
make black
```
To get warning message on non respect of pep8 code guidance:
(the command runs on all .py files in the project)
```
make lint
```
You can also run automatically, black, lint and few other packages to analyze and check your code base before commiting
```
make precommit
```

##  ✍️ Authors
