# class_16
### Bird's Eye View
***What makes machine learning so special?***
Machine learning is the practice of teaching computers how to learn patterns from data, often for making decisions or predictions.<br>
For true machine learning, the computer must be able to learn patterns that it's not explicitly programmed to identify.

***Key Terminology***

For this mini-course, we will focus on developing practical intuition instead of diving into technicalities (which we'll save for later).
* Model - a set of patterns learned from data.
* Algorithm - a specific ML process used to train a model.
* Training data - the dataset from which the algorithm learns the model.
* Test data - a new dataset for reliably evaluating model performance.
* Features - Variables (columns) in the dataset used to train the model.
* Target variable - A specific variable you're trying to predict.
* Observations - Data points (rows) in the dataset.

***Machine Learning Tasks***
The two most common categories of tasks are supervised learning and unsupervised learning. 
#### Supervised Learning
* In practice, it's often used as an advanced form of predictive modeling.
* Each observation must be labeled with a "correct answer."
* Only then can you build a predictive model because you must tell the algorithm what's "correct" while training it (hence, "supervising" it).
* Regression is the task for modeling continuous target variables.
* Classification is the task for modeling categorical (a.k.a. "class") target variables.

#### Unsupervised Learning
* In practice, it's often used either as a form of automated data analysis or automated signal extraction.
* Unlabeled data has no predetermined "correct answer."
* You'll allow the algorithm to directly learn patterns from the data (without "supervision").
* Clustering is the most common unsupervised learning task, and it's for finding groups within your data.

### Data Cleaning

***Better Data > Fancier Algorithms***

Data cleaning is one those things that everyone does but no one really talks about. Sure, it’s not the "sexiest" part of machine learning. And no, there aren’t hidden tricks and secrets to uncover

<br>***The first step to data cleaning is removing unwanted observations from your dataset.
This includes duplicate or irrelevant observations.***
Duplicate observations most frequently arise during data collection, such as when you:

Combine datasets from multiple places
Scrape data
Receive data from clients/other departments
<br>
Irrelevant observations are those that don’t actually fit the specific problem that you’re trying to solve.
