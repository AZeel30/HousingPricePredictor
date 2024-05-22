# HousingPricePredictor

This program is designed for predictive modeling of house prices using the scikit-learn library in Python. It follows the typical machine learning workflow, including data preprocessing, model training, evaluation, and dimensionality reduction using PCA.

1. **Data Preprocessing**:
   - The program starts by importing necessary libraries for data manipulation and modeling, including NumPy, Pandas, Matplotlib, Seaborn, and scikit-learn.
   - It reads the dataset containing information about house properties.
   - The data is prepared for modeling by removing irrelevant columns ('id' and 'price') and converting categorical variables into numerical format if needed.

2. **Model Training**:
   - It splits the data into training and testing sets using the train_test_split function from scikit-learn.
   - Two regression models, Linear Regression and Gradient Boosting Regressor, are trained on the training data to predict house prices.
   - The Gradient Boosting Regressor is configured with specific hyperparameters such as the number of estimators, maximum depth, minimum samples split, learning rate, and loss function.

3. **Model Evaluation**:
   - The performance of the models is evaluated on the test set using the score method to assess their predictive accuracy.
   - Additionally, the loss on the test set for each stage of the gradient boosting process is calculated and plotted to visualize model deviance during training.

4. **Dimensionality Reduction**:
   - The program employs Principal Component Analysis (PCA) for dimensionality reduction on the scaled features of the training data. This helps in reducing the complexity of the dataset while preserving most of the information.

Overall, this program provides a comprehensive pipeline for training predictive models of house prices, including data preprocessing, model training, evaluation, and dimensionality reduction techniques.
