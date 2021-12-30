# Starbuck's Capstone Challenge
<br>

### Project Overview
This project is capstone project of Udacity Data Science Nanodegree program. The prime objective of this project is to combine transaction, demographic and offer data to determine which demographic groups respond best to which offer type. The data set is a simplified version of the real Starbucks app because the underlying simulator only has one product whereas Starbucks actually sells dozens of products.

### Data Sets

The data is contained in three files:

* portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.)
* profile.json - demographic data for each customer
* transcript.json - records for transactions, offers received, offers viewed, and offers completed

Here is the schema and explanation of each variable in the files:

**portfolio.json**
* id (string) - offer id
* offer_type (string) - type of offer ie BOGO, discount, informational
* difficulty (int) - minimum required spend to complete an offer
* reward (int) - reward given for completing an offer
* duration (int) - time for offer to be open, in days
* channels (list of strings)

**profile.json**
* age (int) - age of the customer 
* became_member_on (int) - date when customer created an app account
* gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
* id (str) - customer id
* income (float) - customer's income

**transcript.json**
* event (str) - record description (ie transaction, offer received, offer viewed, etc.)
* person (str) - customer id
* time (int) - time in hours since start of test. The data begins at time t=0
* value - (dict of strings) - either an offer id or transaction amount depending on the record

### File Structure:
```
- data
|- profile.json  # data to process 
|- portfolio.json  # data to process
|- transcript.json  # data to process

- fig
|- Average of Person Age Who Completed an Offer per Offer Type.jpg
|- Count of Completed Offers per Offer.jpg
|- Count of Gender per Year.jpg
|- Count of Incompleted Offers per Offer.jpg
|- Count of New User per Month.jpg
|- Count of Offer per Channel.jpg
|- Count of Offer per Type.jpg
|- Count of User per Gender.jpg
|- Duration Average of Offer per Type.jpg
|- Test Confusion Matrix of - DT.jpg
|- Test Confusion Matrix of - KNN.jpg
|- Test Confusion Matrix of - LR.jpg
|- Test Confusion Matrix of - RF.jpg
|- Test Confusion Matrix of - SVC.jpg
|- Top 10 Users of The Highest Collected Reward.jpg
|- Train_Test Accuracy.jpg
|- Histogram of Age.jpg
|- Histogram of Income.jpg
|- Relation between Age and Income.jpg
|- Relation between Reward and Difficulty.jpg
|- Sum of The Time Completed vs Incompleted Offers.jpg

- shutterstock.jpg
- pic1.png
- pic2.png
- README.md
- Starbucks_Capstone_notebook.ipynb

```
<br>

### Libraries Used:
- Pandas
- Numpy
- Matplotlib
- Itertools
- Seaborn
- sklearn

### Summary of The results of The analysis
- The number of clients in the app has been rapidly in 2016 and 2017
- The users who spend more time on the offer, are more likely to complete the offer.
- The most of new or old users are male and they are interactive with discount offers mainly while the female has the same attitude against discount and BOGO types.
- Email is the most effective channel to send offers.
- The discount offer is featured for a long duration compared to the other types.

### Medium Blog Post
The link of my Medium blog post is [https://mohammed-sadiq-alali.medium.com/starbucks-capstone-challenge-fd01b8d5abec](https://mohammed-sadiq-alali.medium.com/starbucks-capstone-challenge-fd01b8d5abec)

### Acknowledgements
This project was completed as part for Udacity Data Science Nanodegree program. Also, the data set contains simulated data that was provided by the Starbucks rewards mobile app.