# israelpalestinenews
This project investigates how The New York Times (NYT) and The Guardian frame the Israel-Palestine conflict through their headlines.

# Abstract
This project investigates how The New York Times (NYT) and The Guardian frame the Israel-Palestine conflict through their headlines. While NYT is often perceived as pro-Israel, The Guardian takes a more left-leaning approach with a less explicitly defined stance. Through sentiment analysis, thematic clustering, and comparative language analysis, we examine differences in coverage, including the portrayal of key political figures, humanitarian crises, and military actions.

# Research Question 
How do headlines from The New York Times and The Guardian differ in their framing, sentiment, and coverage of the Israel-Palestine conflict since Oct. 7?

# Data Collection
We used APIs and documentation from NYT’s Developer Network and The Guardian’s Open Platform to collect our data. We searched for articles pertaining to Israel/Palestine from 10/01/2023 to 02/28/2025 by conducting searches with the following terms: “Israel”, “Palestine”, “Gaza”, “Palestinians”, “Hamas”, “IDF”. We saved our nearly 10,000 results in two DataFrames (one for each source) that contained the headline and its date/time of publication. We hoped to analyze a greater number of news sources, but found that very few provide APIs or allow for web scraping. 

# Data Exploration
We applied TF-IDF and 7-means clustering to our headlines data from each news source. For additional insight, we also created word clouds to showcase the most frequent terms in each cluster. While some clusters were similar across both sources (i.e. hostage negotiations; humanitarian aid), a number of differences were revealed as well. While NYT places a greater emphasis on U.S. foreign policy and military conflict, The Guardian highlights grassroot movements, Middle East regional conflicts, and calls for ceasefire.  

We applied VADER, a sentiment analysis tool designed for short texts such as headlines. For each headline, VADER provides a score (ranging from -1, extremely negative, to +1, extremely positive). We grouped headlines by week and news source and highlighted some of the many developments that may have impacted sentiment trends. 

We used VADER to analyze mentions of Biden and Netanyahu, noting a sharp decline in sentiment in The Guardian for both leaders in March 2024, likely due to Netanyahu’s Rafah attack plans and shifting perceptions of Biden’s culpability. These trends highlight media framing, and evolving discourse around their leadership.

# Conclusions
Our analysis shows that both outlets maintain a negative tone, with The Guardian scoring lower on average than NYT. While NYT focuses on U.S. political responses and diplomacy, The Guardian highlights protests, ceasefire demands, and humanitarian issues. The Guardian’s sharper negative sentiment, especially toward Netanyahu and Biden, aligns with key conflict developments and may stem from its use of more charged language. These findings underscore how editorial perspectives shape media narratives and public discourse, contributing to discussions on media bias and journalism’s role in international conflicts.

