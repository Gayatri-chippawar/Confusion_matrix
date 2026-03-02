# 📊 Confusion Matrix & Classification Metrics
## 📌 Project Overview

This project builds a binary classification model to predict the presence of heart disease using Logistic Regression.

Model performance is evaluated using:

Confusion Matrix

Precision

Recall

F1-Score

The focus is on proper classification evaluation rather than relying only on accuracy.

## 📂 Dataset

Dataset: Heart Disease Dataset
Problem Type: Binary Classification

0 → No Heart Disease

1 → Heart Disease Present

The dataset contains medical attributes such as:

Age

Sex

Chest pain type

Resting blood pressure

Cholesterol

Maximum heart rate

Fasting blood sugar

etc.

## 🤖 Model Used
Logistic Regression

Logistic Regression is used because:

It works well for binary classification.

It provides probability-based predictions.

It is interpretable and efficient.

Mathematical form:

𝑃
(
𝑌
=
1
)
=
1
1
+
𝑒
−
(
𝛽
0
+
𝛽
1
𝑋
1
+
𝛽
2
𝑋
2
+
.
.
.
+
𝛽
𝑛
𝑋
𝑛
)
P(Y=1)=
1+e
−(β0+β1X1+β2X2+...+βnXn)
1
	​

## 📊 Confusion Matrix

For binary classification:

	Predicted 1	Predicted 0
Actual 1	TP	FN
Actual 0	FP	TN

Where:

TP → Correctly predicted heart disease

TN → Correctly predicted no disease

FP → Incorrectly predicted disease

FN → Missed disease case

📐 Evaluation Metrics
🔹 Precision
𝑃
𝑟
𝑒
𝑐
𝑖
𝑠
𝑖
𝑜
𝑛
=
𝑇
𝑃
𝑇
𝑃
+
𝐹
𝑃
Precision=
TP+FP
TP
	​


Indicates how many predicted disease cases were actually correct.

Important when false alarms must be minimized.

🔹 Recall
𝑅
𝑒
𝑐
𝑎
𝑙
𝑙
=
𝑇
𝑃
𝑇
𝑃
+
𝐹
𝑁
Recall=
TP+FN
TP
	​


Indicates how many actual disease cases were correctly detected.

Very important in medical diagnosis (missing a patient is risky).

🔹 F1 Score
𝐹
1
=
2
×
𝑃
𝑟
𝑒
𝑐
𝑖
𝑠
𝑖
𝑜
𝑛
×
𝑅
𝑒
𝑐
𝑎
𝑙
𝑙
𝑃
𝑟
𝑒
𝑐
𝑖
𝑠
𝑖
𝑜
𝑛
+
𝑅
𝑒
𝑐
𝑎
𝑙
𝑙
F1=2×
Precision+Recall
Precision×Recall
	​


Balances Precision and Recall.

Useful when dataset may not be perfectly balanced.

⚙️ Workflow

Data preprocessing

Checked missing values

Feature scaling

Train-test split

Trained Logistic Regression model

Generated predictions

Built Confusion Matrix

Calculated Precision, Recall, F1-score

## 🎯 Why These Metrics Matter in Heart Disease Prediction

In medical datasets:

False Negative (FN) is dangerous → patient has disease but model predicts no disease.

Therefore, Recall is critical.

F1-score ensures balanced evaluation.

## 📈 Key Learnings

Implemented confusion matrix from scratch

Understood TP, TN, FP, FN deeply

Learned why accuracy alone is not sufficient

Gained practical experience in medical dataset evaluatio
