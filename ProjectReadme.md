Here is where you include:

  - Background on your code files
  My workbook uses the training and test data from the 2016 Kaggle Competition "Two Sigma Connect: Rental Listing Inquiries". The objective is to predict the interest level for listings as low, medium, or high (multi-class classification). The workbook consists of three main sections: exploratory data analysis, feature engineering, and hyperparameter tuning. The classification model used was lightGBM, a gradient boosting framework similar to xgboost but with faster performance.
  
  - How to run your code, guide to install any additional packages
  The training and test dataset could not be uploaded onto github because they exceeded the size limit (25MB). In order to run the code, downloaded and unzip the dataset from this link. [link] (https://www.kaggle.com/c/two-sigma-connect-rental-listing-inquiries/data). Make sure that the datasets are placed in appropriate directory or change the relative paths specified in the workbook.
  The workbook uses many of the standard data visualization and machine learning packages used in lectures including numpy, pandas, matplotlib, seaborn, and sklearn. In addition, I also used nltk for text preprocessing and lightgbm for model training; these can be installed using the commands 'pip install nltk' and 'pip install lightgbm'.

  
  - Results, interpretation and reflection
  RESULTS
  I chose lightgbm as the machine learning model because this was the model used by the Calgary DataScience Academy in their workbooks, which I referenced for my project. LightGBM is also popularly used in Kaggle competitions and has faster performance compared to xgboost.
  I started with a baseline model, which was trained with the default parameters for lightGBM and used only the numerical features in the original data set. This resulted in a log loss of 0.65189 for the validation set. The log loss was reduced to 0.56295 with feature engineering and further reduced to 0.55878 with hyperparameter tuning. Finally, the model achieved a log loss of 0.56065 of the test dataset, which I obtained by submitting my prediction to the competition.
  
  INTERPRETATION
  The objective of this project is to select a Kaggle competition and try to put together a solution for the problem. I chose the 2016 Kaggle Competition "Two Sigma Connect: Rental Listing Inquiries". I started with exploratory data analysis, to identify patterns in the data which will help with the feature engineering. I build a baseline model, using only the numerical features in the original dataset. Then I applied feature engineering and hyperparameter tuning, which led to significant improvement in model performance. My best model achieved a log loss of 0.56065 on the test data. Compared to the winner of this kaggle competition, who achieved a log loss of 0.49194, there is still significant room for improvement. With additional time, I would do more exploratory data analysis and feature engineering to capture more patterns in the data.
  
  REFLECTION
  There was no deviation from the project proposal. In the proposal, I have outlined that I will compete in the 2016 Kaggle Competition "Two Sigma Connect: Rental Listing Inquiries", using lightGBM as my machine learning model, and apply exploratory data analysis, feature engineering, and hyperparameter tuning. All the outlined components are completed for the project.