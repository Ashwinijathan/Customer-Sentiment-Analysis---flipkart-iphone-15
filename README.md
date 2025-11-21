# Customer-Sentiment-Analysis---flipkart-iphone-15
**Project Overview**

This project focuses on understanding customer sentiment toward the iPhone 15 (128GB) by analyzing user-generated reviews. Using web-scraped data, the reviews are cleaned, processed, and evaluated through sentiment analysis techniques to uncover how customers perceive various aspects of the product. This helps transform unstructured feedback into meaningful insights.

**Project Goal**

The goal is to determine whether customer sentiment is generally positive or negative and identify the key factors influencing these opinions. By uncovering recurring themes—such as performance, camera quality, battery life, and pricing—the project aims to support data-driven decisions, enhance customer experience, and highlight opportunities for product or marketing improvements.

**Objective:**
1. scrape atleast 300 reviews from Flipkart's product page for the iPhone 15 128GM model.
2. Clean and preprocess the scraped customer review data for accurate analysis.
3. Perform sentiment analysis to classify each review as positive or negative.
4. Analyze overall sentiment trends to identify actionable insights, review patterns.
5. Suggest product improvements and identify key marketing opportunities for the iPhone 15 (128GB) on Flipkart based on insights derived from customer sentiment analysis.

**Tasks involved:**
**1. Data Collection (Web Scraping):**

Tool: Selenium and BeautifulSoup

Task: Scrape at least 300 customer reviews from Flipkart's product page for the iPhone 15 128GB model. Each review should include:UserName,Ratings,Reviews,City

Steps:

 - Automate browser interactions, navigate to Flipkart’s product page for iPhone 15 128GB, and extract the reviews.
 - Use BeautifulSoup to parse the HTML of the reviews and extract the relevant details (username, rating, and review text).
 - Handle pagination to retrieve reviews from multiple pages.

**2. Data Cleaning and Preprocessing:**

Tool: Pandas

Task: Clean and preprocess the scraped data for analysis.

Steps:

- Eliminate duplicate reviews to ensure data quality.
- Address missing or incomplete data by removing rows or filling in missing values.
- Text preprocessing:
     - Convert the review text to lowercase.
     - Extracting irrelevant words such as "READ" from review text and "Certified" from city.
     - Capitalizing each word in UserName

**3. Sentiment Analysis:****

Tool: TextBlob

Task: Analyze the sentiment of each review to classify them as either positive or negative.

Steps:

 - Use TextBlob to perform sentiment analysis on the review text.
 - Based on polarity score between -1 (negative) and +1 (positive), will classify positive or negative sentiment
 - Threshold to classify the sentiment:
      Positive sentiment: Polarity score ≥ 0.1
      Negative sentiment: Polarity score < 0.1
 - Store the sentiment classification for each review in the dataset

**4. Data Analysis and Insights:**

Tool: Pandas and Matplotlib/Seaborn for visualization

Task: Perform an analysis on the sentiment of reviews and extract actionable insights.

Steps:

Sentiment Distribution: Calculate the overall distribution of positive and negative sentiments for the 300 reviews.
Average Rating vs Sentiment: Analyze if there is any correlation between the numeric ratings (1-5 stars) and sentiment polarity. 
Word Cloud: Create a word cloud to identify the most frequently mentioned words in the positive and negative reviews.
Review Length Analysis: Investigate if longer reviews are associated with more detailed sentiments, either positive or negative.

**5. Reporting:**

Summarize the findings in a clear, concise report with the following sections:

 - Overview of the data collection and cleaning process.
 - Sentiment Analysis Results: Distribution of positive/negative reviews, average sentiment per rating, etc.
 - Insights: Key trends from the sentiment analysis, such as common issues with the product or positive highlights.
 - Recommendations: Based on customer sentiment, suggest improvements for the iPhone 15 128GB model or potential areas Flipkart can focus on for marketing.
