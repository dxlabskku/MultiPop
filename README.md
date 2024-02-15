# MultiPop: Enhancing Instagram Engagement with Content-Based Multimodal Deep Learning in the Café and Bakery Sector
This repository is to supplement the paper "MultiPop: Enhancing Instagram Engagement with Content-Based Multimodal Deep Learning in the Café and Bakery Sector".


## Abstract
Social media has entrenched itself as an indispensable marketing tool. 
We introduce a quantitative approach to predicting the popularity of social media posts within the café and bakery sector. 
Employing a multimodal popularity prediction model that harnesses both images and text from post content, it utilizes the features of posts that significantly influence their popularity on one of the most widely Instagram. 
By focusing solely on post-content features and excluding user information, 
we analyzed 8,765 Instagram posts from the cafe and bakery domain, revealing that our model attains a superior accuracy rate of 82.0\% compared to existing popularity prediction methods. 
Furthermore, the study identifies hashtags and post captions as exerting a greater impact on post popularity than images. 
This research furnishes valuable insights, particularly for small business owners and individual entrepreneurs, 
by introducing novel computational and empirical methodologies for Instagram marketing strategy and post popularity prediction, thereby enhancing the comprehension of social media marketing dynamics.

## Overview of our framework
<img width="80%" src="https://github.com/dxlabskku/Instagram-Popularity/assets/97144805/971242d7-8f57-4eec-9896-f7570abaa3be"/>




## Dataset
This research built a new dataset To ensure the accuracy of popularity prediction and facilitate thorough post-analysis, data collection was meticulously conducted within a specific domain.
Focusing on the "café and bakery" domain, it specifically targets accounts of influencers specialized in reviewing cafés and bakeries.
Only Korean accounts were included in the study, and due to the domain's specificity, accounts of "nano influencers" and above were selected, all of whom have over 1,000 followers.

The posted dates of the collected data range from September 2016 to July 2023. 
The collected data encompassed various types of information, 
including the number of followers of each account, the first photo of each post, the content of each post, the date and time of each post, and the number of likes garnered by each post.
Following the initial collection of raw influencer posts, several steps were undertaken to further refine and process these posts.

The initial step in our data preprocessing involved stabilizing the number of likes by excluding the top 2.5\% and bottom 2.5\% of posts, totaling 5\%, 
based on the difference between the date the data was collected and the date the post was originally posted. 
This step aimed to eliminate the initial and most recent posts from the accounts. 
Second, to independently assess the influence of posts and hashtags, we extracted hashtags from the post captions, creating two distinct features: post captions without hashtags and their features. Any data lacking either of these features was removed.
Third, we conducted a text-cleaning process on the post-caption data. 

Following the preprocessing stage, the dataset underwent further refinement to ensure its suitability for analysis, resulting in a final dataset comprising 8,765 posts.
