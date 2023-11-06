# Overview of the analysis:
The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.
The objective is to optimize the model in order to attain an accuracy score surpassing 75%.


# Results:
- ## Data Preprocessing
    - I read in the charity_data.csv to a Pandas DataFrame
        The target variables for the models were  “IS_SUCCESSFUL”, 1 for a yes and 0 for a no
    - I droped "EIN" and "NAME" for the first analysis, but added back "NAME" for the second analyses for binning purposes. The feature variables were every columns except the target variables and
        the droped variable(s)
    -  "APPLICATION" data was analyzed and "CLASSIFICATION" value was used for binning   
    


- ## Compiling, Training, and Evaluating the Model
    - I decided to include 3 layers: an input layer with 80 neurons, a second layer with 30 neurons, and an output layer with 1 neuron
    https://github.com/sanjchip/deep-learning-challenge/blob/main/Resources/define%20the%20model.png?raw=true

    - I selected the relu activation function for the first and second layers, and the sigmoid activation function for the output layer since the goal was binary classification

    - The first attempt was only 73% accuracy 
    https://github.com/sanjchip/deep-learning-challenge/blob/main/Resources/first%20attempt.png?raw=true

    - ## Optimization:
    After adding back "NAME" we increased our accuracy to 78%
    https://github.com/sanjchip/deep-learning-challenge/blob/main/Resources/second%20attempt.png?raw=true