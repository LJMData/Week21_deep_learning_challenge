# Week21_deep_learning_challenge

### Project Description
This project aims to use machine learning to help identify which organizations are worth donating to and which are high-risk using artificial neural networks. The dataset used in this project is provided by a non-profit organization, Alphabet Soup. The goal is to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup, based on various features provided in the dataset.

### Preprocessing
The preprocessing step involves cleaning and formatting the data to be used by the machine learning model. In this project, the following preprocessing steps were taken:

* Dropping non-beneficial ID columns, 'EIN' and 'NAME'.
* Binning categorical variables that have few unique values and replacing them with "Other".
* Encoding categorical variables using one-hot encoding.
* Splitting the preprocessed data into training and testing datasets.
* Scaling the data using StandardScaler.
* Compile, Train and Evaluate the Model

The model used in this project is a deep neural network with seven hidden layers. The model was compiled using binary cross-entropy as the loss function and the Adam optimizer. The model was trained with 100 epochs and was saved every five epochs using a callback function.

After training the model, it was evaluated using the test dataset, and the loss and accuracy were calculated. The final trained model was saved as an HDF5 file.

### Dependencies
pandas
sklearn
tensorflow

### How to Run
* Download the dataset "charity_data.csv" from the following URL: https://static.bc-edx.com/data/dl-1-2/m21/lms/starter/charity_data.csv
* Install the necessary dependencies using pip or conda.
* Open the Jupyter notebook or Python file containing the code.
* Run the code in the file.
* The trained model will be saved as an HDF5 file.