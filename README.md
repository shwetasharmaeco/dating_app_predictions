# I know too much!!

images: EDA graphs
dating.ipynb: exploratory data analysis
feature_selection.ipynb: data balancing, runs Logistic Regression, Random Forest Classifier and Gradient Forest Classifier models with all variables but text columns
nlp.ipynb: Reruns models using NLP technique on essay columns.
capstone_2_dating.pptx: Project's power point presentation.

# Motivation and Goal
Many users skip questions asking sensitive information. This project tries to predict if a user consumes drug or not from other questions answered by the user using machine learning techniques.


## Data
The data set consists of user profile data for 59,946 OkCupid users, including age, gender, income, education, religion, location, what kind of relationship, smoking and drinking habits. For some features, such as ethnicity, religion and offspring, users are allowed to pick multiple responses, making the data messy.

* A total of 48,442 users has their income listed as '-1' (maybe they do not wish to share this information on the internet).
* Many users wrote “space camp” for education.
* Most data (text) in 10 essays columns aka user BIO
* 12 body types
* 6 unique classes for drinks habits
* 33 unique classes for education
* 206 unique classes for ethnicity
* 46 unique classes for religion
* Drugs column (target) had 3 classifications i.e. "Often", "Sometimes", "Never" and data was highly **imbalanced**. Thus, "Often" and "Sometimes" were clubbed including users who consume drugs.

![Image](/images/drug_perc.png)

## Preview

**Distribution over gender**

![Image](/images/sex.png)

**Distribution over drinking categories**

![Image](/images/drinks.png)

**Joint distribution of drugs and drinks**

![Image](/images/drugs_drinks.png)

**Distribution over drug categories**

 0 being users who do not consume drug and 1 being users who consume drugs
 
![Image](/images/drugs_age.png)










