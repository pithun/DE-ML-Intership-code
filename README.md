### DESCRIPTION
A phishing website is a domain similar in name and appearance to an official website. They're made in order to fool someone into believing it is legitimate.
Today, phishing schemes have gotten more varied, and are potentially more dangerous than before.

We try to use some features of sites and machine learning techniques to identify these sites.

Model is trained using dataset with up to 30 features and 1372 training records.

### Dataset
Task: Classification

Data Type: Categorical

### TOOLS/TECHNOLOGIES USED
- Python
- Pandas
- Numpy
- Matplotlib
- Scikit-learn

### APPROACH
I started by cleaning which involved checking for missing values, doing a duplicate search where duplicates were found and removed, ensuring consistency in values 
across features. I then did some EDA showing the distribution of the classes in the dataset, we had 52% of sites not being a phishing site and 48% being one. 
I used train test split to then divide the dataset into training and testing sets with 20% of data used for testing. I then initialized three models and trained and
tested performance with the test set. I then did a four fold cross validation to get the best model (a Random Forest model) and tuned it. See all pretuned and tuned
model results below. 


### Algorithms Implemented
- Random Forest Classifier (96.22% model accuracy)
- XG Boost Classifier (97.09% model accuracy)
- CatBoost Classifier (96.80% model accuracy)

#### Random Forest Classifier (97.67% accuracy after tuning)
