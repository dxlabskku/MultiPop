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




## Dataset
This research constructed a new dataset to guarantee the accuracy of popularity predictions and conduct thorough post analysis within a specific domain. 
Focusing on the "café and bakery" domain, it exclusively targeted Korean influencer accounts that specialize in reviewing cafés and bakeries. 
The accounts selected were "nano influencers" or above, each boasting over 1,000 followers.

Data collection spanned approximately two months, from early July to the end of August 2023, 
incorporating 33 accounts into the process and resulting in the accumulation of metadata for each account and 12,563 posts. 
The collected data ranged in post dates from September 2016 to July 2023, including information such as the number of followers for each account, 
the first photo of each post, post content, the date and time of each post, and the number of likes each post received.

The data preprocessing phase involved stabilizing the number of likes by excluding the top 2.5% and bottom 2.5% of posts 
based on the difference between the data collection date and the original post date. This aimed to remove the initial and most recent posts from the accounts. 
Additionally, to independently assess the impact of posts and hashtags, hashtags were extracted from post captions, 
creating two separate features: post captions without hashtags and their features. Any data missing these features was eliminated. 
The third step was a text-cleaning process on the post-caption data, which included removing punctuation and numbers, 
using regular expressions to replace all characters except Korean and English with spaces, eliminating single Korean or English alphabet characters and multiple spaces, 
and converting English uppercase letters to lowercase to ensure text consistency.

After the preprocessing stage, the dataset was further refined to ensure its suitability for analysis, ultimately resulting in a final dataset comprising 8,765 posts.
