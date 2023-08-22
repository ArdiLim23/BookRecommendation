# BookRecommendation
## Complete process of book recommendation

This project included the following processes:
* Exploratory Data Analysis (EDA)
* Data Cleansing / Data Preparation
* Content-Based Filtering
  >The book "Author" will be the main feature. Besides that, **Term Frequency - Inverse Document Frequency (TF-IDF)** is used for the
  >feature extraction, and the algorithm to create recommendations uses **cosine similarity**
* Collaborative Filtering
  * Item-Based
    > Using a Compressed Sparse Row (CSR) Matrix based on the Rating for every book from UID data which is converted into a pivot table to
    > optimize the computation, then the CSR Matrix is fed into K-Nearest Neighbour with Cosine Similarity distance measurement 
  * Model-Based
    > Taking Book ID and User ID as the feature and rating as the label, a standard label encoding process is done for each book and user ID
    > feature. then the data is fed into the model which we can get from the Keras documentation, the model itself contains embedding layer
    > with each 50 embedding size used.

### This project is created with:
* Google Collab
* TensorFlow
* Keras
* Scikit-Learn
* Numpy
* Seaborn
* Pandas
