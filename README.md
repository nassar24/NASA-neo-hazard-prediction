

---

## NASA NEO Hazard Prediction

Outer space is teeming with an infinite number of objects, some of which are much closer to Earth than we realize. While a distance of 70,000 km might seem harmless, in astronomical terms, it’s incredibly close and capable of disrupting natural phenomena. These near-Earth objects (NEOs), including asteroids, can pose significant risks. Therefore, it’s crucial to understand what surrounds us and identify potential threats.

### Project Overview
This project aims to build a machine learning model to classify asteroids based on their hazard status. The dataset contains information about various characteristics of asteroids, and the goal is to predict whether an asteroid is hazardous or not.

### Data
The dataset is from Kaggle: The NASA certified asteroids that are classified as the nearest Earth objects are contained. The dataset contains 338,199 records with 9 columns.

**Key columns include:**
- `neo_id`: Unique identifier for each NEO.
- `name`: Name of the NEO.
- `absolute_magnitude`: Measure of the intrinsic brightness of the NEO.
- `estimated_diameter_min` and `estimated_diameter_max`: Minimum and maximum estimated diameters of the NEO.
- `relative_velocity`: Speed at which the NEO is traveling relative to Earth.
- `miss_distance`: Distance by which the NEO misses Earth.
- `is_hazardous`: Boolean indicating if the NEO is potentially hazardous.
- `orbiting_body`: The celestial body that the NEO is orbiting; all records show “Earth”.

**Missing values are present in the columns:**
- `absolute_magnitude`: 28 missing values.
- `estimated_diameter_min`: 28 missing values.
- `estimated_diameter_max`: 28 missing values.

The proportion of missing values in these columns is very low (about 0.0083%).

### Project Steps
#### Data Preparation
- **Data Cleaning**: Removed irrelevant columns and handled missing values.
- **Feature Engineering**: Created new features such as `diameter_ratio` and `velocity_distance`.
- **Handling Imbalance**: Used SMOTE to balance the dataset.

#### Exploratory Data Analysis (EDA)
- **Visualized** the distribution of features.
- **Examined** the correlation between features.

#### Modeling
- **Split** the dataset into training and testing sets.
- **Trained and evaluated** using Random Forest Classifier.

#### Evaluation
- **Used metrics** such as accuracy, precision, recall, and F1 score.
- **Generated** classification reports and confusion matrices.

---

