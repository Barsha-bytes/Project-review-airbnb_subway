Airbnb Listings and Subway Analysis – NYC
Course: MSDS692 – Data Science Practicum 1
Author: Barsha Kakshapati
Semester: Fall 2025

Project Description (What the project is about)
This project analyzes Airbnb listings in New York City. I combined listing price/location data with unstructured guest reviews (measuring sentiment) and subway distance. My goal was to build a strong predictive model to find out exactly how much these factors influence price.

Dataset Sources
Listings and Reviews: Inside Airbnb

Subway Data: MTA GTFS

Key Findings (The main answers)
Model

Average Prediction Error (MAE)

Explained Variance (R 
2
 )

Simple Model (Linear Regression)

$16.95

≈68%

Final Model (Random Forest)

12.50

≈81%

Result: My final model is, on average, only $12.50 off the actual price, which is a great result for NYC listings!

Top Price Drivers:

Property Type (e.g., Hotel vs. Apartment)

Guest Capacity (how many people fit)

Sentiment Score (how good the reviews are)

How to Run This Project (Instructions)
Download the project:

git clone [https://github.com/Barsha-bytes/Project-review-airbnb_subway.git](https://github.com/Barsha-bytes/Project-review-airbnb_subway.git)

Open the main notebook: Look in the notebooks/ folder for airbnb_subway.ipynb.

Visualizations
Once you save your plots (charts) and upload them to the visualizations/ folder, they will appear here!
