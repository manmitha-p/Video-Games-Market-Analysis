# Video Games Market Analysis Project

## Overview
This project, conducted by Group Husky 2, involves a comprehensive analysis of the video game industry using extensive datasets to understand sales trends, genre popularity, and regional market preferences. The project utilizes various AWS services for data storage, processing, predictive modeling, and visualization.

## Datasets
- `game_sales_data.csv`
- `vgsales.csv`

These datasets provide detailed information on game titles, platforms, release years, genres, and sales figures across different regions.

## Project Workflow

### 1. Data Cleaning
- **Duplicate Removal**: Identified and removed duplicate entries to ensure data integrity.
- **Handling Missing Values**: Imputed or removed missing values to maintain dataset quality.
- **Data Type Conversion**: Converted sales figures to numeric types and adjusted release years to date formats.
- **Merging Datasets**: Integrated the datasets to provide a unified view of the market.

### 2. AWS Services Utilized
- **Amazon S3**: For scalable and secure data storage.
- **AWS IAM**: For managing permissions and securing data access.
- **AWS Glue**: For data cataloging, cleaning, and transformation.
- **Amazon SageMaker**: For building, training, and deploying predictive models.
- **AWS QuickSight**: For interactive data visualization and dashboard creation.

### 3. Analysis and Insights
- **Popular Genres**: Identified the most successful genres worldwide.
- **Critic Scores**: Analyzed the impact of critical acclaim on sales.
- **Genre Performance**: Examined genre success across different platforms and over time.
- **Regional Preferences**: Compared genre popularity in different geographic regions.
- **Top Performing Games**: Highlighted standout titles within each genre.

### 4. Predictive Modeling
- **Data Preprocessing**: Imputed missing values, one-hot encoded categorical variables, and standardized numerical features.
- **Model Architecture**: Developed a neural network with input, hidden, and output layers for regression.
- **Model Training and Evaluation**: Trained the model on the dataset and evaluated performance using mean squared error (MSE).

### 5. Visualization
- Created a comprehensive QuickSight dashboard summarizing key metrics and trends, making the insights accessible and actionable.

## Steps to Reproduce

### Prerequisites
- AWS Account
- Datasets (`game_sales_data.csv`, `vgsales.csv`)
- AWS CLI and SDKs installed

### Instructions

1. **Create an S3 Bucket**
   - Log into the AWS Management Console.
   - Navigate to S3 and create a new bucket for data storage.
   - Upload `game_sales_data.csv` and `vgsales.csv` to the bucket.

2. **Set Up AWS Glue**
   - Create a new crawler in AWS Glue pointing to the S3 bucket.
   - Run the crawler to populate the Glue Data Catalog with the dataset schemas.

3. **Query Data with AWS Athena**
   - Navigate to AWS Athena in the AWS Management Console.
   - Set Athena to use the Glue Data Catalog.
   - Execute SQL queries to analyze video game sales trends and other insights.

4. **Build Predictive Model with SageMaker**
   - Preprocess data: handle missing values, one-hot encode categorical variables, and standardize numerical features.
   - Develop a neural network model and train it on the dataset.
   - Evaluate the model's performance and use it for sales predictions.

5. **Create Visualizations with QuickSight**
   - Connect QuickSight to the data stored in S3 and Glue.
   - Build interactive dashboards to visualize key insights and trends.

## Conclusion
This project demonstrates the power of AWS cloud analytics tools in handling large-scale data analysis, predictive modeling, and visualization. By utilizing these tools, we gained valuable insights into the video game industry's market dynamics, informing strategic decisions and enhancing operational efficiency.
