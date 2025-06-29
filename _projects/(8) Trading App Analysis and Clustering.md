---
name: Trading App Analysis and Clustering
tools: [Analysis, Python, Clustering]
description: Cleaning, Analysis, and Clustering of Trading app data.
---

# Trading App Analysis and Clustering
The data are provided by Revou courses.
This project will try to answer these question. 
- What are the user trends of our investment app? checking the trend of our apps will help check the growth.
- How much money is moving in each type of investment and how often? this make sure to apply feature in a right way.
- What kind of investment behaviour our user have in each type? investment behaviour can be different between each user and usually it wil have its own group.
- Is certain type like occupation gende ror age group have certain distinct type? this question will help in deciding our segmentation group later.

Before proceeding with the analysis i cleaned the data first. Stuff that i fix are
*  change user id to str
*  remove user id duplicate for safe check
*  Change the datatype of date to datetime so its readable 
*  fill the NaN from refferal with "non Referral' for clarity
*  adding the age to age range for easier clustering in later use

For detail here are the notebook i made for data cleaning, EDA, and clustering.

<p class="text-center">
{% include elements/button.html link="https://colab.research.google.com/drive/1Y-JSEE26abaeU11CDtWKiFf4qkzLGq2G?usp=sharing" text="Google Colab Link" %}
</p>

Here are some the graph i produced.

![alt text](https://i.imgur.com/hFycNJk.png "Graph")
![alt text](https://i.imgur.com/mTPaf0G.png "Graph")

## Clustering
{% include elements/figure.html image="https://i.imgur.com/Fg0EMPr.jpeg" caption="The 3 Cluster" %}

- Cluster 0 are filled with youngster and someone with less than 10 m mincome, the majority are student. most of income from non work related (undian, orangtua, tabungan etc)
- Cluster 1 are mostly filled with high income person and with age above 20>, income source gome from bisnis or payday, this correlate with occupation that is swasta and pengusaha. almost  most are male
- cluster 2 are dominanly filled with woman with most of then are between 20-40, this cluster also filled with IRT occupation
