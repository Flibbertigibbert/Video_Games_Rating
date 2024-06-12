# Video_Games_Rating

**Machine Learning Problem: Video Games Rating Prediction**

## Project Description

 Dataset Link : https://www.kaggle.com/datasets/ibriiee/video-games-sales-dataset-2022-updated-extra-featThe project includes steps for setting up a virtual environment, installing necessary packages, and running a machine learning model using Python.

## Setup

To set up the project environment, follow these steps:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/BrainTumourClassification.git
   cd BrainTumourClassification
   ```

2. **Create a virtual environment:**
   ```bash
   python3 -m venv myenv
   ```

3. **Activate the virtual environment:**
   - On macOS and Linux:
     ```bash
     source myenv/bin/activate
     ```
   - On Windows:
     ```bash
     myenv\Scripts\activate
     ```

4. **Install the required packages:**
   ```bash
   pip install -r requirements.txt
   ```
## Data Directory

The data directory should be structured as follows:
```
data/
|-- train/
|   |-- class1/
|   |-- class2/
|   ...
|-- test/
|   |-- class1/
|   |-- class2/
|   ...
```
Each subdirectory (`class1`, `class2`, etc.) contains images of brain tumours classified into respective categories.

![image](https://github.com/Flibbertigibbert/Video_Games_Rating/assets/43761458/cd19a102-a48b-42c1-a2c0-b1e59deaf922)
![image](https://github.com/Flibbertigibbert/Video_Games_Rating/assets/43761458/cd19a102-a48b-42c1-a2c0-b1e59deaf922)


## Training and Testing(**Model Details:Pipeline for Categorical Feature Processing:**)
Training Phase: A machine learning pipeline has been built to predict video game ratings
The simplified flow is as follows:
1. Data management is done using pandas.
2. Data preprocessing, including encoding and handling missing values, is carried out using sklearn.
3. XGBoost is employed for prediction.
4 The data is split into training and testing sets.
5 The model is trained on the training data.


Testing involves:
1. Loading and preprocessing the test data.
2. Using the trained model to make predictions on the test set.
3. Model accuracy, precision, recall, and F1-score are evaluated on the test data.
4. Save Your Model: Save the trained model to disk using a serialization library like joblib or pickle.

The model's performance can be evaluated based on the provided metrics:

Accuracy (0.7069): This metric indicates the overall correctness of the model's predictions. An accuracy of 0.7069 suggests that about 71% of the predictions made by the model are correct.

Precision (0.6768): Precision reflects the model's ability to correctly identify positive instances among all instances predicted as positive. A precision score of 0.6768 means that approximately 68% of the instances predicted as positive are actually positive.

Recall (0.6477): Recall, also known as sensitivity or true positive rate, measures the model's ability to correctly identify positive instances among all actual positive instances. A recall of 0.6477 indicates that around 65% of actual positive instances are correctly identified by the model.

F1-score (0.6561): The F1-score is the harmonic mean of precision and recall, providing a balanced measure of a model's performance. A higher F1-score (0.6561 in this case) suggests a good balance between precision and recall.

Overall, the model appears to have decent performance based on these metrics.

## Deployment on Streamlit

1.Install Streamlit: Make sure you have Streamlit installed.
````bash 
  pip install streamlit
  ````
2. Create a New Python Script: Create a new Python file, e.g., app.py
3. Import Necessary Libraries: Import Streamlit and other necessary libraries in your script.
4. Run the App: Test your Streamlit app locally by running the following command in your terminal:
5. Deploy the App

The trained XGBClassifier model has been successfully deployed on Streamlit, allowing users to input relevant data such as the year of release, genre, platform, publisher, global sales, critic score, critic count, user score, and user count. The model then processes this input to predict the video game rating, providing valuable insights for decision-making purposes.
## Usage

To run the notebook, follow these steps:

1. **Start Jupyter Notebook:**
   ```bash
   jupyter notebook
   ```

2. **Open the `Notebook.ipynb` notebook:**
   Navigate to the directory where the notebook is located and open it in your web browser.

3. **Run the notebook:**
   Follow the instructions and run each cell sequentially to train and evaluate the brain tumour classification models.

## Libraries Used

The following libraries are used in this project:
- sklearn
- matplotlib
- numpy
- pandas
- xgboost
- itertools
- os
- shutil
- warnings

## Contributing

Contributions are welcome! If you have any improvements or suggestions, please create a pull request or open an issue.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
