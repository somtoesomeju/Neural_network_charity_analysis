# Neural_network_charity_analysis

## Purpose
In this project, I am using neural networks to create a binary classifier to classify if applicants would be successful if funded by Alphabet Soup (an investment firm). In this project I will take advantage of the machine learning dependencies, Tensorflow and StandardScaler. Using my model, I am aiming to predict a target accuracy of 75%. This means that in my model, it should be able to sucessfully find companies that would actually do well if funded by Alphabet Soup.

## Resources
- Software: Google collab
- Languages used: Python.

## Results
### Data Processing
In order to make the model more accurate, I dropped two unecessary columns "EIN" and "NAME". The "IS_SUCCESSFUL" column is our target column because it contains binary data (0's & 1's). The 'APPLICATION_TYPE','AFFILIATION	CLASSIFICATION','USE_CASE','ORGANIZATION	STATUS','INCOME_AMT','SPECIAL_CONSIDERATIONS' & 'ASK_AMT' are all important features in our analysis.

### Compiling, Training & Evaluating the Model
Using Tensorflow, I am creating a neural network model that should achieve a target accuracy of at least 75%. In the model, I am going to try multiple "re-evaluations" in order to improve the accuracy.

 - In my first attempt, I removed the 'USE_CASE' column from our dataset. this produced an anncuracy of 73.3% ![add image](https://github.com/somtoesomeju/Neural_network_charity_analysis/blob/main/Resources/use_case.png).

- In my second attempt, I replaced "sigmoid" with "tanh". This slightly increased the accuracy to 73.4% ![add image](https://github.com/somtoesomeju/Neural_network_charity_analysis/blob/main/Resources/Tanh.png).

- In my third attempt, I increased the number of hidden nodes to 20 for the first layer and 8 for the second layer. I got a slightly lower accuracy of 73.1% ![add image](https://github.com/somtoesomeju/Neural_network_charity_analysis/blob/main/Resources/additional_nodes.png).

- In the final attempt, I changed the activation on the first hidden node layer to "relu", the second to "sigmoid" the third and the output layers to "tanh". I also added a third hidden layer to the model. I attained an accuracy of 73.45% ![add image](https://github.com/somtoesomeju/Neural_network_charity_analysis/blob/main/Resources/fourth_test.png).

## Summary
In the end, I was unable to achieve a 75% accuracy in my machine learning model. Even though the values were close, it was not accurate enough to be used for our project. I did try to add some extra layers whoch slightly increased it. The solution might be to either add more layers, or remove less data from the dataset. That might give us a more accurate prediction.




