Airbnb Listings and Subway Analysis – NYC
Course: MSDS692 – Data Science Practicum 1
Author: Barsha Kakshapati
Semester: Fall 2025

Project Description (What the project is about)
This project analyzes Airbnb listings in New York City. I combined listing price/location data with unstructured guest reviews (measuring sentiment) and subway distance. My goal was to build a strong predictive model to find out exactly how much these factors influence price.

# Airbnb NYC Listings and Reviews Analysis: Predicting Price with Sentiment
2. Overview	## Project Overview This project conducts a comprehensive analysis of Airbnb listings in New York City, aiming to understand the factors that influence listing prices. The core approach is to build a robust predictive model by integrating two distinct data sources: structured property data and unstructured text data from guest reviews.
3. Metadata	### Project Details * **Course:** MSDS692 – Data Science Practicum 1 * **Author:** Barsha Kakshapati * **Semester:** Fall 2025

Export to Sheets
Step 2: Detail Data Sources and Feature Engineering (The "How")
Explain the key features you created, as these are the main drivers of your analysis.

Action	Suggested Markdown Content (Copy/Paste)
1. Data Sources	## Data and Methodology The analysis combines the following external datasets: * **Listings & Reviews:** Sourced from Inside Airbnb. * **Subway Data:** MTA GTFS information for transit proximity.
2. Key Features	### Feature Engineering Focus Special emphasis was placed on transforming unstructured data into predictive features (Week 4): * **Sentiment Score:** The average compound score of guest reviews using the VADER lexicon. * **Distance to Subway:** Calculated using a **cKDTree** to find the nearest subway station distance in meters for each listing. * **Property Type:** One-hot encoded property classifications and other structural features like **Guest Capacity**.

Export to Sheets
Step 3: Present Modeling and Key Findings (The "What")
Showcase your success with quantitative results, which are more impactful than a general description.

Action	Suggested Markdown Content (Copy/Paste)
1. Modeling Approach	## Predictive Modeling and Results The project follows a standard machine learning pipeline for price prediction (regression). The process began with a **baseline Linear Regression** model and is being refined with a **Random Forest** model to maximize accuracy.
2. Performance Table	### Model Performance Summary `
3. Top Drivers	### Top Price Drivers The analysis identified the following key factors driving pricing variation: 1. **Property Type** (e.g., Hotel vs. Apartment) 2. **Guest Capacity** (number of people accommodated) 3. **Sentiment Score** (how good the guest reviews are)
4. Current Status	## Project Status * **Status:** In Progress (90% complete for Week 5). * **Completed:** Data cleaning, feature engineering, and baseline Linear Regression model training/evaluation are complete. * **Next Steps:** Evaluate baseline performance plots, test and refine the Random Forest model (Week 6).

Export to Sheets
Step 4: Add Reproducibility Instructions
Provide clear instructions so anyone can download and run your work.

Action	Suggested Markdown Content (Copy/Paste)
1. Instructions	## How to Run This Project The project code is maintained in this GitHub repository, which contains Jupyter notebooks and Python scripts for full reproducibility. ### **Step 1: Download and Setup** 1. Clone the repository to your local machine: ```bash git clone https://github.com/Barsha-bytes/Project-review-airbnb_subway ````<br>2. Navigate to the project directory and install required dependencies (assuming a requirements.txt is available):<br> ```bash<br>cd Project-review-airbnb_subway` `pip install -r requirements.txt` ` ```` `### Step 2: Run the Analysis` `The analysis can be run sequentially through the following notebooks:` `* `1_Data_Collection_and_Cleaning.ipynb` `* `2_Feature_Engineering_and_Sentiment.ipynb` `* `3_Predictive_Modeling_Baseline.ipynb` (Contains the Linear Regression and MAE calculation)` `* `4_Model_Refinement_and_Results.ipynb` (Contains the Random Forest and final results)`
git clone [https://github.com/Barsha-bytes/Project-review-airbnb_subway.git](https://github.com/Barsha-bytes/Project-review-airbnb_subway.git)

Open the main notebook: Look in the notebooks/ folder for airbnb_subway.ipynb.

Visualizations
Once you save your plots (charts) and upload them to the visualizations/ folder, they will appear here!
