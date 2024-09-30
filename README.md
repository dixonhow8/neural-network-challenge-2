# neural-network-challenge-2
This is the Module 19 challenge assignment.

## Background
I was tasked with creating a neural network that HR can use to predict whether employees are likely to leave the company. Additionally, HR believes that some employees may be better suited to other departments, so you are also asked to predict the department that best fits each employee. These two columns should be predicted using a branched neural network.

## Files
Download the following file to help you get started: attrition.ipynb

## Steps to Begin
Before starting the Challenge, be sure to complete the following steps:

1. Create a new repository for this project called `neural-network-challenge-2`. Do not add this Challenge assignment to an existing repository.
2. Clone the new repository to your computer.
3. Inside your local Git repository, add the starter file `attrition.ipynb` from your file downloads.
4. Push these changes to GitHub.
5. Upload `attrition.ipynb` to Google Colab and work on your solution there.
6. Make sure to periodically download your file and push the changes to your repository.

## Instructions
Open the starter file in Google Colab and complete the following steps, which are divided into three parts:

### Part 1: Preprocessing
- Import the data and view the first five rows.
- Determine the number of unique values in each column.
- Create `y_df` with the attrition and department columns.
- Create a list of at least 10 column names to use as `X` data (excluding the attrition and department columns).
- Create `X_df` using your selected columns.
- Show the data types for `X_df`.
- Split the data into training and testing sets.
- Convert your `X` data to numeric data types as necessary.
- Create a `StandardScaler`, fit the scaler to the training data, and transform both the training and testing data.
- Create a `OneHotEncoder` for the department column, fit the encoder to the training data, and transform both the training and testing data.
- Create a `OneHotEncoder` for the attrition column, fit the encoder to the training data, and transform both the training and testing data.

### Part 2: Create, Compile, and Train the Model
- Find the number of columns in the `X` training data.
- Create the input layer (do NOT use a sequential model, as there will be two branched output layers).
- Create at least two shared layers.
- Create a branch to predict the department target column (with one hidden layer and one output layer).
- Create a branch to predict the attrition target column (with one hidden layer and one output layer).
- Create the model.
- Compile the model.
- Summarize the model.
- Train the model using the preprocessed data.
- Evaluate the model with the testing data.
- Print the accuracy for both department and attrition.

### Part 3: Summary with answered questions

1. **Is accuracy the best metric to use on this data? Why or why not?**
   - Accuracy may not be the best metric due to potential class imbalances. Other metrics like F1-score or precision/recall might provide better insights into model performance.

2. **What activation functions did you choose for your output layers, and why?**
   - For the department output layer, a softmax activation function was chosen to handle multi-class classification. For the attrition output layer, a sigmoid activation function was selected for binary classification.

3. **Can you name a few ways that this model could be improved?**
   - The model could be improved through feature engineering, hyperparameter tuning, regularization techniques to prevent overfitting, and exploring more advanced architectures or ensemble methods.

## Author
Howard P. Dixon
