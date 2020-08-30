# I know too much!!

# Motivation and Goal
Many users skip questions asking sensitive information. This project tries to predict if a user consumes drug or not from other questions answered by the user.


## Data
The data set consists of user profile data for 59,946 OkCupid users, including age, gender, income, education, religion, location, what kind of relationship, smoking and drinking habits. For some features, such as ethnicity, religion and offspring, users are allowed to pick multiple responses, making the data messy.

* A total of 48,442 users has their income listed as '-1' (maybe they do not wish to share this information on the internet).
* Many users wrote “space camp” for education.
* Most data (text) in 9 essays columns aka user BIO
* 12 body types
* 6 unique classes for drinks habits
* 33 unique classes for education
* 206 unique classes for ethnicity
* 46 unique classes for religion
* Drugs column (target) had 3 classifications i.e. "Often", "Sometimes", "Never" and data was highly imbalanced. Thus, "Often" and "Sometimes" were clubbed including users who consume drugs.

![Image](/images/drug_perc.png)





