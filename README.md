# 🚨 Detection of Fraudulent Transactions

This project is a machine learning pipeline designed to detect fraudulent financial transactions using various classification algorithms. The dataset used includes details of transactions such as type, amount, and account balances.

## 📁 Dataset

The dataset used is `Fraud.csv`, which contains the following features:

- `step`: Unit of time (e.g., hourly step)
- `type`: Type of transaction (e.g., PAYMENT, TRANSFER)
- `amount`: Amount of the transaction
- `nameOrig`: Customer's name (anonymized)
- `oldbalanceOrg`: Initial balance before the transaction
- `newbalanceOrig`: Final balance after the transaction
- `nameDest`: Recipient's name (anonymized)
- `oldbalanceDest`: Initial recipient balance
- `newbalanceDest`: Final recipient balance
- `isFraud`: 1 if the transaction is fraudulent, else 0
- `isFlaggedFraud`: 1 if the transaction was flagged as fraud

## 📊 Technologies Used

- Python
- Pandas, NumPy
- Seaborn, Matplotlib
- Scikit-learn
- XGBoost
- Imbalanced-learn (SMOTE)

## 🧪 ML Pipeline

1. **Data Exploration**
   - Understand structure, check for missing values.

2. **Preprocessing**
   - Label Encoding for categorical features.
   - Dropping irrelevant columns.
   - Feature scaling using `StandardScaler`.

3. **Handling Imbalance**
   - Used SMOTE to balance the dataset.

4. **Model Building**
   - Logistic Regression
   - Decision Tree
   - Random Forest
   - Gradient Boosting
   - XGBoost

5. **Evaluation Metrics**
   - Accuracy
   - Classification Report
   - Confusion Matrix

## 🚀 How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/dorasambhrant/Detection-of-Fraud-Transaction.git
   cd Detection-of-Fraud-Transaction

	2.	Install dependencies:

pip install -r requirements.txt


	3.	Run the Jupyter notebook or use Google Colab.
	4.	Load dataset (Fraud.csv) and execute cells sequentially.

📈 Sample Output
	•	Visualizations of fraud vs non-fraud transactions
	•	Model performance comparison
	•	ROC curves and classification metrics

📌 Notes
	•	The dataset is highly imbalanced. Always use techniques like SMOTE or adjust class weights.
	•	For real-world applications, be cautious of false positives and false negatives.

👨‍💻 Author

Soham Dixit
