# simple-model-inversion
My attempt to recreate the attack described in "Model Inversion Attacks that Exploit Confidence Information and Basic Countermeasures" by Fredrikson et al. in 2015 using Tensorflow 2.9.1

## Instructions for Use (using Pip and virtual Enviroments)
1. *optional* Create a virtual enviroment to install all the required libraries for running the program
    * Create the enviroment: python -m venv env
    * Activate the enviroment: env\Scripts\activate
    * Deactivate the enviroment (afterwards): deactivate
2. Active the enviroment and pip install packages to fulfill **requirements.txt**
3. Download the training data https://www.kaggle.com/datasets/kasikrit/att-database-of-faces?select=s1
5. Select your enviroment as the kernel for either Jupyter notebook and run each cell in order

The output of the inversion will show you step-by-step the inversion taking place.


### simplemodel.ipynb
Uses the highest-level of abstraction tensorflow offers to create the face-recognition model.

### complexmodel.ipynb
The model training process is a little less abstract and uses a defined training and testing function.
