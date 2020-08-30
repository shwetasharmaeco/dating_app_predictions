# I know too much!!

images: EDA graphs

dating.ipynb: exploratory data analysis

feature_selection.ipynb: data balancing, runs Logistic Regression, Random Forest Classifier and Gradient Forest Classifier models with all variables but text columns

nlp.ipynb: Reruns models using NLP technique on essay columns.

capstone_2_dating.pptx: Project's power point presentation.

## Motivation and Goal
Many users skip questions asking sensitive information. Project's goal is to predict if a user consumes drug or not from other questions answered by the user implementing machine learning techniques.

## Methods Used

Data Visualization

Natural Language Processing

Vectorization

Logistic Regression, Random Forest, Gradient Boosting

## Technologies
Python

pandas, numpy

Scipy

Scikit-learn

NLTK

matplotlib, seaborn

## Data Pipeline
Download the OKCupid dataset from reddit.

Select and clean relevant columns.

Split data and balance trained data.

Build up the model pipelines to train the model.

Choose the best performance model to apply to the OKCupid dataset, and predict if a user consumes drugs or not.

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
* Drugs column (target) had 3 classifications i.e. "Often", "Sometimes", "Never" and data was highly **imbalanced**. Thus, "Often" and "Sometimes" were clubbed, including users who consume drugs and recall was chosen as the most important metric to optimize.

![Image](/images/drug_perc.png)

## Data Cleaning and prepping

* Nans were treated as answered no by the user for smoking and drinking columns.
* answers under ethnicity, education and religion were put into wider buckets.
* "Space camp" or Nan in education column were treated as in college/university. 
* Nan in ethnicity and religion were put under "other" category.
* 10 essay columns were clubbed together, stop words were removed, each word reduced to its stem and tokenized before implementing NLP techniques (TF-IDF Vectorizer).
* Trained data was balanced by oversampling from minority class.

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

## Baseline Results

Accuracy: 0.691

Precision: 0.181

Recall: 0.203

F1 score: 0.191

## Final Results

Out of three models, Gradient Boosting gave best results including age, gender, bio, drinking and smoking habits of the users.

Accuracy: 0.770

Precision: 0.415

Recall: 0.715

F1 score: 0.525

Further, predictions were on users who did not answer the question on drug consumption.











