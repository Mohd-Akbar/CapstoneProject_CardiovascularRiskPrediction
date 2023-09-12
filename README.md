# CapstoneProject_CardiovascularRiskPrediction
In the Cardiovascular Risk Prediction project, a dataset comprising information on 3,390 individuals, encompassing 16 predictor variables, and a target variable. The goal was to predict the 10-year risk of developing coronary heart disease (CHD). Here's a concise summary of our workflow:

Data Preprocessing: Began by cleaning the data, handling missing values, and ensuring data types were appropriate for visualization.

Exploratory Data Analysis (EDA): Comprehensive EDA included univariate, bivariate, and multivariate analysis. This process provided valuable insights tha subsequent steps.

Feature Engineering: Created new features like pulse_pressure and glucose_diabetes, leveraging variables not directly linked to TenYearCHD. Addressing multicollinearity through VIF was also part of this stage.

Data Transformation: To achieve normal distribution, experimented with various transformation techniques and used quantile-quantile plots to assess data distribution. StandardScaler from sklearn was applied for data scaling.

Handling Imbalanced Data: Recognizing that the dataset was highly imbalanced, with only 15% of individuals having a high risk of CHD, we used SMOTE (Synthetic Minority Oversampling Technique) to balance the dataset.

Data Splitting: We divided the data into training and testing sets, ensuring a stratified representation of both classes.

Model Selection: We implemented multiple machine learning models, including Logistic Regression, Random Forest, XGBoost, Naive Bayes, KNN, and SVM.

Model Evaluation: The models were assessed using key metrics such as Precision, Recall, F1 Score, Accuracy, and AUC-ROC. Given the healthcare context, Recall (minimizing false negatives) was our primary focus, followed by F1 Score and Accuracy.

Hyperparameter Tuning: We fine-tuned the XGBoost model, achieving the highest performance with specific hyperparameters (learning rate, maximum tree depth, and the number of trees).

Final Model Selection: Based on comprehensive experimentation and comparisons, we chose XGBoost as the optimal model for deployment.

In summary, project involved rigorous data processing, feature engineering, and model evaluation. Despite challenges and occasional setbacks, we successfully developed a predictive model for identifying individuals at risk of developing CHD, with XGBoost emerging as the top-performing model. We focus on healthcare-specific metrics like Recall demonstrates a thoughtful approach to model selection.
