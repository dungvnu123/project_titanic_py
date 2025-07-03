🛳️ Titanic - Dự đoán hành khách sống sót bằng Machine Learning
📌 Mô tả dự án
Dự án này áp dụng các kỹ thuật tiền xử lý dữ liệu, trích xuất đặc trưng và mô hình hóa để dự đoán khả năng sống sót của hành khách trên con tàu Titanic, dựa trên tập dữ liệu từ cuộc thi nổi tiếng Titanic - Machine Learning from Disaster (Kaggle).
project_titanic_py/
│
├── train.csv                  # Dữ liệu huấn luyện
├── test.csv                   # Dữ liệu kiểm tra
├── gender_submission.csv      # File mẫu nộp Kaggle
├── thuc_hanh.ipynb            # Notebook xử lý & train mô hình
├── README.md                  # Giới thiệu dự án (file này)
🧠 Các bước thực hiện
Tiền xử lý dữ liệu

Xử lý giá trị thiếu (Age, Embarked)

Tạo cột mới: Family_size, Title

Encoding dữ liệu phân loại

Tạo pipeline tự động

SimpleImputer, StandardScaler, OneHotEncoder

ColumnTransformer cho dữ liệu số & phân loại

Huấn luyện mô hình

Logistic Regression (có thể mở rộng Random Forest, XGBoost, v.v.)

Train/test split để đánh giá độ chính xác

Đánh giá mô hình

Accuracy, classification report

Confusion matrix trực quan
5.Hoc may // hien tai dang dua ra mo hinh phu hop hon 
