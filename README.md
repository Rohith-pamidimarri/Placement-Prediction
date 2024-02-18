# Placement Prediction Dataset Analysis and Modeling

## Introduction:

The dataset provides comprehensive information about students from Geethanjali Engineering College, Nellore, Andhra Pradesh, belonging to the 2015 batch. It serves as a valuable resource for research and analysis in the domain of higher education, particularly focusing on factors influencing student placements after graduation.

### Dataset Features:

- **Name:** The name of the student.
- **Roll_no:** Unique roll number assigned to each student.
- **Age:** Age of the student.
- **Gender:** Gender of the student (Male/Female).
- **Branch:** Academic discipline or field of study (e.g., Computer Science, Mechanical Engineering, etc.).
- **Internships:** Number of internships completed by the student, indicating practical experience.
- **CGPA:** Cumulative Grade Point Average (CGPA) representing the student’s academic performance.
- **Hostel:** Indicates whether the student resides in a hostel (Yes/No).
- **Backlogs:** Number of backlogs (unsuccessfully completed courses) the student has.
- **PlacedOrNot:** Binary variable indicating whether the student has been placed in a job after graduation (Yes/No). This serves as the target variable for placement prediction models.

## Analysis and Modeling Pipeline:

1. **Data Import**:
   - Necessary libraries were imported, and the dataset was loaded using pandas.

2. **Data Exploration and Cleaning**:
   - Checked for data inconsistencies like missing values and duplicates. None were found.
   - Checked for outliers in the 'Age' column using visualization and removed them.
   - Checked for outliers in the 'CGPA' column and found none.

3. **Data Transformation**:
   - Converted categorical columns ('Gender' and 'Branch') into numerical columns.
   - Dropped unnecessary columns ('Name' and 'Roll_no').
   - Split the data into features and target variables.
   - Normalized the data using StandardScaler.

4. **Feature Selection**:
   - Used Principal Component Analysis (PCA) to reduce dimensionality.
   - Visualized the new data after PCA.

5. **Model Building**:
   - Utilized Logistic Regression, Random Forest Classifier, and K-Nearest Neighbors for classification.
   - Evaluated each model's performance on the original dataset, PCA-transformed dataset, and Linear Discriminant Analysis (LDA)-transformed dataset.

6. **Model Evaluation**:
   - Evaluated models using classification reports, including precision, recall, and F1-score.

## Conclusion:

The analysis, preprocessing, and modeling pipeline provided valuable insights into the placement prediction dataset. The thorough exploration, cleaning, and transformation of the data enabled the construction and evaluation of predictive models. The findings suggest that, for this dataset, maintaining the original feature space may be more effective for certain classification algorithms. Further refinement and experimentation with different models and techniques could enhance the predictive performance and applicability of the models developed.

Great job on conducting a comprehensive analysis, preprocessing, and modeling pipeline for the placement prediction dataset! If you have any further questions or need additional assistance, feel free to ask!

