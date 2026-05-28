# California House Price Prediction

I built this project to predict house prices across California 
districts using census data. The goal was simple - given 
information about a neighborhood like income, location, and 
number of rooms, can we predict what houses there are worth?

## What I Did
- Explored the data to understand patterns and missing values
- Started with a simple Linear Regression as a baseline
- Tested 5 different models and compared them fairly using Cross Validation
- Tuned the best model to squeeze out better performance
- Built a prediction function you can use for any new house

## Results
Starting with Linear Regression gave an R² of 0.625.
After testing all models and tuning the best one 
(HistGradientBoosting), I got R² up to 0.826 — 
a 31% improvement over the baseline.

## What I Found Interesting
Out of all the features, median income of the neighborhood
turned out to be the strongest signal for house prices.
Location mattered too, but income drove the predictions more
than anything else.

## Tech Used
Python, Pandas, Scikit-learn, Matplotlib, Seaborn, Jupyter Notebook

## How to Run
pip install -r requirements.txt
jupyter notebook house_price_prediction.ipynb
