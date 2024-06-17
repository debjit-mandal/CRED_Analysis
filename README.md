
# Crowd Reaction Estimation Dataset (CRED) Analysis

## Introduction
In the realm of social media, understanding and predicting post reach is a significant challenge. This project presents various analyses using the Crowd Reaction Estimation Dataset (CRED), which consists of pairs of tweets from The White House with comparative measures of retweet count. The analyses aim to provide insights into tweet engagement and factors affecting retweet counts.

## Dataset
The CRED dataset contains pairs of tweets with the following columns:

- **URL_x**: URL for the first tweet
- **Tweet_id_x**: Tweet ID of the first tweet
- **Datetime_x**: Timestamp when the first tweet was posted
- **cleaned_tweet_text_x**: Cleaned version of the first tweet
- **retweet_count_x**: Retweet count of the first tweet
- **claude_x_cleaned**: Response when Claude is prompted with the first tweet
- **chatgpt_x_cleaned**: Response when ChatGPT is prompted with the first tweet
- **flanul2_x**: Response when Flan-ul2 is prompted with the first tweet
- **URL_y**: URL for the second tweet
- **Tweet_id_y**: Tweet ID of the second tweet
- **Datetime_y**: Timestamp when the second tweet was posted
- **cleaned_tweet_text_y**: Cleaned version of the second tweet
- **retweet_count_y**: Retweet count of the second tweet
- **claude_y_cleaned**: Response when Claude is prompted with the second tweet
- **chatgpt_y_cleaned**: Response when ChatGPT is prompted with the second tweet
- **flanul2_y**: Response when Flan-ul2 is prompted with the second tweet
- **category**: Category of the tweets
- **retweet_count_x_more_y**: It is 1 if retweet count of the first tweet is more than the second. Else, it is 0.

## Analyses
The notebook includes the following analyses:

1. **Exploratory Data Analysis**: Visualizing the distribution of retweet counts for both tweets.
2. **Time-based Analysis**: Examining the relationship between the time of posting and retweet counts.
3. **Category-wise Analysis**: Analyzing retweet counts across different tweet categories.
4. **Sentiment Analysis**: Performing sentiment analysis on model responses (Claude, ChatGPT, Flan-ul2) and visualizing the sentiment distributions.
5. **Prediction Modeling**: Building a predictive model to estimate which tweet will receive more retweets using features such as timestamp and model responses.
6. **Feature Importance Analysis**: Identifying the most important features influencing the prediction of higher retweet counts.

## Installation
To run the notebook and analyses, you need to have Python installed along with the following libraries:

- numpy
- pandas
- matplotlib
- seaborn
- scikit-learn
- textblob

You can install the required libraries using the following command:

```bash
pip install -r requirements.txt
```

## Usage
Clone the repository:

```bash
git clone https://github.com/debjit-mandal/CRED_Analysis.git
cd CRED_Analysis
```

Ensure you have the dataset file CRED_without_tweets.xlsx in the project directory.

Run the Jupyter notebook:

```bash
jupyter notebook CRED_Analysis_Notebook.ipynb
```

Follow the instructions in the notebook to perform the analyses.

## Summary
In this notebook, various analyses are performed using the Crowd Reaction Estimation Dataset (CRED). The dataset consists of pairs of tweets from The White House with comparative measures of retweet counts. Our analyses included:

1. **Exploratory Data Analysis:** Visualized the distribution of retweet counts for both tweets.
2. **Time-based Analysis:** Examined the relationship between the time of posting and retweet counts.
3. **Category-wise Analysis:** Analyzed retweet counts across different tweet categories.
4. **Sentiment Analysis:** Performed sentiment analysis on model responses (Claude, ChatGPT, Flan-ul2) and visualized the sentiment distributions.
5. **Prediction Modeling:** Built a predictive model to estimate which tweet will receive more retweets using features such as timestamp and model responses.
6. **Feature Importance Analysis:** Identified the most important features influencing the prediction of higher retweet counts.

These analyses provided insights into tweet engagement and factors affecting retweet counts.

## Conclusion
These analyses revealed several interesting patterns and insights about tweet engagement:

- The distribution of retweet counts showed variability, indicating differences in tweet popularity.
- Time-based analysis suggested that the hour of the day might influence retweet counts.
- Category-wise analysis highlighted differences in engagement across various tweet categories.
- Sentiment analysis of model responses showed varying sentiment scores, which can impact tweet engagement.
- The predictive modeling approach demonstrated the potential to estimate tweet success using available features.

These findings can help digital marketers and content writers better understand and predict social media post reach, leading to more effective content strategies.

## License
This project is licensed under the MIT License.

## Acknowledgements
Special thanks to the creators of the CRED dataset (https://www.kaggle.com/datasets/sohomghosh/generator-guided-crowd-reaction-assessment/data) and the developers of the machine learning models used in this analysis.
