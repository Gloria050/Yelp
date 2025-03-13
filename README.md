# Yelp Data Analysis Project

![Yelp Logo](https://upload.wikimedia.org/wikipedia/commons/a/ad/Yelp_Logo.svg)

## Overview

This project analyzes the Yelp dataset to explore user behavior, business patterns, and social networks. Through data visualization, sentiment analysis, and network analysis, we extract valuable insights about how users interact with businesses and each other on the Yelp platform.

## Table of Contents

1. [Introduction](#introduction)
2. [Data Description](#data-description)
3. [Setup and Installation](#setup-and-installation)
4. [Analysis Perspectives](#analysis-perspectives)
   - [Business Types and Locations](#business-types-and-locations)
   - [User Reviews and Preferences](#user-reviews-and-preferences)
   - [Business Operations and Revenue](#business-operations-and-revenue)
   - [User Behaviors and Trends](#user-behaviors-and-trends)
   - [Market Competition and Trends](#market-competition-and-trends)
   - [Sentiment Analysis](#sentiment-analysis)
   - [Network & Community Detection](#network--community-detection)
5. [Challenges & Pain Points](#challenges--pain-points)
6. [Key Findings](#key-findings)
7. [Skills Developed](#skills-developed)

## Introduction

Yelp is an online platform that allows users to search for and browse information about businesses, including their address, phone number, hours of operation, and other details. It also enables users to view reviews and ratings of businesses written by other users, and to write and publish their own reviews and comments. Yelp's review system leverages the power of social networking, encouraging users to share their experiences and opinions about businesses, which helps other users to find better businesses.

## Data Description

The Yelp dataset is a collection of data related to businesses, reviews, users, and other interactions on the Yelp platform. The dataset includes information from several cities across the United States and Canada, covering a variety of business categories and user demographics.

This analysis utilizes several Yelp datasets:

1. **yelp_business.csv**: Contains business information (ID, name, address, location, rating, categories, city, etc.)
2. **yelp_business_attributes.csv**: Contains attributes of businesses (WiFi availability, parking, etc.)
3. **yelp_business_hours.csv**: Operating hours for businesses (opening and closing times for each day)
4. **yelp_checkin.csv**: Check-in data for businesses (time and date of check-ins)
5. **yelp_review.csv**: User reviews for businesses (user ID, business ID, rating, review text, date)
6. **yelp_tip.csv**: Short tips left by users about businesses (recommended dishes, suggestions)
7. **yelp_user.csv**: User information (ID, name, registration time, average rating, etc.)

# Yelp Data Analysis Project

![Yelp Logo](https://upload.wikimedia.org/wikipedia/commons/a/ad/Yelp_Logo.svg)

## Overview

This project analyzes the Yelp dataset to explore user behavior, business patterns, and social networks. Through data visualization, sentiment analysis, and network analysis, we extract valuable insights about how users interact with businesses and each other on the Yelp platform.

## Dataset

This analysis uses the Yelp Dataset Challenge data, consisting of six CSV files:
- `yelp_business.csv` - Business information including location, categories, and ratings
- `yelp_business_hours.csv` - Business operating hours
- `yelp_checkin.csv` - Customer check-in data
- `yelp_review.csv` - User reviews of businesses
- `yelp_tip.csv` - User tips (short reviews)
- `yelp_user.csv` - User information and friend connections

## Analysis Perspectives

### Business Types and Locations
Analysis of business distributions across different cities and regions.

### User Reviews and Preferences
Understanding user ratings, review patterns, and preferences.

### Business Operations
Analyzing business hours, check-in patterns, and operational insights.

### User Behavior Trends
Exploring how users interact with the platform and businesses.

### Sentiment Analysis
Natural language processing of reviews to understand customer sentiment.

### Network & Community Detection
Social network analysis of user connections and community structures.

## Key Findings

- Approximately 80% of users write only about 2 reviews on average
- Clear temporal patterns exist in check-in data, with weekends showing different patterns
- Elite users tend to write reviews with more neutral sentiment compared to regular users
- Las Vegas, Phoenix, and Toronto have the highest number of businesses and reviews
- Analysis of user networks reveals distinct community structures within geographic areas

## Project Structure

```
project1_yelp_data/
├── data/                     # Data directory (not tracked in git due to size)
│   ├── yelp_business.csv
│   ├── yelp_business_hours.csv
│   ├── yelp_checkin.csv
│   ├── yelp_review.csv
│   ├── yelp_tip.csv
│   └── yelp_user.csv
├── code/                     # Analysis code
│   ├── data_processing.py    # Data loading and cleaning functions
│   ├── visualization.py      # Visualization functions
│   ├── sentiment_analysis.py # Sentiment analysis of reviews
│   ├── network_analysis.py   # Network and community detection
│   └── main.py               # Main analysis pipeline
├── notebooks/                # Jupyter notebooks for exploration
│   ├── 01_data_exploration.ipynb
│   ├── 02_business_analysis.ipynb
│   ├── 03_user_analysis.ipynb
│   ├── 04_sentiment_analysis.ipynb
│   └── 05_network_analysis.ipynb
├── reports/                  # Analysis reports
│   └── yelp_analysis_report.pdf
└── README.md                 # Project documentation
```

## Setup and Installation

```bash
# Clone the repository
git clone https://github.com/username/project1_yelp_data.git
cd project1_yelp_data

# Create a virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install required packages
pip install -r requirements.txt
```

## Data Preparation

Due to the large size of the Yelp dataset, the data files are not included in this repository. To run the analysis:

1. Download the Yelp dataset from [Yelp Dataset Challenge](https://www.yelp.com/dataset)
2. Extract the CSV files and place them in the `data/` directory
3. Run the data processing scripts to prepare the data for analysis

## Running the Analysis

```bash
# Process the data and generate visualizations
python code/main.py

# Alternatively, explore the data through Jupyter notebooks
jupyter notebook notebooks/01_data_exploration.ipynb
```

## Contributors

- Primary Analyst: [Your Name]

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgements

- Yelp for providing the dataset through the Yelp Dataset Challenge
- All contributors to the open-source libraries used in this project


## Challenges & Pain Points

### Data Volume and Complexity
The Yelp dataset contains millions of rows of data, making it challenging to extract meaningful insights. We use sampling techniques to reduce dataset size while maintaining analysis integrity, though this may overlook important patterns visible only in the full dataset.

### Data Quality
The user-generated nature of the data means quality varies widely. We implement cleaning and preprocessing techniques to ensure accuracy and reliability, though this can be time-consuming and may require manual intervention.

### Bias
The dataset may be subject to bias and manipulation. We use statistical techniques to account for bias and adjust for confounding variables, though this may not fully address all sources of bias.

### Interpretation and Communication
We focus on effective data visualization and storytelling techniques to convey key insights in a compelling and accessible way, though this requires specialized skills in data visualization and communication.

## Key Findings

- Approximately 80% of users write only about 2 reviews on average
- Clear temporal patterns exist in check-in data, with weekends showing significantly different patterns compared to weekdays
- Elite users tend to write reviews with more neutral sentiment compared to regular users
- Community detection reveals distinct social groups within local geographic areas
- Business categories show significant variation in rating distributions
- Las Vegas, Phoenix, and Toronto have the highest number of businesses and reviews
- Review sentiment varies significantly by business category and location

## Skills Developed

### Data Analysis Skills
Cleaning, transforming, aggregating, and analyzing large-scale datasets, using various modeling and analysis methods including regression, classification, clustering, and time-series analysis.

### Business Analysis Skills
Analyzing data from platform, user, and merchant perspectives to understand the Yelp platform's operational status and provide actionable insights.

### Programming Skills
Using Python for data cleaning and analysis, SQL for data querying and aggregation, and R for statistical analysis and visualization.

### Visualization Skills
Creating effective visualizations using tools like Matplotlib, Seaborn, Plotly, and Folium to communicate findings to non-technical stakeholders.

### Teamwork Skills
Collaborating with team members to develop analysis plans, interpret results, and create compelling data narratives.

## Contributors

- Gloria

## License

This project is licensed under the MIT License - see the LICENSE file for details.

---

*Note: This analysis is for educational purposes only and uses publicly available Yelp datasets.*
