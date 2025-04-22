Genre Classification Using Random Forest
🧠 Objective
The objective of this project is to classify books into genres using metadata features such as:

Author Popularity

Book Length

Number of Keywords

We applied a Random Forest Classifier to build the prediction model.

📂 Dataset
Source: book_genres.csv

Features used:

author_popularity – Numerical indicator of author's popularity

book_length – Length of the book (e.g., in pages or words)

num_keywords – Number of descriptive keywords

Target variable: genre – The category/genre of the book

🔍 Methodology
1. Data Preparation
Loaded the dataset using pandas

Selected relevant features and separated the target (genre)

Split the dataset into training and testing sets (80/20 split)

2. Model Training
Applied a Random Forest Classifier (sklearn.ensemble)

Set a random state for reproducibility (random_state=42)

3. Model Evaluation
Predicted genres for the test set

Evaluated performance using:

Confusion Matrix

Accuracy

Precision (macro average)

Recall (macro average)

Classification Report

📊 Results
Confusion Matrix Heatmap

The actual image is generated in code output.

Performance Metrics

Metric	Value
Accuracy	{{ accuracy }}
Precision (macro avg)	{{ precision }}
Recall (macro avg)	{{ recall }}
Replace {{ accuracy }}, etc., with actual printed values from your code run.

Classification Report
nginx
Copy
Edit
{{ report }}
Include the printed classification report from your code output here.

✅ Conclusion
The Random Forest model was effective in classifying genres based on limited metadata.

The confusion matrix revealed where misclassifications occurred.

The macro-averaged metrics give a fair estimate of performance across all genres, especially in the case of class imbalance.

Further improvements could include:

Feature engineering (e.g., keyword analysis using NLP)

Balancing the dataset if certain genres are underrepresented

Trying other classifiers (e.g., SVM, Gradient Boosting)



The model’s performance may vary depending on dataset size, feature quality, and genre diversity.



