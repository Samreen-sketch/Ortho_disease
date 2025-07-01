# Ortho_disease
What is Biomechanic in Orthopedic :
Biomechanics in orthopedics refers to the study of how the human body moves, how forces act on bones, joints, and muscles, and how these forces affect movement, stability, and injury — especially in orthopedic patients.
The biomechanical characteristics are especially used in orthopedic and spinal health research in datasets like the Vertebral Column Data Set, where measurements of the vertebral column (lumbar lordosis angle, pelvic incidence, etc.) are used as features to:
•	Diagnosing spinal issues
•	Divide the patients into three categories: 
spondylolisthesis, hernia, and normal.
# The most widely used models for this data
•	RandomForestClassifier
•	XGBClassifier
•	Logistic Regression
# Why XGBClassifier Model is used
High accuracy and good handling of non-linear data.
# Import Libraries

These libraries help build and evaluate models to classify text data effectively.
# Import csv file
The data was loaded into a pandas DataFrame for analysis and model training.
![image](https://github.com/user-attachments/assets/a42c8640-5dc7-4d1e-8a5e-a073288d0558)
![image](https://github.com/user-attachments/assets/c2b8ffbb-6c93-40ee-b147-acc8af1de85b)
# Preprocessing in wrangler mode
 To analyze and preprocess biomechanical features of orthopedic patients
- Includes variables such as pelvic tilt, sacral slope, lumbar lordosis, and class labels (e.g., normal, hernia, spondylolisthesis)
- ![image](https://github.com/user-attachments/assets/cb1041b2-b0b1-4752-93d7-0a5622857807)
-  # Separate features and target
-  # Train-test split
-  This split allows the model to be trained on one portion of the data and tested on unseen data to evaluate performance.
-  # Initialize XGBoost model
-  # Train the model
-  # Predict and evaluate
-  After training, the model was evaluated using the test dataset.
-  Classification Report: Shows precision, recall, F1-score, and accuracy for each class.
-  Confusion Matrix: Displays the number of true positives, true negatives, false positives, and false negatives.
-  ![image](https://github.com/user-attachments/assets/50e98647-df49-4c52-b6a7-953a7917b2e8)
- # Conclusion Of The Evaluation Result
🔹	Class 0:
•	Support: 12 real-world examples
•	Predicted correctly: 7
•	Mislabeled as:
•	Class 1 → four times
•	Class 2 → One instance
•	Precision: 0.58 (only 58% of the 0s that were predicted were actually 0).
•	Recall: 0.58, meaning that only 58% of real zeros were accurately anticipated.
•	➤ Class 0 (Hernia) presents challenges for the model
🔹 Class 1: 
•	18 real samples are supported.
•	Accurately anticipated: 13.
Misclassified as:
•	Class 0: 5 times
•	Accuracy: 0.76
•	Recall: 0.72
•	➤ Moderate performance for Class 1(Normal)
🔹 Class 2:
•	Support: 32 actual samples
•	Correctly predicted: 32
•	Misclassified: 0 times!
•	Precision: 0.97
•	Recall: 1.00 (100%)
•	➤ Excellent performance on Class 2 (degree_spondylolisthes)
# Visualization:
Correlation Heatmap
![image](https://github.com/user-attachments/assets/b4baa0e5-0ddb-4dfe-98d5-abb37d9064ba)
# Box Plot
![image](https://github.com/user-attachments/assets/26015790-de5a-44b1-840f-a9ce9a61efbf)
Insight of Visual:
This illustration demonstrates how the distribution of lumber lordosis angles varies by class. However, it is high in class 2, which is spondylolisthesis, indicating that a number of instances fall under this category of spinal condition. 
![image](https://github.com/user-attachments/assets/4ed4a92a-fb00-4a4d-aef2-2ba5a1b51dc5)
This graphic illustrates how the distribution of pelvic indices varies by class. However, it is high in class 2, which is spondylolisthesis, indicating that a number of instances fall under this category of spinal condition. 
![image](https://github.com/user-attachments/assets/7bf23668-a8f9-463a-99e4-ffd6fa439697)
# Findings of this evaluation and Visualisation
The vertebral column dataset is nearly precise. The real and projected values do not differ significantly. The visualization also demonstrates that spondylolisthesis condition is present in a number of patients based on actual data. Evaluation of machine learning models is likewise the same










