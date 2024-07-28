# Sleep Health and Lifestyle

This synthetic dataset contains sleep and cardiovascular metrics and lifestyle factors of close to 400 fictive persons.

The workspace is set up with one CSV file, `data.csv`, with the following columns:

- `Person ID`
- `Gender`
- `Age`
- `Occupation`
- `Sleep Duration`: Average number of hours of sleep per day
- `Quality of Sleep`: A subjective rating on a 1-10 scale
- `Physical Activity Level`: Average number of minutes the person engages in physical activity daily
- `Stress Level`: A subjective rating on a 1-10 scale
- `BMI Category`
- `Blood Pressure`: Indicated as systolic pressure over diastolic pressure
- `Heart Rate`: In beats per minute
- `Daily Steps`
- `Sleep Disorder`: One of `None`, `Insomnia` or `Sleep Apnea`

**Background**: You work for a health insurance company and are tasked to identify whether or not a potential client is likely to have a sleep disorder. The company wants to use this information to determine the premium they want the client to pay.<br>

**Objective**: Construct a classifier to predict the presence of a sleep disorder based on the other columns in the dataset.<br>
**Methods Used**:Exploratory Data Analysis, Inferential Statistics, Data Visualization, Machine Learning, Predictive Modeling.<br>
**Type of Problem**: Multi-class Classification Task. <br>
**Language, Libraries, technologies used**: Python, Pandas, Matplotlib, Seaborn, Numpy, Scipy, Scikit-learn, joblib<br>
## KEY INSIGHTS: 
To start this project, I first checked that all the data was clean and matched the description in the data dictionary; I cleaned up the data that wasn't clean and then validated all my data.<br>
Once my data was clean, I carried out an exploratory data analysis, followed by statistical tests which revealed that : 
 - Those whose occupation is Accountant, Doctor, Engineer, or Lawyer are less likely to have a sleep disorder nurses have a high chance of sleep apnea, and Salespersons and Teachers are more likely to have insomnia
 - Overweight people have a high chance to suffer from a sleep disorder and people with an ideal or normal Blood pressure are less likely to have a sleep disorder.
 -  People between the ages of 50 and 60 have low-stress levels, and a sleep quality of around 9, but are susceptible to sleep apnea <br>
 - Men and women aged between 42 and 45 are very likely to have insomnia, and women of 50 and above 55 have a very high chance of having sleep apnea <br>
After that, I preprocessed my data and created a baseline model: A LogisticRegression and a comparison model: A DecisionTree,
i fitted both models and evaluated them. With an accuracy of 89% the baseline model performs better .<br>

I plotted the importance of each variable to see which variables contributed the most to the model prediction. I saved the model as a pickle file using joblib




Source: [Kaggle](https://www.kaggle.com/datasets/uom190346a/sleep-health-and-lifestyle-dataset/)
