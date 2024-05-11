
# Credit Risk Modeling Project

## Overview

This project aims to develop a robust credit risk modeling solution using big data analytics techniques. By leveraging advanced machine learning algorithms and large-scale data processing frameworks, we seek to improve the accuracy and efficiency of credit risk assessment for lending institutions leveraging
borrower data to predict default likelihood, enabling informed investment
decisions and riskmanagement..

## Table of Contents

1. [Background](https://chatgpt.com/c/0999a670-b29a-4107-b270-4acdca472de8#background)
2. [Dataset](https://chatgpt.com/c/0999a670-b29a-4107-b270-4acdca472de8#dataset)
3. [Technologies Used](https://chatgpt.com/c/0999a670-b29a-4107-b270-4acdca472de8#technologies-used)
4. [Project Structure](https://chatgpt.com/c/0999a670-b29a-4107-b270-4acdca472de8#project-structure)
5. [Usage](https://chatgpt.com/c/0999a670-b29a-4107-b270-4acdca472de8#usage)
6. [Results](https://chatgpt.com/c/0999a670-b29a-4107-b270-4acdca472de8#results)
7. [Future Improvements](https://chatgpt.com/c/0999a670-b29a-4107-b270-4acdca472de8#future-improvements)
8. [Contributing](https://chatgpt.com/c/0999a670-b29a-4107-b270-4acdca472de8#contributing)
9. [License](https://chatgpt.com/c/0999a670-b29a-4107-b270-4acdca472de8#license)

## Background

Assessing credit risk is crucial for financial institutions to make informed lending decisions. Traditional methods often rely on limited data sources and may not capture the complex relationships inherent in credit risk. In this project we will be doing credit risk modelling of peer to peer lending
Bondora systems, Credit risk modeling involves analyzing data to assess the
likelihood that a borrower will default on a loan or fail to meet their financial
obligations. Peer-to-peer lending platforms like Bondora facilitate lending directly
between individuals, bypassing traditional financial institutions. In the context of
Bondora's peer-to-peer lending system, credit risk modeling would likely involve
analyzing borrower data, such as credit scores, income, employment history, and
other relevant factors, to predict the likelihood of default for each borrower. This
helps investors on the platform make informed decisions about which loans to
fund and manage their risk exposure.

## Dataset

The dataset used in this project comprises anonymized historical loan data, including borrower information, loan terms, credit scores, and repayment outcomes. The dataset is obtained from [Bondora](https://www.bondora.com/en?noredirect=1) company a leading company in lending loans in europe, and it consists of 370000 records with 112 features.

## Technologies Used

* Apache Spark for distributed data processing
* Python for data preprocessing, modeling, and evaluation
* Scikit-learn and Spark MLlib for machine learning algorithms
* Pandas and PySpark for data manipulation
* Jupyter Notebook for interactive development and experimentation

## Project Structure

<pre><div class="dark bg-gray-950 rounded-md border-[0.5px] border-token-border-medium"><div class="flex items-center relative text-token-text-secondary bg-token-main-surface-secondary px-4 py-2 text-xs font-sans justify-between rounded-t-md"><span>bash</span><div class="flex items-center"><span class="" data-state="closed"><button class="flex gap-1 items-center"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24" class="icon-sm"><path fill="currentColor" fill-rule="evenodd" d="M7 5a3 3 0 0 1 3-3h9a3 3 0 0 1 3 3v9a3 3 0 0 1-3 3h-2v2a3 3 0 0 1-3 3H5a3 3 0 0 1-3-3v-9a3 3 0 0 1 3-3h2zm2 2h5a3 3 0 0 1 3 3v5h2a1 1 0 0 0 1-1V5a1 1 0 0 0-1-1h-9a1 1 0 0 0-1 1zM5 9a1 1 0 0 0-1 1v9a1 1 0 0 0 1 1h9a1 1 0 0 0 1-1v-9a1 1 0 0 0-1-1z" clip-rule="evenodd"></path></svg>Copy code</button></span></div></div><div class="overflow-y-auto p-4 text-left undefined" dir="ltr"><code class="!whitespace-pre hljs language-bash">├── dataset/
│   ├── LoanData.csv       # Raw dataset
│   └── processed_data    # Processed data
├── notebooks/
│   ├── 0_data loader.ipynb   			# Donwloading data notebook
│   ├── 1_preprocessing.ipynb      		# Preprocessing and first EDA notebook
│   ├── 2_EDA_And_FeatureEngineering.ipynb     	# Second EDA phase notebook
│   ├── 3_Assosiation.ipynb   			# Assosiation Rules notebook
│   ├── 4_modelling.ipynb      			# Model training (sklearn) notebook
│   ├── 5_BigData_algorithms.ipynb   		# Model Training (PySpark) notebook
│   ├── 6_KNN_mapReduce.ipynb      		# KNN MapReduce algorithm notebook
│   └── 7_kmeans.ipynb				# Clustering notebook
|
├── README.md           # Project README file
└── requirements.txt    # Python dependencies
</code></div></div></pre>

## Usage

1. Clone this repository.
2. Install the required dependencies using `pip install -r requirements.txt`.
3. Execute the Jupyter notebooks in the `notebooks/` directory sequentially to preprocess the data, train the model, and evaluate its performance.

## Results

The trained credit risk model achieves an accuracy of average  87%. Further details and insights are provided in the [results notebook](./notebooks/5_BigData_algorithms.ipynb).

All visualizations can be found in [preprocecssing](./notebooks/1_preprocessing.ipynb) and [EDA](./notebooks/2_EDA_And_FeatureEngineering.ipynb) notebooks

## Future Improvements

* Incorporate additional features such as economic indicators, transactional data, and alternative credit scoring methods.
* Explore deep learning approaches for capturing complex nonlinear relationships in the data.
* Deploy the model in a production environment for real-time credit risk assessment.
