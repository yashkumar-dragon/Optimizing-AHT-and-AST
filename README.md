# Optimizing-AHT-and-AST
Project Overview
This project focuses on optimizing key metrics such as Average Handle Time (AHT) and Average Speed to Answer (AST) for United Airlines. The goal is to reduce call resolution times and improve customer satisfaction through data analysis, machine learning, and process automation recommendations.

Steps to Deploy This Project

1. Setup the Environment
Requirements
Ensure that you have the following software installed on your system:

Python 3.7 or higher
pip (Python package installer)

Install Required Packages
Navigate to the project directory and install the required Python libraries:

pip install -r requirements.txt

The requirements.txt file includes the following libraries:

pandas
numpy
scikit-learn
matplotlib
seaborn
nltk (for NLP tasks)
jupyter (for running notebooks)

2. Data Preparation
Datasets
Ensure that the following datasets are available in the same directory:

calls.csv: Main dataset containing call-related information.
customers.csv: Customer details including loyalty status.
reason.csv: List of primary call reasons.
sentiment_statistics.csv: Sentiment analysis data for each call.
test.csv: Test dataset for predicting the primary call reason.
You can either download the datasets from the provided resources or move them into the project folder.

4.Jupyter Notebooks

Navigate to the directory where the ipynb notebooks is available.

write "jupyter notebook" in cmd to access the ipnyb file

You can explore the Jupyter Notebooks provided for detailed step-by-step analysis which includes

	1. Data Cleaning and Merging
	clean and merge the datasets into a single file for analysis. It will handle missing values and prepare the data for further processing.

	2. Data Analysis and Visualization
	compute key statistics, including AHT, AST, sentiment distribution, and more:

	This will generate basic statistics such as:

	Overall AHT and AST
	Call distributions based on agent performance, customer sentiment, and call types
	Analysis of high-AHT call reasons

	3. Machine Learning Model Training
	Train a machine learning model to predict the primary_call_reason using the provided features (e.g., sentiment, agent tone, silence percentage):

	This script uses a Random Forest Classifier to predict the primary reason for a call and evaluates the model's accuracy.

	4. Predictions on Test Data
	Use the trained model to predict the primary call reason for the test dataset:

	This will generate a file in the format test_<your_name>.csv with the following columns:

	call_id: Unique identifier for each call.
	primary_call_reason: Predicted primary reason for each call.

	5. Natural Language Processing (NLP)
	Perform NLP tasks such as extracting key phrases from the call_transcript and clustering similar call reasons:

	python nlp_analysis.py
	This script applies TF-IDF and clustering techniques (like K-means) to group frequent call issues and determine the proportion of self-solvable issues.

	6. Generate Insights and Recommendations
	Produce insights on how agent tone, customer sentiment, and silence percentage impact call center performance:

	It will also suggest improvements to the IVR system based on identified call patterns.

Future Enhancements

Further improve the predictive model by exploring other algorithms (e.g., Logistic Regression, Gradient Boosting).
Automate the retraining and evaluation process to adapt to changing call center data.
Continuously monitor and enhance the IVR system based on evolving customer needs.

Conclusion
This project offers a comprehensive approach to improving call center operations by analyzing data, applying machine learning techniques, and providing actionable recommendations to reduce AHT and AST. The final deliverables include code files, a test prediction file, and a presentation summarizing the findings.

Author
Yash Kumar
