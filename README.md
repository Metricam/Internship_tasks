# :wave: Internship Tasks
This repository includes data and task description for the AI/ML Summer Internship program.

---

# Summer 2022 Cohort
Tasks per track:
- [Data Science and Time Series Forecasting](#TS)
- [NLP and Deep Learning](#NLP)
- [Image Processing and Computer Vision](#CV)
- [BI and Data analytics](#BI)

## :point_right: Data Science and Time Series Forecasting <a name="TS"></a>
Dataset: https://www.kaggle.com/datasets/utathya/future-volume-prediction

Description: this is a demand forecasting data for different agencies with different SKUs. The same data used in pytorch-forecasting TFT example.

Tasks:
1. Data is aggregated at monthly level. The task is to create a forecasting model that would forecast the demand for the next 3 months. How would you evaluate and compare your models?
2. Please list at least 3 models/methods that can be used for this task. Make sure that at least one of them is an ML method and at least one of them does not use any ML/DL. List their advantages and disadvantages.
3. Please select a method that you think best suits the problem and create a forecasting model. You are free to do feature engineering or add additional data.
Please explain how your method works.
4. Agency06 and Agency14 are new and they want to decide which SKUs to sell. Please recommend 3 SKUs for each of them and explain why. How would you approach this problem?
5. Assume one of the managers really wants to use an ML model. you are tasked with training that model. The model has 5 hyperparameters. How would you approach the problem?
6. One of the managers thinks that increasing the discount (decreasing Sales in price_sales_promotion.csv) would make the number of sales higher.
7. How would you approach solving this problem? Can you quantify the effect of changing the Sales by 1%?
8. Assume that it holds true. Should they decrease the price? By how much? Is there a problem with this, if yes do you have any suggestion to reformulate the initial problem of forecasting the volume of sales.
9. You have successfully created an ML model that has great performance. They have been using the model for 2 years. Then suddenly the model performance drops. What could have possibly resulted in this outcome. Could you have prevented it? If yes how. If not, what can you do now?


Submission: Please use Python for the project. Please create a jupyter notebook with your solutions. Use markdown to answer the questions and describe your code. Push your work to github. Make sure you have all the info for creating your working environment. Use this form to submit your work: https://forms.gle/wVAcjBgSWwcp7HyH9

**Deadline: 27/May/2022**

## :point_right: NLP and Deep Learning <a name="NLP"></a>
Dataset: https://www.kaggle.com/datasets/mewbius/ecommerce-products

Description: the dataset contains a small sample of labeled examples and a lot of unlabeled product information. You will have several tasks on this dataset with classification of product category based on description being the main task.

Tasks:
1. Cite 3 scientific papers that suggest approaches that can be used for the main task (aka classification of product categories using descriptions) of this problem. Present a very short summary of the key aspects of the papers (may be in bullet points).
2. Select productsfull.csv dataset. Use only description column to extract the color of the product whenever applicable. Compare your results with the colorname columns
3. Using the same dataset, extract a set of keywords describing each category. What methods did you use for keywords extraction? Explain.
4. Separate part of the productsclassified.csv dataset and keep it for evaluation purposes (let’s call the rest training data). Now, first, take again productsfull.csv that has no Classification column (aka no label). Use description column to pretrain a language model and then using training data build a product classification pipeline with zero-shot and few-shot approaches separately. Provide your model performance evaluation on the separated evaluation set.
5. Which approach provided better results? Zero-shot learning or few-shot learning? Why?
6. You have successfully created an ML model that has a great performance. They have been using the model for 2 years. Then suddenly the model performance drops. What could have possibly resulted in this outcome. Could you have prevented it? If yes how. If not, what can you do now?

Submission: Please use Python for the project. Please create a jupyter notebook with your solutions. Use markdown to answer the questions and describe your code. Push your work to github. Make sure you have all the info for creating your working environment. Use this form to submit your work: https://forms.gle/wVAcjBgSWwcp7HyH9

**Deadline: 27/May/2022**

## :point_right: Image Processing and Computer Vision <a name="CV"></a>
Image: [Image_for_CV_task_1.jpg](Image_for_CV_task_1.jpg)

Description: Consider the image above. The task is to be able to detect different shapes and calculate their area in the picture. 

Tasks:
Please create 3 different methods:
1. Find the objects by the color. The color should be input. Find all the objects that have the given color. Calculate their areas. Please explain your solution.
2. Find the objects by their geometric shape (that is rectangle, circle, triangle etc.). Find all the objects with the given shape and calculate their areas. Please explain your solution.
3. Create an unsupervised ML model that can find the area given a marker on a relatively brighter and homogeneous background. No need to filter for color or shape. Please explain your solution.
4. Please compare the three approaches. List their advantages and disadvantages. 
5. Assume you have a high resolution image (30000 x 30000 pixels). The image cannot be fully read into the memory of your machine. So you have to divide the image into grids and process the grids separately. Maximum size of the grid can be 3000x3000. Will your solutions work in that case? If not, how can you make them work? How would you approach the problem? How would you do the splitting/cutting into grids. Please go over all the three approaches and cover if they would work or not, and if not what can you do to make them work. 

Submission: Please use Python for the project. Please create a jupyter notebook with your solutions. Use markdown to answer the questions and describe your code. Push your work to github. Make sure you have all the info for creating your working environment. Use this form to submit your work: https://forms.gle/wVAcjBgSWwcp7HyH9

**Deadline: 27/May/2022**

## :point_right: BI and Data analytics <a name="BI"></a>
Dataset: `bigquery-public-data.crypto_ethereum` on Google BigQuery

Description: Please create an account in Google BigQuery if you don’t have one yet. The task is to calculate the several features/variables for each address on the publicly available dataset `bigquery-public-data.crypto_ethereum`:

Tasks:
Calculate the following features:
1. transactions sent
2. transactions recieved
3/ ETH sent
3. ETH recieved
4. Average monthly transactions sent
5. Average monthly transactions recieved
6. Average monthly ETH sent
7. Average monthly ETH recieved
8. Average time between transactions sent
9. Average time between transactions recieved
10. STD of time between transactions sent
11. STD of time between transactions recieved
12. Active months
13. ETH balance
14. After calculating the features, use different visualizations to try to find relationships between the features. You should be able to find/see distinct groups of addresses. Please use statistical tests to find groups or validate that the groups are indeed different. 

Notes:
- Please note. 1 WEI is equal to 10^-18 ETH. So you need to convert all the WEI into ETH.
- Please use the Python library called `google-cloud-bigquery` to access the DB and calculate the features.
- You can learn more about the dataset from here: `https://www.kaggle.com/datasets/bigquery/ethereum-blockchain/code?utm_medium=partner&utm_source=cloud&utm_campaign=big+data+blog+ethereum`


Submission: Please use Python for the project. Please create a jupyter notebook with your solutions. Use markdown to answer the questions and describe your code. Push your work to github. Make sure you have all the info for creating your working environment. Use this form to submit your work: https://forms.gle/wVAcjBgSWwcp7HyH9

**Deadline: 27/May/2022**

---
