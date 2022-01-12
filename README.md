# Echo-Chamber-in-Delhi-Election-2020

This is the research work carried out to study the Echo Chamber existing in Delhi Election 2020.


## Demonstration of Project:

https://user-images.githubusercontent.com/47279598/148943010-1be35edf-2d56-4631-b8e6-2ed35f50308a.mp4

### Link to download dataset : https://drive.google.com/drive/folders/18YEkbc8dL-AgoMKd0159KbsI7WBXHHCx?usp=sharing

## How to use?

1. Download the required files into a directory if your choice.
2. Open required codes in Jupyter Notebook.  
3. Install the dependencies as mentioned in code.
4. Execute the code.
5. Done

## Table of Contents: 

1. [Abstract](https://github.com/Piyush2912/Echo-Chamber-in-Delhi-Election-2020#1-abstract)
2. [Motivation](https://github.com/Piyush2912/Echo-Chamber-in-Delhi-Election-2020#2-motivation)
3. [Problem Statement](https://github.com/Piyush2912/Echo-Chamber-in-Delhi-Election-2020#3-problem-statement)
4. [Introduction](https://github.com/Piyush2912/Echo-Chamber-in-Delhi-Election-2020#4-introduction)
5. [Requirements](https://github.com/Piyush2912/Echo-Chamber-in-Delhi-Election-2020#5-requirements)
6. [Dataset Creation](https://github.com/Piyush2912/Echo-Chamber-in-Delhi-Election-2020#6-dataset-creation)
7. [Generic Methodology](https://github.com/Piyush2912/Echo-Chamber-in-Delhi-Election-2020#7-generic-methodology)
8. [Results](https://github.com/Piyush2912/Echo-Chamber-in-Delhi-Election-2020#8-results)
9. [Comparison with other model](https://github.com/Piyush2912/Echo-Chamber-in-Delhi-Election-2020#9-comparison-with-other-model)
10. [Summary and Conclusion](https://github.com/Piyush2912/Echo-Chamber-in-Delhi-Election-2020#10-summary-and-conclusion)
11. [Limitations](https://github.com/Piyush2912/Echo-Chamber-in-Delhi-Election-2020#11-limitations-challenges-faced-during-the-project)
12. [Future Scope](https://github.com/Piyush2912/Echo-Chamber-in-Delhi-Election-2020#12-future-scope)
13. [Credits](https://github.com/Piyush2912/Echo-Chamber-in-Delhi-Election-2020#13-credits)
14. [License](https://github.com/Piyush2912/Echo-Chamber-in-Delhi-Election-2020#14-license)

## 1. Abstract

- This project is concerned with the study of Echo chamber existing in Delhi Election 2020.
- There are three phrases of our project.
  - Training: Training model on the basis of three clustering algorithms.
  - Optimizing: Determining the best algorithm for analysis of results.
  - Analysis of Results on the basis of tolerance, influence and studying future trend of 30 days with RNN  
- Dataset consist of  1M tweets combined with 4 csvs for the four classes, BJP Support, BJP Against, AAP Support, AAP Against..
- K-Means clustering is used with TF-IDF Vectorizer with max-features as 200 and n-gram range as (1,2). 
- Our proposed model gives a result of AAP wining Delhi election in 2020.

## 2. Motivation

- The changing online environment - where the breadth of the information we are exposed to is algorithmically narrowed - has raised concerns about the creation of "echo chambers"; in which individuals are exposed mainly to information already in alignment with their preconceived ideas and opinions. 
- It has been said that Echo chambers are tricky to recognize, especially if you’re in one. 
- So it gets us to wondering if a social group or website may be an echo chamber. 
- Just before starting this project we asked a few questions from us regarding an Echo chamber.
  -	Do they tend to only give one perspective on an issue?
  -	Is that viewpoint mainly supported by rumour or incomplete evidence?
  -	Are facts ignored whenever they go against that viewpoint?
- To find the answers to these questions we moved ahead with our study.
- Secondly there was a lot of buzz around echo chambers being called a trap and it should be avoided.
- And several tips were suggested on avoiding them that we should make a habit of checking multiple news sources to ensure you’re getting complete, objective info, interacting with people of different perspectives. 
- So to find the answer to whether echo chambers are really dangerous we analysed echo chambers on Delhi CM elections held in 2020.

## 3. Problem Statement

- The goal is to predict whether the AAP or BJP will win election in year 2020 by social network analysis.
- Since this is an issue of unsupervised machine learning - clustering. 
- Algorithms have been narrowed down to three.
  - K-means clustering algorithm
  - DBSCAN (Density Based Spatial Clustering of Application with Noise) clustering algorithm
  - Meanshift clustering algorithm

<p align="center">
  <img src="https://user-images.githubusercontent.com/47279598/148946369-9dc7e92e-8a9a-4678-ab1c-e6b06b418b79.png"/>
</p>

<p align=center> 
  Figure 1: AAP (Aam Aadmi Party)
  Source: https://www.shutterstock.com/search/aap+icon
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/47279598/148944405-b4b677a2-df38-4406-8b1f-c6387f2f236d.png"/>
</p>
<p align=center> 
  Figure 2: BJP (Bharatiya Janata Party)
  Source: https://www.bjplogo.com/
</p>

## 4. Introduction

- An echo chamber is an environment where a person only encounters information or opinions that reflect and reinforce their own. 
- Echo chambers can create misinformation and distort a person’s perspective so they have difficulty considering opposing viewpoints and discussing complicated topics. Echo chambers can happen anywhere information is exchanged, whether it’s online or in real life. 
- But on the Internet, almost anyone can quickly find like-minded people and perspectives via social media and countless news sources.
- Echo chambers have emerged as an issue of concern in the political discourse of democratic countries. 
- There is growing concern that, as citizens become more polarised about political issues, they do not hear the arguments of the opposite side, but are rather surrounded by people and news sources who express only opinions they agree with. If echo chambers exist, then they might hamper the deliberative process in democracy.
- In this Research, we did social network analysis on twitter dataset and studied the degree to which echo chambers exist in political discourse on Twitter, and how they are structured. 
- We approach the study in terms of two components: the opinion that is shared by a user, and the “chamber”, i.e., the social network around the user, which allows the opinion to “echo” back to the user as it is also shared by others. 
- The opinion corresponds to content items shared by users, while the underlying social network is what allows their propagation. 
- We say that an echo chamber exists if the political leaning of the content that users receive from the network agrees with that of the content they share.

## 5. Requirements

All the experimental trials have been conducted on a laptop equipped by an Intel i7-8750H processor (4.1 GHz), 16 GB of RAM with 1050ti max-Q with 4 GB of VRAM. 
The Jupyter Notebook software equipped with Python 3.8 kernel was selected in this project for the development and implementation of the different experimental trails.

- Jupyter Notebook version 6.1 or above
- Python version 3.8 or above
- Python Libraries Used:
  - numpy https://numpy.org/doc/
  - pandas https://pandas.pydata.org/docs/
  - scikit-learn https://scikit-learn.org/stable/user_guide.html
  - keras https://keras.io/guides/
  - matplotlib https://matplotlib.org/stable/users/index.html
  - seaborn https://seaborn.pydata.org/tutorial.html

## 6. Dataset Creation

### Sources of Dataset Creation
- Kaggle : https://www.kaggle.com/nitinmaheshtiwari/2020-delhi-election-tweets-dataset

### Dataset Description

<p align="center">
  <img src="https://user-images.githubusercontent.com/47279598/148944460-d5e02326-9039-46bb-b945-55c04faefcd9.png"/>
  </p>
<p align=center> 
Figure 3: Snapshot of dataset
</p>

- Dataset contains tweets from 2020 Delhi Election time.
- Two major political parties covered are: Bharatiya Janata Party (BJP) and Aam Aadmi Party (AAP).
- This dataset contains user tweets along with the userID, date and time of creation and a sentiment score.
- Attributes of this dataset:
    - created_at : Time and Date of tweet creation.
    - tweet : Contains tweets from different users.
    - user_id : UserID of the user tweeting the Tweet.
    - sent : Contains sentiment score of every tweet i.e whether written in favour of the party or in against of the party.
- Dataset contains around 1M+ tweets for both the political parties.

## 7. Generic Methodology

<p align="center">
  <img src="https://user-images.githubusercontent.com/47279598/148944516-6f9c3235-56e7-42b5-8514-9707cc415e99.png"/>
  </p>
<p align=center> 
Figure 4: Data Pipeline
</p>

- The following figure 5 represents sequential steps performed in order to reach to end goal.
- firstly we preprocessed the data followed by making clusters in the dataset. 
- Then analysing tolerance level of people in each echo chamber and influencing power of each echo chamber.
- I used standard preprocessing methods for data preprocessing that includes stopwords and punctuation removal followed by removing tags and hyperlinks. 
- Finally, lemmatizing it using inbuilt POS tagger and lemmatizer in the NLTK library of python.
- After preprocessing has been done now our data is ready to be applied to the machine learning models.
- Second step was to identify clusters in this preprocessed dataset for which I used different clustering algorithms: these are DB-SCAN clustering algorithm, K Means clustering algorithm and Mean Shift clustering algorithm. 

## 8. Results

### Comparison between various clustering algorithms:

<p align="center">
  Table 1 : Comparison between various clustering algorithms
</p>
<p align="center">
  <img src="https://user-images.githubusercontent.com/47279598/148944571-97f144dd-4ab3-4a95-9ea3-966421110337.png"/>
  </p>

- After Going through the comparison Table 1 we choose K-means clustering as our primary clustering algorithm for further evaluation of Echo chambers. 
- We choose K-means clustering because we are getting higher silhouette score as higher the score clusters are denser, adjusted rand score as 1 which is a perfect match, lower davies bouldin score as lower the value better is the clustering performance, mutual info score is almost similar to other clustering algorithms, high Calinski harabasz score as higher the index better the performance. 
- We found that K means was actually performing well so we decided to carry on the remaining work with the results of K Means only.

### Analysis of Tolerance level of people

- The tolerance level of people indicates the upper limit of how many opposing thoughts and ideologies a person can tolerate.
- Based on the above definition, we categorized tolerance into 3 levels:
  - High Tolerance Level
  - Moderate Tolerance Level
  - Low Tolerance Level
- We calculated a Fluctuating Factor for each user as,

<p align="center">
  <img src="https://user-images.githubusercontent.com/47279598/148944665-9ba0f3ba-0e28-4a1b-b1ac-73b566aba37d.png"/>
  </p>
<p align="center">
Figure 5: Formula for Fluctuating Factor
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/47279598/148944709-453ba888-f90d-43dc-b41f-963bab6ddb8a.png"/>
  </p>
<p align="center">
 Figure 6: Formula of Tolerance  
</p>

### Results of Tolerance level of people

<p align="center">
  <img src="https://user-images.githubusercontent.com/47279598/148944833-5774a4d6-073e-4a9e-b9ac-dc67499337c1.png"/>
  </p>
<p align=center> 
Figure 7: Probability Density of people with each level of tolerance in support of BJP
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/47279598/148944915-3baf8577-936b-4b32-a5a6-ebbec98ba9aa.png"/>
  </p>
<p align=center> 
Figure 8: Probability Density of people with each level of tolerance in opposition of BJP
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/47279598/148944970-4cf55744-34ed-4faf-9fa4-4f4d54ece1b4.png"/>
  </p>
<p align=center> 
Figure 9: Probability Density of people with each level of tolerance in support of AAP
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/47279598/148945011-2b05c841-cd8d-4dc4-81cf-c853f3e69ea3.png"/>
  </p>
<p align=center> 
Figure 10: Probability Density of people with each level of tolerance in opposition of AAP
</p>

#### Now These are the results obtained after tolerance analysis. 

- The tolerance level of people indicates the upper limit of how many opposing thoughts and ideologies a person can tolerate. 
- Based on the above definition, we categorized tolerance into 3 levels:
  - High Tolerance Level
  - Moderate Tolerance Level
  - Low Tolerance Level

- We can see in the figure 7 first chart that the probability of people in support of bjp having high tolerance are less which means that with slight change in the opinions of the people who are in support of BJP they will likely change their echo chamber and can go to other three clusters and users with moderate tolerance are high so they have chances to either go in a different cluster or stay in their own. 
- Similarly we can see for users in support of AAP the probability of people in support of AAP having high tolerance are high which means that with slight change in the opinions they will not go to different chambers and only few users who are having low tolerance are likely to change their chamber. 
- Similar analysis can be done for the opposition of BJP and opposition of AAP chart and these results become valid as we know that AAP actually won those elections.  


## 9. Analysing the Influence power of Users in Echo Chamber

- Now the final part is analyzing the influence power of each user in the echo chamber.
- The influence of an echo chamber can be defined as its power to make other people agree with its opinions and ideologies.
- An echo chamber with high influencing power can attract new users to join as well as retain its existing users.  
- Based on previous data of each user, we tried to predict his future trend of tweets using RNN.
- We generated the data for 30 days using Simple RNN and based on that data, we calculated the number of people joining a particular echo chamber and the number of people leaving that echo chamber.
- For each echo chamber: for each day in 30 days : Plotting the value of (number of people joined -  number of people left) gives us the slope of the curve which is basically the Influence power of echo-chamber.
- Then we plotted data for each echo chamber to find the influence power.

### Results of Influence power of users in echo chamber

<p align="center">
  <img src="https://user-images.githubusercontent.com/47279598/148945095-457893cf-19ba-48d7-8190-9cbdd9fd79a8.png"/>
  </p>
<p align=center> 
Figure 11: Growth and Decline in number of people over a period of 30 days and corresponding Influence in support of BJP
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/47279598/148945151-5bccccac-fa5c-4210-83c4-d215797f9e2d.png"/>
  </p>
<p align=center> 
Figure 12: Growth and Decline in number of people over a period of 30 days and corresponding Influence in opposition of BJP
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/47279598/148945183-bb128da8-f160-4f83-bba5-92e1278df173.png"/>
  </p>
<p align=center> 
Figure 13: Growth and Decline in number of people over a period of 30 days and corresponding Influence in support of AAP
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/47279598/148945240-f0535d30-e28f-4a1f-af6e-b8757d6c932a.png"/>
  </p>
<p align=center> 
Figure 14: Growth and Decline in number of people over a period of 30 days and corresponding Influence in opposition of AAP
</p>

#### These are the results obtained after analysing influence. 

- We can see the Growth and Decline in the number of people over a period of 30 days and corresponding Influence in support of BJP, in opposition of BJP, in support of AAP, in opposition of AAP. 
- It can be seen in figure 12 that the influence of this eco-chamber over others is very high. 
- It can be assumed that it was successful in influencing people with low and moderate levels of tolerance from opposition of BJP and opposition of AAP eco-chambers. 
- It is clearly shown in figure 11 that over a period of 30 days, some people left this eco-chamber under the influence of other eco-chambers. 
- But their influence on other eco-chambers is quite high as clearly shown in Figure 12. 
- Those in opposition of bjp that in a period of 30 days, this eco-chamber has influenced a huge number of people to tweet against BJP. 
- In Figure 14 we can see that over the period of 30 days, the number of people leaving this eco-chamber are very high compared to people joining it, and this shows the poorest influencing power of this echo-chamber among the four.

## 10. Summary and Conclusion

- Tolerance level of people as well as Influence power of echo chambers both play a major role in election results.
- AAP support group has a high number  of highly tolerant people as well as high influencing power, resulting in a major victory in Delhi Election 2020.
- BJP had more people with moderate levels of tolerance hence it was more prone to lose its user base under the  influence of others.

## 11. Limitations/ Challenges faced during the project

- The dataset consisted of lot of noise which could hamper the results of our analysis so they were removed from datasets.
- Only these 3 algorithms were considered in this research because they have upper hand when dealing with textual data.
- Used standard preprocessing methods for data preprocessing that includes stopwords and punctuation removal followed by removing tags and hyperlinks. 
- lemmatizing it using inbuilt POS tagger and lemmatizer in the NLTK library of python. 

## 12. Future Scope

- The results shown in this study are just one step towards the understanding of echo chambers and the interplay between network and content, which open up several directions for future work. 

- First, exploring more social networking platforms like koo or reddit, which might lead to a better understanding of echo chambers in social media. 
  - To investigate new features to improve existing model.
  - For instance, n-gram features can turn out to be very informative for identifying good clusters, which indicates a distinctive writing style of the set of users. 
  - In this study we focused on content polarity clustering based techniques on a ground truth, but more powerful NLP techniques (e.g., topic modelling) might enable more powerful analysis. 
  - Second, Our findings show the effect of tolerance and influence on each user in an echo chamber but this could be extended by adding a new parameter of unfriending between them.
- To increase the size of dataset and make it more robust.

## 13. Credits: 

Thanking my project teammates for caring and supporting me wholeheartedly. The role you played in my life is invaluable. I’m grateful for all of your help and continued support.
<div class="align-text">
  <p>
   <p text-align= "justify"> Adarsh Kumar : https://www.linkedin.com/in/adarsh-kumar-5b1a1719b/  
  </p>   
   <p text-align= "justify"> Rohan Arora : https://www.linkedin.com/in/rohanarora18/  </p> 
  </p>
</div>

## 14. License: 

- Apache License 2.0
