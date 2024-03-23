# neural-network-challenge-1
Module 18 - Student Loan Refinancing
Assignment for AI/ML Bootcamp Module 18 Challenge
Description
Our assignment was to simulate working at a company that specializes in student loan refinancing. If the company can predict whether a borrower will repay their loan, it can provide a more accurate interest rate for the borrower. My team has asked me to create a model to predict student loan repayment.

The business team has given me a CSV file that contains information about previous student loan recipients. With my knowledge of machine learning and neural networks, I decide to use the features in the provided dataset to create a model using Google Colab that will predict the likelihood that an applicant will repay their student loans. The CSV file contains information about these students, such as their credit ranking.

This challenge consists of the following subsections:

Part 1: Prepare the data for use on a neural network model
Part 2: Compile and evaluate a model using a neural network
Part 3: Predict loan repayment success by using my neural network model
Part 4: Discuss creating a recommendation system for student loans
Getting Started
Dependencies
Google User Account
Google Colaboratory: Google Colaboratory, or Colab, is a cloud-based notebook space, which allows you to run code in the cloud, rather than locally on your computer. These cloud-based notebooks make it easy to install the tools we need and give us the power of cloud computing.
Installing
Clone this repo to your environment
Setup Google Colaboratory
Navigate to Google Colaboratory
You will need a Google account to use Colab. Sign up for an account if you don't already have one. Reference How to setup a Google account for instructions.
Within your Google account, navigate to Google Drive and select "Go to Google Drive".
After navigating to Google Drive, click the New button and select Folder to create a new folder called "dev".
Navigate to the new folder. Once in the folder, you’ll need to connect (download) the Google Colab application:
Click New.
Scroll down to More and expand the dropdown menu.
At the bottom of the menu, click "Connect more apps."
Type “colab” in the top-right search field, and then press Enter to search for the Colaboratory application.
Click the Connect button to download the Colaboratory application.
How to Create a Colab Notebook
Create a Colab notebook by clicking New, hovering over More, and then selecting Colaboratory.
A new tab will launch with a new notebook. Everything is hosted online, but the functionality is very similar to Jupyter Notebook.
Upload notebook file, 'student_loans_with_deep_learning.ipynb', from your repo to Colab as follows:
From the Colab notebook you just opened, click File and then "Upload notebook."
Drag the notebook file into the box to upload. NOTE: When you upload notebooks, Google Drive will save them by default to a folder called Colab Notebooks. These files can easily be moved to the dev folder created earlier.
Executing program
Open 'student_loans_with_deep_learning.ipynb' in Colab
Step through the notebook to see my data preparation and analysis by clicking the "Run" button.
The results are displayed after each step.
Part 1: Prepare the data for use on a neural network model
Using Pandas and scikit-learn’s StandardScaler(), preprocess the dataset so that it can be used to compile and evaluate the neural network model.

The notebook completes the following data preparation steps:

Read the data from https://static.bc-edx.com/ai/ail-v-1-0/m18/lms/datasets/student-loans.csvLinks into a Pandas DataFrame. Review the DataFrame, looking for columns that could eventually define my features and target variables.

Create the features (X) and target (y) datasets. The target dataset is defined by the “credit_ranking” column. The remaining columns define the features dataset.

Split the features and target sets into training and testing datasets.

Use scikit-learn's StandardScaler to scale the features data.

Part 2: Compile and Evaluate a Model Using a Neural Network

Use TensorFlow to design a deep neural network model. This model uses the dataset’s features to predict the credit quality of a student based on the features in the dataset. Determine the number of layers that my model will contain or the number of neurons on each layer. Then, compile and fit my model. Finally, evaluate the model to calculate its loss and accuracy.

I completed the following steps:

Create a deep neural network by assigning the number of input features, the number of layers, and the number of neurons on each layer using TensorFlow’s Keras.

Compile and fit the model using the binary_crossentropy loss function, the adam optimizer, and the accuracy evaluation metric.

Evaluate the model using the test data to determine the model’s loss and accuracy.

Save and export my model to a keras file, and name the file student_loans.keras.

Part 3: Predict loan repayment success by using my neural network model

Use the model I saved in the previous section to make predictions on my reserved testing data.

I completed the following steps:

Reload my saved model, file student_loans.keras.

Make predictions on the testing data, saving them to a DataFrame and rounding the predictions to binary values.

Generate a classification report with the predictions and testing data.

Part 4: Discuss creating a recommendation system for student loans

Briefly answer the following questions:

Question 1: Describe the data that you would need to collect to build a recommendation system to recommend student loan options for students. Explain why this data would be relevant and appropriate.

Question 2: Based on the data you chose to use in this recommendation system, would your model be using collaborative filtering, content-based filtering, or context-based filtering? Justify why the data you selected would be suitable for your choice of filtering method.

Question 3: Describe two real-world challenges that you would take into consideration while building a recommendation system for student loans. Explain why these challenges would be of concern for a student loan recommendation system.