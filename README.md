Credit Card Fraud Detection with Random Forest
🎯 Mục tiêu: Dự đoán giao dịch thẻ tín dụng có phải là gian lận không, với Random Forest.
Dữ liệu có tỷ lệ gian lận cực thấp (~0.17%), gây khó khăn cho việc huấn luyện mô hình.
📁 Dataset
Nguồn: Kaggle - Credit Card Fraud Detection
284,807 dòng; 492 gian lận 

 Pipeline thực hiện (10 bước bài bản)
Khám phá dữ liệu (EDA)
Trực quan hóa dữ liệu
Tiền xử lý (Amount, Time)
Xử lý mất cân bằng (Undersampling, SMOTE, kết hợp)
Huấn luyện mô hình (Logistic, RF, XGBoost)
Trực quan kết quả (ROC, PR, confusion matrix)
Chọn mô hình tốt nhất theo PR-AUC
Tối ưu bằng GridSearchCV
Tối ưu threshold phân loại
