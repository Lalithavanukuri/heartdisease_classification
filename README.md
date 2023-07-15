# heartdisease_classification

I collected this dataset from Kaggale named 'Heart Disease Dataset' which contains 13 attributes named 
age
sex
chest pain type (4 values)
resting blood pressure
serum cholestoral in mg/dl
fasting blood sugar > 120 mg/dl
resting electrocardiographic results (values 0,1,2)
maximum heart rate achieved
exercise induced angina
oldpeak = ST depression induced by exercise relative to rest
the slope of the peak exercise ST segment
number of major vessels (0-3) colored by flourosopy
thal: 0 = normal; 1 = fixed defect; 2 = reversable defect
and a target attribute whether they have a heart disease or not.
It contains 1026 feilds.



It is a CSV (comma seperated values)file.
1.Load dataset and read file.
The code reads a dataset from a CSV file named "heart.csv" using the pd.read_csv() function.
2.Preprocessing steps
It handles missing values by replacing with the mean value.
The dataset is split into features (X) and the target variable (y) using the drop() method and indexing.
The data is further split into training and testing sets using the train_test_split() function from scikit-learn.
The features are scaled using StandardScaler() to standardize the numerical values to have zero mean and unit variance.
3.Model Training 
A decision tree classifier model is created using DecisionTreeClassifier() from scikit-learn, with a random seed set to 42.
The model is trained on the training data using the fit() method, where it learns patterns and relationships in the features and target variable.
4.Model evaluation
Predictions are made on the testing data using the predict() method, where the model uses the learned patterns to classify the samples.
The accuracy of the model is evaluated by comparing the predicted labels with the true labels from the testing data using the accuracy_score() function from scikit-learn.

Lastly, a visualization of the decision tree is generated using export_graphviz() and displayed using Graphviz and the Image function, providing an intuitive representation of the learned decision-making process of the model.




