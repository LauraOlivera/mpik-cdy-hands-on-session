# mpik-cdy-hands-on-session
Hands on session for the CDY summer school - Saturday 29th June 2024
Organized by Quentin Remy, Georg Schwefer, Davide Depaoli and Laura Olivera-Nieto

# Step 0 - Setup
## Installation
We will use two packages to analyze and model gamma-ray data, respectively: GAMERA and Gammapy.

To get started, first you need to install the software.
We will use the latest stable Gammapy release, 1.2. Please follow the installation instructions detailed here https://docs.gammapy.org/1.2/getting-started/index.html#quickstart-setup, including the download of the public datasets.
Please make sure to define the `GAMMAPY_DATA` environment variable (`export GAMMAPY_DATA=your/path/to/it/gammapy-datasets/1.2`)

To install GAMERA, please follow the instructions in http://libgamera.github.io/GAMERA/docs/download_installation.html. We will use only the python bindings ("gappa").

To test your setup you can just run the following code

```
import sys
sys.path.append('path/to/installation/GAMERA/lib')
import gappa as gp
from gammapy.utils.check import check_tutorials_setup

check_tutorials_setup()
```
If it works, you should be good to go!

## GitHub
Through the tutorial today we will be using github to distribute code. The idea is that you will first get a notebook with some exercises and tips, we will give you some time to work on it, and after a while, we will provide a notebook with the solution. All of this code sharing will be done using git.

The first step is to clone this repository as 
```
git clone https://github.com/LauraOlivera/mpik-cdy-hands-on-session.git
```
Now you have a local copy of the repository. In order to get new changes you just need to do
```
git pull
```
For each exercise we will provide two notebooks: one called `exercise_X.ipynb` and one `exercise_X_solution.ipynb`. Please do not modify the "solution" files so as to not run into merge conflicts.

# Workflow
We will start doing the notebooks in the Gammapy folder, labelled 1 to 5. We will walk you through 1-3 so that you can get familiar with the framework. Notebooks 4 and 5 are an exercise.

After that we will move to the Gamera section. We will walk you through exercise 1 and leave 2-4 to you.

Finally we will combine both sections and tackle the Gammapy notebooks 6 and 7, where Gamera is used to fit a model to the joint Crab datasets.



