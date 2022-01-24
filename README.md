# Starbucks Capstone Project
## Table of Contents
1. [Problem Statement](#pd) <br>
2. [Files](#an)<br>
3. [Results](#rs)<br>
4. [Required Packages](#bw)<br>
5. [Credits and Acknowledgements](#ca)<br>

<a name="pd"></a>
## 1. Problem Statement
A data set contains simulated data that mimics customer behaviour on the Starbucks rewards mobile app. Once every few days, Starbucks sends out an offer to users of its mobile app. An offer can be merely an advertisement for a drink or an actual offer such as a discount or BOGO (buy one get one free). Some users might not receive any offer during certain weeks. Not all users receive the same offer, and that is the challenge to solve with this data set.

The problem statement is to combine transaction, demographic and offer data to determine which demographic groups respond best to which offer type. 

<a name="an"></a>
## 2. Files

- Jupyter notebook that illustrate the analysis, comments, and rationale

- Input Files include:
  - portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.)
  - profile.json - demographic data for each customer
  - transcript.json - records for transactions, offers received, offers viewed, and offers completed
  

<a name="rs"></a>
## 3. Results
KMeans and HDBSCAN were used to build the cluster. Finally,  3 group of customers with differentiable characteristics were identified,

- `Cluster 0`: This cluster seems to be the largest cluster, including the younger to mid generations. But they have also spent lesser time using the app (i.e. they have only recently joined the rewards program when compared to Cluster 1)

- `Cluster 1`: This cluster consists of the older and wealthy customers. They also have been involved with the app the longest. However, this cluster seems to receive the lowest number of offers. This should be corrected as they are willing to spend and are loyal.

- `Cluster 2`: This cluster includes the customers who are receiving more offers than the other two clusters despite being low in number

- Based on this evaluation, Cluster 0 and 1 can receive more offers, in order to encourage Cluster 0 to be more active on the app and to give back to Cluster 1 for being loyal.
Cluster 2 are not really responding to offers although they are receiving a lot of offers.

<a name="bw"></a>
## 4. Required Packages
- Python 3+
- Machine Learning Libraries: NumPy, Pandas, SciKit Learn
- Data Visualization: Seaborn
- Training and Deployment: AWS Sagemaker

<a name="ca"></a>
## 5. Credits and Acknowledgements
- Udacity AWS Machine Learning Engineer Nanodegree Program
- Starbucks Datasets
- [Sklearn KMeans](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html)
- [Sklearn pre-processing](https://scikit-learn.org/stable/modules/preprocessing.html)
- [HDBSCAN](https://hdbscan.readthedocs.io/)
- [Sklearn PCA](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html?highlight=pca#sklearn.decomposition.PCA)



