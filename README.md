# simple-model-inversion
My attempt to recreate the attack described in "Model Inversion Attacks that Exploit Confidence Information and Basic Countermeasures" by Fredrikson et al. in 2015 using Tensorflow 2.9.1

This was my first time using virtual enviroments, tensorflow and any python ML related libraries. For this reason I experimented with different abstractions for training models in tensorflow.

Link to original paper: https://dl.acm.org/doi/10.1145/2810103.2813677

Inspired by: https://github.com/Djiffit/face-decoding-with-model-inversion

## Instructions for Use (using Pip and Virtual Enviroments)
1. *optional* Create a virtual enviroment to install all the required libraries for running the program
    * Create the enviroment: python -m venv env
    * Activate the enviroment: env\Scripts\activate
    * Deactivate the enviroment (afterwards): deactivate
2. Active the enviroment and pip install packages to fulfill **requirements.txt**
3. Unzip the training/testing data. Original images can be found here: https://www.kaggle.com/datasets/kasikrit/att-database-of-faces?select=s1
   * faces
      * faces/training *(9 photos per person in each directory)*
          * faces/training/s1
          * faces/training/s2
          * ...
          * faces/training/s40
      * faces/testing *(1 photo per person in each directory)*
          * faces/testing/s1
          * faces/testing/s2
          * ...
          * faces/testing/s40

5. Select your enviroment as the kernel for either Jupyter notebook and run each cell in order

The output of the inversion will show you step-by-step the inversion taking place.


### simplemodel.ipynb
Uses the highest-level of abstraction tensorflow offers to create the face-recognition model.

### complexmodel.ipynb
The model training process is a little less abstract and uses a defined training and testing function.
