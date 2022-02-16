# Phone Review Analysis and Summarization

## The objective is to 

1) Scrape data from different tech-blog.
2) Comparison and summarization of the product review from multiple websites.
3) Implementation of NLP algorithms to do sentiment analysis. Classification of web scraped data into positive and negative reviews.

## Detail
1) **Data scraping** Scrape the data from the following websites that contain reviews from popular tech-bloggers on various gadgets: Gizmodo (https://gizmodo.com), Engadget (https://www.engadget.com), Nextpit (https://www.nextpit.com), Gadgets.ndtv (https://gadgets.ndtv.com), Trustedreviews (https://www.trustedreviews.com), Gizbot (https://www.gizbot.com), TomsGuide (https://www.tomsguide.com), DigitalTrends (https://www.digitaltrends.com) and T3(https://www.t3.com).

2) **Exploratory data analysis and preprocessing**
    The data scraped contain different smartphones reviews from nine tech-blog mentioned above. Scraped data contained 3158 rows and four columns. Cleaned, transformed, structured, and formatted data from multiple data sources and stored it in a new single dataset REVIWE.csv. The final dataset we got has 1168 rows and five columns. Cleaned data consist of  As a part of preprocessing, removed unwanted data from review text, removed HTML tags, removed unwanted non-ascii character, newline, and tab. Decoded the encoded string, converted phone names to lower case for a better match and removed a few outliers review with a very low or very high word count. Phone reviews containing two or more reviews as we are summarizing reviews from at least more than two sites. After preprocessing got data of 295 unique phones.

3) **Summarization**
  
    * **Extractive Text Summarization**
      The extractive approach involves picking up the documents' most important phrases and lines. It then combines all the essential lines to create the summary. So, in this method,  every line, in summary, belongs to the original document, which is summarized.
    * **Abstractive Text Summarization**
      It is a more advanced method than extractive text summarization; many advancements keep coming out frequently—the abstractive approach based on deep learning. The process is to identify the important sections, interpret the context and reproduce in a new way. So, this method uses the term and new phrases, different from the original document, keeping the same points, just like how we summarize. The important thing is to note that note the sentences which are produced
here, in summary, are generated, not just extracted from the original text.

4) **Sentiment Analysis**
    * We have used VADER and Textblob for sentiment analysis.
    * Instead of analyzing all reviews at once, we are performing sentiment analysis of each sentence. Getting top positive and negative sentences from long reviews. Also checking if review is regarding some feature or compared with any competitor phone.
