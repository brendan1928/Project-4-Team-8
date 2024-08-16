# About the Project
## Project Statement 1: Personalized Medical Recommendation System (Text Based Input)

### Link to Presentation : https://www.canva.com/design/DAGNsaCV2aE/t70h1j2Ws90ylKeiccywUg/edit
- ML Model Notebook : https://github.com/brendan1928/Project-4-Team-8/blob/main/HealthCareML_Code_Roshni.ipynb  
- To run Flask-API dash board : https://github.com/brendan1928/Project-4-Team-8/blob/main/main.py
- Dashboard link through Terminal  
  ![image](https://github.com/user-attachments/assets/4e5f3b45-ec5c-42c1-9ce7-ea9ff73fbac6)

### Overview:
The Personalized Medical Recommendation System is designed to empower users with tailored healthcare guidance by leveraging advanced machine learning techniques. The system integrates user-provided symptoms and health data to predict potential diseases, recommend personalized medications, and suggest suitable workout routines. Implemented as a Flask API, the system ensures accessibility and scalability, making it available across various devices.

### Machine Learning Approach:

- Model Selection: The system employs classification models like Random Forest and Decision Trees to predict diseases based on input symptoms.
- Personalization: The recommendation engine generates medication advice and workout plans, adapting to individual health profiles.
- Regression Analysis: Regression models are used for tasks like adjusting medication dosages, ensuring precise and effective recommendations.
- Challenges Addressed: Data consistency, feature engineering, model optimization, and user privacy were key challenges, each addressed with targeted solutions.

### Outcome:
This system enhances healthcare accessibility by offering accurate, real-time medical advice, tailored to each user's unique needs, while maintaining high standards of privacy and security.

## Project Statement 2: Pneumonia Detection App Using Deep Learning (Image Based Input)
> [!IMPORTANT]
> Key information users need to know to achieve their goal.  
- NOTE: All the files regarding this app, ML model, python file for code, Data set for input are located under `PNEUMONIA-detection_Deep-Learning_Chest-X-Ray-image-Recognition` Folder
#
- ML Model Notebook : https://github.com/brendan1928/Project-4-Team-8/blob/main/Pneumonia_Detection_Chest-XRay_image_recognition/ML_Model_Code_Roshni.ipynb
- To run App : 

#
### Overview:
The Pneumonia Detection App is a desktop application designed to assist in the early detection of pneumonia using chest X-ray images. Developed with a focus on ease of use and accuracy, the application employs deep learning models to analyze X-ray images, providing real-time feedback through a user-friendly interface built with PyQt5.

### Machine Learning Approach:

- Model Selection: The application utilizes a TensorFlow-based deep learning model, specifically the VGG16 architecture, to perform image recognition and detect signs of pneumonia from X-ray images.
- Image Processing: The model processes images by extracting relevant features, enabling accurate classification of pneumonia cases.
- Real-Time Detection: The application delivers results instantaneously, offering both visual and audio feedback to the user.
- Challenges Addressed: Key challenges included optimizing the deep learning model for speed and accuracy, managing large image datasets, and ensuring the interface is intuitive for non-technical users.
- Speech Audio Result: The application features speech synthesis to audibly convey the diagnosis, ensuring that users can receive and understand their results in an accessible and clear Audio.
### Outcome:
This app serves as a valuable tool for healthcare professionals and individuals alike, providing a reliable, real-time method for pneumonia detection, thereby facilitating timely medical intervention.
<br />
## The Problem Statement 

The AI model attempts to answer the following questions in an attempt to quell the overburdened healthcare system Canada is currently experiencing:
<br/>
•	Can a professional’s expertise be reflected in a single model, allowing for higher volume of diagnoses?
<br/>
•	What is an inaccuracy in this model, what is the risk, and how can it be accounted for?
<br/>
•	Can this model and data be used proactively for resource allocation & funding decisions?
<br/>

## The Model

This project uses diagnoses data to create clear links between symptoms and diseases, as well as provides recommendations on how to diet and exercise according to the predicted disease. It also supports photoimaging of the lungs to flag if an infection is detected.
<br/>
The data is first loaded in to Python with the Pandas library and cleaned to ensure optimal performance of the database and model; outputs are validated using the Matplotlib and Seaborn libraries.
<br/>
The data is then loaded in and stored in a database; the AI model pulls from this database, and uses a Single Vector Machine model to equate symptoms with diseases. It does this via a flask-hosted app where the user can type in up to four symptoms – the app has input validation and synonym dictionaries to help guide the user.
<br/>


## Data Sources

Kaggle Diagnoses Data
<br/>
https://www.kaggle.com/datasets/noorsaeed/medicine-recommendation-system-dataset/data
<br/>
CBC Healthcare System is Overburdened
<br/>
https://www.cbc.ca/news/canada/toronto/healthcare-staff-union-survey-1.7073334
<br/>

## Evaluation Standards

The model will be evaluated on a points-system with 100 potential points.

### Data Model Implementation (25 points)

•	A Python script initializes, trains, and evaluates a model (10 points)
<br/>
•	The data is cleaned, normalized, and standardized prior to modeling (5 points)
<br/>
•	The model utilizes data retrieved from SQL or Spark (5 points)
<br/>
•	The model demonstrates meaningful predictive power at least 75% classification accuracy or 0.80 R-squared. (5 points)

### Data Model Optimization (25 points)
•	The model optimization and evaluation process showing iterative changes made to the model and the resulting changes in model performance is documented in either a CSV/Excel table or in the Python script itself (15 points)
<br/>
•	Overall model performance is printed or displayed at the end of the script (10 points)

### GitHub Documentation (25 points)

•	GitHub repository is free of unnecessary files and folders and has an appropriate .gitignore in use (10 points)
<br/>
•	The README is customized as a polished presentation of the content of the project (15 points)

### Group Presentation (25 points)

•	All group members speak during the presentation. (5 points)
<br/>
•	Content, transitions, and conclusions flow smoothly within any time restrictions. (5 points)
<br/>
•	The content is relevant to the project. (10 points)
<br/>
•	The presentation maintains audience interest. (5 points)
<br/>

## Challenges and Solutions ( Optimization,  Logging & Formation)
1. Data Cleaning
- Optimization: Performance bottlenecks were resolved by replacing inefficient loops with vectorized operations.
- Logging: Introduced logging to track cleaning steps like missing value handling and outlier detection.
- Formatting: Standardized inconsistent formats across datasets using custom functions.

2. Model Building
- Optimization: Employed Grid Search and Random Search to reduce hyperparameter tuning time.
- Logging: Added detailed logs for model training, validation scores, and hyperparameters.
- Formatting: Ensured consistent feature scaling and encoding to avoid model fitting errors.

3. Dictionaries and Synonyms
- Optimization: Improved synonym mapping speed by using hash maps.
- Logging: Implemented version control to track dictionary updates and their effects.
- Formatting: Standardized synonym formats to maintain data consistency.

4. Auto-Correcting Functions
- Optimization: Refined auto-correct algorithms to enhance processing speed.
- Logging: Added logging to trace applied corrections for better error analysis.
- Formatting: Ensured corrected inputs aligned with standardized formats.

5. Schema Diagrams and Relationships
- Optimization: Simplified schema design by normalizing data for efficient queries.
- Logging: Established version control for schema changes.
- Formatting: Regularized data types and clarified relationships to ensure smooth integration.

# Conclusion

The model concludes that there is a very large opportunity for the use of AI/ML in the Healthcare industry; while risk of inaccuracies necessitate some level of human supervision, high initial accuracy rates over a large number of requests indicate that these tools can be used as a filtering mechanism to ‘bucket’ diagnoses, flagging responses with similar historically inaccurate results.


# Contact

For any comments or suggestions on the model, feel free to check the Contacts page on either app in the repo for task breakdown and ownership. Contributors' GitHub pages are also included in the list of Contributors to the repo.
