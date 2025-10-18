Airbnb NYC Price Prediction: Quantifying the $10.81 Capacity Premium

Course: MSDS692 – Data Science Practicum 1

Author: Barsha Kakshapati

Semester: Fall 2025

Repository: https://github.com/Barsha-bytes/Project-review-airbnb_subway.git

1. Project Overview & Business Impact

This project conducts a comprehensive analysis of Airbnb listing prices in New York City, moving beyond traditional pricing features (like bedroom count) to measure the value of Guest Experience (via sentiment) and Transit Accessibility (via distance to subway).

By building a robust predictive regression model, we identified a $40 Million Market Opportunity for hosts who strategically maximize capacity and customer service, as the current market undervalues these factors.

Key Performance Metric

Metric

Model

Value

Mean Absolute Error (MAE)

Baseline Linear Regression

$16.95

Status



Completed (Baseline), Random Forest Refinement Next

2. Methodology and Feature Engineering

The analysis integrates structured property data with unstructured textual data from guest reviews, utilizing advanced techniques to generate powerful predictive features.

Data Sources

Listings & Reviews: Sourced from Inside Airbnb.

Subway Data: MTA GTFS information used to map transit access across the city.

Review Text: Over 400,000 raw guest reviews used for sentiment analysis.

Technical Feature Creation

Special emphasis was placed on engineering features that drive value:

Feature

Data Type

Technical Method

Purpose

Distance to Subway

Structured

cKDTree (nearest neighbor)

Calculates the Euclidean distance (in meters) to the nearest subway station, quantifying convenience.

Sentiment Score

Unstructured (Reviews)

VADER Lexicon

Extracts the average compound sentiment score from guest reviews, quantifying service quality.

Guest Capacity

Structured

Regression Coefficient

The maximum number of guests a listing accommodates (the single largest price driver).

3. Key Quantitative Findings

The predictive modeling effort yielded precise, actionable insights into how price is truly determined in the NYC market:

The Capacity Premium (OFFENSE)

For every additional guest a property can accommodate, the listing earns a significant premium, demonstrating that space for people is more valuable than simple room count.

$$\text{Capacity Premium} = + \mathbf{\$10.81} \text{ per guest, per night}$$

The Transit Penalty (DEFENSE)

Listings that are farther from the subway system are penalized, highlighting the importance of convenience for NYC guests and the need to offset this cost.

$$\text{Transit Penalty} = - \mathbf{\$1.26} \text{ per point of Transit Score}$$

4. How to Run This Project (Reproducibility)

The project code is maintained in this GitHub repository and is fully reproducible using the provided Jupyter notebook.

Step 1: Download and Setup

Clone the repository to your local machine:

git clone [https://github.com/Barsha-bytes/Project-review-airbnb_subway.git](https://github.com/Barsha-bytes/Project-review-airbnb_subway.git)


Navigate to the project directory and install required dependencies:

cd Project-review-airbnb_subway
pip install -r requirements.txt


Step 2: Run the Analysis

The full analysis pipeline is contained within the core Jupyter notebook, which includes data loading, feature engineering, and the Linear Regression baseline model.

Core Notebook: airbnb_subway.ipynb

Supporting Documents

Full Presentation: Project Work (1).pdf .

Core Code: airbnb_subway.ipynb
