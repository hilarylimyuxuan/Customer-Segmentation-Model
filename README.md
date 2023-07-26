# wqd7003grp4
## Phase 1: Business Understanding
  1. Data Mining Goals<br />
  To build a customer segmentation model based on their behavioral data (spending, product usage etc.)

 
  2. Business Objectives<br />

* To increase customer retention and loyalty.<br />
* To fulfil customer's needs with recommendation system.<br />
* To boost up revenue and expand market shares.<br />

 3. Business Background<br />

* Founded in 2015, a Brazilian e-commerce platform<br />
* Olist works to connect small retailers to major e-commerce sites,     enabling the latter to increase their sales through large e-commerce platforms.<br />
* Olist's software and list their products in their software, which Olist will post to the major e-commerce sites for sale under its own name.<br />

 
  4. Situation Assessment<br />

* Business: Inadequate personalized recommendation system<br />
* Seller: Lesser profit as e-commerce platform takes higher percentage of profit sharing.<br />
* Customer:<br />
    - Logistic delivery timeliness problem<br />
    - Unattractive discounts<br />
    - Limited suppliers for certain types of product<br />
## Phase 2: Data Understanding
  1. Collect raw data: Fully understand the source of the data, determine the data carrier, data embodiment, and data storage location for these influencing factors.<br />
  2. Describe data: data description, preliminary understanding of data, simple description of data.<br />
  3. Explore data: Probe for data meaning.<br />
  4. Extract data: Analyze the information and knowledge hidden in the data.<br />

## Phase 3: Data Preparation
  1. Data preparation: dataset and dataset description.<br />
  2. Cleaning data: data cleaning, removing NA values from the dataset, dealing with missing values, dealing with outliers.<br />
  3. Constructing data: deriving attributes, data transformation.<br />
  4. Integrating data: merging data needed at a later stage.
## Phase 4: Modelling
  1. In this step, we use various techniques to segment the customer data into different groups based on patterns or similarities.<br />
  2. Initially, dimensionality reduction technique i.e., Principal Component Analysis (PCA) is used to reduce 57 selected features by selecting features with the most variance. Then, new combination of principal components scoring (scores_pca) dataset is formulated.<br />
  3. Then, we proceed to clustering algorithm technique i.e., K-Means clustering. Formulated PCA scores are then fitted with K-means. The method is then executed with a parameter specifying the number of clusters. The algorithm will then group the data points into the desired number of clusters, each having data points that are comparable to the previous cluster.<br />
  4. As a result, segmented cluster components dataset is formulated as the final models.<br />

## Phase 5: Evaluation
  1. In this section, the resulted models are further evaluated using Silhouette score, Calinski-Harabasz index, and Davies-Bouldin index.<br />
  2. Identify any patterns or trends in the data that can be used to target specific segments of customers.<br />
  3. Compare the segments to the overall population to identify any specific characteristics that set them apart.<br />
  4. For Silhouette score evaluation, between 2n to 5n clusters were compared for evaluation. As a result, 4n cluster appears to be the best as the thickness of the silhoutte plot is more uniform compared to others.<br />
  5. In addition, Davies-Bouldin index evaluation too exhibits a similar cluster pattern. It is observed that choosing 4 clusters minimizes the similarity measure. This is also supported with the higher Calinski-Harabasz index score indicating that the clusters are well separated and compact.<br />

## Phase 6: Deployment
  1. Use the segments to create targeted marketing campaigns for different groups of customers.<br />
  2. Use the segments to inform product development and inventory management decisions.<br />
  3. Monitor the success of the segmentation by tracking changes in customer behavior and sales revenue
