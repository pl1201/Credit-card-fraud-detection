Credit Card Fraud Detection with Random Forest
🎯 Mục tiêu

Dự đoán xem một giao dịch thẻ tín dụng có phải gian lận hay không bằng mô hình Random Forest.
Dữ liệu có tỷ lệ gian lận cực thấp (~0.17%), gây khó khăn cho việc huấn luyện mô hình → cần áp dụng kỹ thuật xử lý mất cân bằng.

📁 Dataset

Nguồn: Kaggle - Credit Card Fraud Detection

Số lượng: 284,807 dòng, trong đó 492 giao dịch gian lận

Đặc điểm:

- Dữ liệu đã được PCA ẩn danh (V1 → V28)

- Thêm 2 cột: Time và Amount

🔄 Pipeline xử lý

- Khám phá dữ liệu (EDA) – thống kê mô tả, phân phối dữ liệu

- Trực quan hóa dữ liệu 

- Tiền xử lý – scale Amount, chuẩn hóa Time

- Xử lý mất cân bằng: RandomUnderSampling, SMOTE, kết hợp cả 2

- Huấn luyện mô hình – Logistic Regression, Random Forest, XGBoost, Gradient Boosting

- Đánh giá mô hình – ROC, PR curve, confusion matrix

- Chọn mô hình tốt nhất – dựa trên PR-AUC

- Tối ưu tham số – dùng GridSearchCV

  Điều chỉnh threshold phân loại – cân bằng precision và recall
   . Trực quan hóa: matplotlib, seaborn
   . Machine Learning: scikit-learn
   . Mất cân bằng: imbalanced-learn (SMOTE, RandomUnderSampler)
   . Đánh giá: ROC-AUC, PR-AUC, F1, Recall, Confusion Matrix, Classification Report
