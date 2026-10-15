# 🚀 Predicting Falcon 9 First Stage Landings

**Applied Data Science Capstone Project**

Welcome! This project uses data science and machine learning to predict whether the SpaceX Falcon 9 first stage will land successfully.

## Why This Matters

SpaceX advertises Falcon 9 launches at about **$62 million**, while other providers charge upwards of **$165 million**. Much of that saving comes from reusing the first stage of the rocket. If we can predict whether the first stage will land successfully, we can estimate the cost of a launch more accurately. That insight is valuable to any company bidding against SpaceX for a launch contract.

## Project Highlights

- Collected launch data from the **SpaceX API** and scraped historical records from **Wikipedia**
- Explored the data with **SQL**, **Matplotlib**, **Seaborn**, and **Folium**
- Built an interactive dashboard with **Plotly Dash**
- Trained and tuned several classification models, reaching **94.44% accuracy** on the test set

## Project Workflow

The project is organized into seven modules, each building on the one before it.

### 1. Data Collection and Wrangling (SpaceX API)
- Sent GET requests to the SpaceX API to retrieve historical launch data.
- Cleaned and formatted the data, handling anomalies and missing values so it was ready for analysis.

### 2. Web Scraping (Wikipedia)
- Used **BeautifulSoup** to extract Falcon 9 launch records from Wikipedia.
- Parsed the HTML table into a **Pandas** DataFrame for easy manipulation.

### 3. Exploratory Data Analysis and Training Labels
- Explored patterns and correlations with **Matplotlib** and **Seaborn**.
- Identified and labeled the training data for the machine learning models.

### 4. Database Integration
- Loaded the dataset into a **Db2** database.
- Wrote SQL queries to answer specific questions about the launch data.

### 5. Feature Engineering and Geospatial Visualization
- Created new features to improve the predictive power of the models.
- Built interactive maps with **Folium**, marking launch sites and showing success and failure rates to reveal geographic patterns.

### 6. Interactive Dashboard (Plotly Dash)
- Developed a **Plotly Dash** application for real-time visual analytics of the launch data.
- Added dropdown menus and range sliders that drive interactive pie charts and scatter plots.

### 7. Machine Learning and Hyperparameter Tuning
- Standardized the data and split it into training and test sets.
- Tuned hyperparameters with **GridSearchCV** across several models, including SVM, Decision Trees, K-Nearest Neighbors, and Logistic Regression.
- Compared each model's performance on the test data to find the best performer.

## Results

| Model | Test Accuracy |
|-------|---------------|
| **Decision Tree Classifier** | **0.9444** |
| Support Vector Machine (SVM) | 0.8333 |
| K-Nearest Neighbors (KNN) | 0.8333 |

The **Decision Tree Classifier** was the best-performing model on the test set.

## Conclusion

By combining data collection, analysis, feature engineering, and model tuning, this project predicts Falcon 9 first stage landing success with strong accuracy. These predictions can help estimate launch costs and support competitive bids against SpaceX.


## Acknowledgments

- **IBM**, for the course and learning materials
- **Coursera**, for the platform to complete the course

## Get Started

Whether you're a data science enthusiast, a space exploration fan, or a professional interested in predictive modeling, we hope you find something useful here. Browse the notebooks to follow the full workflow, and feel free to open an issue or share feedback.
