# Laptop_Price_Prediction_ML
# Project Title: Laptop Price Prediction for SmartTech Co.
# Project Overview:
    SmartTech Co. has partnered with our data science team to develop a robust machine learning model that predicts laptop prices accurately. As the market for laptops continues to expand with a myriad of brands and specifications, having a precise pricing model becomes crucial for both consumers and manufacturers.
# Client's Objectives:
## Accurate Pricing: 
    Develop a model that can accurately predict laptop prices based on various features, helping our clients stay competitive in the market.
## Market Positioning: 
    Understand how different features contribute to pricing, enabling SmartTech Co. to strategically position its laptops in the market.
## Brand Influence:
    Assess the impact of brand reputation on pricing, providing insights into brand perception and market demand.
# Project Phases:
## Data Understanding
   --  Company, TypeName, Inches, ScreenResolution, Cpu, Ram, Memory, Gpu, OpSys, Weight, and Price are provided columns.
   -- Understand what each column is informing.
   -- Decide the target/Dependent and Independent variables.
   -- The type of ML used depends on the target variable.
## Data Cleaning
   -- Remove the unnecessary columns, as your data contains 'Unnamed: 0’, and 'Unnamed: 0.1’.
   -- Empty rows are removed.
   -- Replaced the wrong values by checking every column and replacing them using the multivariate imputation technique.
   -- Checked the missing values.
   -- Duplicates are removed.
   -- Detecting and Handling the outliers are done using the Boxplot IQR method.
## Feature Extraction
   --  Extract meaningful features to enhance model performance.
   -- Consider creating new features that capture the essence of laptop pricing.
   -- To improve the performance of the model extracted features should be non-redundant and provide a strong relationship with the target variable.
## Exploratory Data Analysis(EDA)
   EDA (Exploratory Data Analysis) in machine learning is the process of examining and summarizing a dataset to uncover patterns, detect anomalies, and gain insights that inform model-building decisions.
## Data Wrangling 
   -- Based on the feature selection the columns remained are Company, typename, Ram, Price, PPI, cpu_brand, Clock_Speed_Category, SSD, Gpu_Brand, Op_Sys, and Weight_Category.
   -- Encoding: DummyEncoding for Company, TypeName, Cpu_Brand, Gpu_Brand, Op_Sys and Ordinalencoding for Clock_Speed_Category, Weight_Category.
   -- Feature scaling: Used StandarScaling for Ram, PPI, SSD.
   -- Feature transforming: Applied Log Transformation on price as it is right skewed. 
## Feature  Selection
 ### Filter Methods
      -- Evaluate the relationship between each feature and the target variable independently.
      -- Select features with a high correlation to the target but low correlation feature are removed.
## Model Development

 ![](https://github.com/BhavanaBalasa/-Laptop_Price_Prediction_ML/blob/main/DataSplit.png)
 
  -- Employed machine learning algorithms such as Linear Regression, Random Forest, and Gradient Boosting to predict laptop prices.
  -- Evaluated and choosed the model that aligns best with the project's objectives.

 ![](https://github.com/BhavanaBalasa/-Laptop_Price_Prediction_ML/blob/main/Models.png)
## Hyperparameter Tuning:
   Fine-tune the selected model to achieve optimal performance.
   
   ![](https://github.com/BhavanaBalasa/-Laptop_Price_Prediction_ML/blob/main/HPT.png)
## Deployment
   -- After building a machine learning (ML) model, the next step is to deploy and integrate it into real-world data to make it useful in practical applications.

  -- Pipeline: In machine learning, a Pipeline is a tool that helps streamline and automate the process of applying multiple steps (like preprocessing, feature engineering, and modeling) in a consistent and reproducible manner. It encapsulates the entire workflow into a single object, which can be used for training, validation, and prediction tasks.

  -- Joblib is a Python library used primarily for saving (serializing) and loading (deserializing) machine learning models 
## Real Example
###  Mean Absolute Error (MAE): 0.03

![](https://github.com/BhavanaBalasa/-Laptop_Price_Prediction_ML/blob/main/Amazon.png)

## Conclusion
   -- Company, typename, Ram, Price, PPI, cpu_brand, SSD, and Gpu_Brand are features that have the most significant impact on laptop prices.
   -- Predicting laptop prices for lesser-known brands can be challenging for an ML model with a lack of Training Data for Lesser-known brands.
   -- Missing, incomplete, or outdated data can affect model accuracy.
   -- Budget laptops may dominate the dataset, leading to the underrepresentation of high-end or niche models.
   -- Predicting the prices of newly released laptops not present in the training dataset is challenging because the model has no prior exposure to these configurations, features, or pricing strategies.






















