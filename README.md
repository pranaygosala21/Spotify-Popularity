## Spotify Popularity Analysis

This project is focused on analyzing the popularity of songs on the Spotify platform. By using data visualization and machine learning techniques, we aim to gain insights into the factors that contribute to a song's popularity and build a model to predict the popularity of songs based on their features.

### Dataset

The dataset used for this analysis is stored in a CSV file named "SpotifyFeatures.csv". It contains various attributes of songs available on Spotify, such as acousticness, danceability, energy, instrumentalness, key, loudness, mode, popularity, and more. Each row represents a unique song.

### Libraries Used

To run the code and perform the analysis, the following Python libraries are required:

- NumPy: For numerical computations.
- Pandas: For working with dataframes and data manipulation.
- Seaborn: For data visualization.
- Matplotlib: For additional plotting functionalities.
- scikit-learn: For building the machine learning model.

### Code Overview

1. Data Loading:
   The first step in the code is to load the dataset into a Pandas dataframe using the `pd.read_csv()` function. Make sure to update the file path accordingly if the dataset is located in a different directory.

2. Data Visualization:
   Several data visualizations are created using Seaborn to understand the distribution of popularity and its relationship with different features like time signature, key, and mode. Additionally, the acousticness and loudness distributions for songs with popularity greater than 50 are plotted.

3. Data Preprocessing:
   To prepare the data for machine learning, the 'time_signature' column is transformed into numerical values.

4. Model Training and Evaluation:
   A Random Forest Classifier model is trained using a subset of the data. The accuracy and AUC score of the model are calculated and printed as evaluation metrics.

5. Confusion Matrix (Missing):
   The code includes an attempt to display the confusion matrix for the model's predictions, but the relevant code snippet is missing. The confusion matrix is useful for evaluating the performance of the classification model.

### Running the Code

To run the code and perform the analysis, ensure that you have all the required libraries installed. You can install them using `pip install library_name`.

Make sure to place the "SpotifyFeatures.csv" file in the specified path or update the file path in the code accordingly.

Execute the code in a Python environment that supports Jupyter notebooks or plain Python scripts.

### Further Improvements

- Data Cleaning: Additional data cleaning steps can be incorporated, such as handling missing values, outlier detection, and feature scaling if needed.

- Hyperparameter Tuning: The model's hyperparameters can be optimized using techniques like Grid Search or Random Search to improve its performance.

- Feature Selection: Investigate which features have the most significant impact on the popularity prediction and consider selecting the most relevant ones to enhance the model's accuracy.

- Confusion Matrix Display: If the missing part of the confusion matrix display is found, it can be included to provide a comprehensive evaluation of the model's performance.
