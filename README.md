# Report of Charity Funding Predicing on the Neural Network Model

Background
The nonprofit Alphabet Soup Foundation wanted a tool that could help the organization select grant candidates with the best chance of success in their venture. Using your knowledge of machine learning and neural networks, you will use the functionality of the provided dataset to create a binary classifier that can predict whether a subscriber will pass if given Alphabet Soup sponsor or not.

# Data Preprocessing

The dataset has all irrelevant information removed; therefore, EIN and NAME were removed from the model. The remaining columns are considered model features. Although NAME was added in the second test. CLASSIFICATION and APPLICATION_TYPE changed to "Other due to high volatility". The data is divided into training and test data sets. The model's target variable is "IS_SUCCESSFUL" and is checked against the value, 1 is considered yes and 0 is no. APPLICATION data were analyzed and the value of CLASSIFICATION was used for grouping. Each unique value is used multiple data points as the cut-off point to group the "rare" categorical variables into a new, "Other" value. Then check if the grouping was successful. Categorical variables are encoded by 'pd.get_dummies().

# Compile, Train, and Evaluate the Model

The neural network is applied to each model in several layers, for a total of three layers. The number of features determines the number of hidden nodes. A three-class training model generated 477 parameters. The first attempt got close to 72%, well below the desired 75%.

# Optimize the Model

The second attempt added 'NAME' to the dataset, this time I got 79% which is 4% above target. A total of 3298 parameters.Deep learning models must have many layers, because they are machine-based, they teach the computer to filter input through layers to learn how to predict and classify information.
