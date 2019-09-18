### 0. Create SageMaker Jupyter Notebook
- Follow the instruction of below link's **Lab 0**
- https://s3.amazonaws.com/sagemaker-workshop/2018_04_southerndatascienceconference/Labs/index.html
  - Choose the region among N.Virginia, Ohio, Oregon, Singapore, Tokyo, Ireland
  - For the instance type, **choose ml.m5.xlarge**
  - When creating IAM role, **choose Any S3 bucket**

### 1. Built-in Linear Learner algorithm
- Follow the instoruction of **linear_time_series_forecast** example in introduction_to_applying_machine_learning folder
- Ref : https://github.com/awslabs/amazon-sagemaker-examples/blob/master/introduction_to_applying_machine_learning/linear_time_series_forecast/linear_time_series_forecast.ipynb

### 2. Amazon Forecast
- Open new Termial window at your Jupyter notebook
- Move to the SageMaker folder (/home/ec2-user/SageMaker/)
```bash
git clone https://github.com/aws-samples/amazon-forecast-samples.git
```
- Move to the notebook folder and follow the instruction of 1, 2, 3 ipynb.
  - Change the region 'us-west-2' to the region that you are working on

### 3. Time-series forecasting with DeepAR
- Follow the instoruction of **deepar_electricity example** in introduction_to_amazon_algorithms folder.
- Ref : https://github.com/awslabs/amazon-sagemaker-examples/blob/master/introduction_to_amazon_algorithms/deepar_electricity/DeepAR-Electricity.ipynb

### 4. Clear the resources
#### Amazon Forecast
- Delete resources within dataset group (datasets, predictors, forecasts)
- Delete the dataset group
#### SageMaker
- Delete SageMaker endpoints
- Delete SageMaker Notebook
- Delete S3 bucket
