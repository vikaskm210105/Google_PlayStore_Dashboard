# Google Play Store Dashboard Project

## Project Overview

This project analyzes Google Play Store applications by studying the relationship between app size and user ratings. The main objective was to create an interactive bubble chart that helps understand how app size, ratings, and installs are related.

## Datasets Used

* Play Store Data.csv
* User Reviews.csv

## Project Workflow

### Data Cleaning

* Loaded both datasets using Pandas.
* Removed duplicate applications.
* Converted Reviews, Rating, and Installs into numeric data types.
* Converted app sizes into megabytes (MB).
* Handled missing values and inconsistent data.

### Data Integration

* Calculated the average Sentiment Subjectivity for each app from the User Reviews dataset.
* Merged both datasets using the App column.

### Filters Applied

The dashboard displays only applications that satisfy the following conditions:

* Rating greater than 3.5
* Reviews greater than 500
* Installs greater than 50,000
* Sentiment Subjectivity greater than 0.5
* Categories restricted to:

  * Game
  * Beauty
  * Business
  * Comics
  * Communication
  * Dating
  * Entertainment
  * Social
  * Events
* Applications containing the letter "S" in their names were excluded.

### Category Customization

* Beauty was translated into Hindi: **सौंदर्य**
* Business was translated into Tamil: **வணிகம்**
* Dating was translated into German: **Partnersuche**
* The Game category was highlighted in pink.

## Visualization

An interactive Plotly Bubble Chart was created where:

* X-axis: App Size (MB)
* Y-axis: Average Rating
* Bubble Size: Number of Installs
* Bubble Color: Application Category

The chart supports interactive features such as hovering, zooming, and filtering through legends.

## Business Rule

As per the internship requirements, the bubble chart is configured to be displayed only between **5:00 PM IST and 7:00 PM IST**.

## Technologies Used

* Python
* Pandas
* Plotly
* Jupyter Notebook

## Conclusion

This project demonstrates the complete workflow of a small data analytics project, including data cleaning, transformation, integration, filtering, and interactive data visualization using Python.
