# 🛳️ Titanic - Dự đoán hành khách sống sót bằng Machine Learning

## 📌 Mô tả dự án

Dự án này áp dụng các kỹ thuật tiền xử lý dữ liệu, trích xuất đặc trưng và mô hình học máy để **dự đoán khả năng sống sót của hành khách** trên con tàu Titanic, dựa trên tập dữ liệu từ cuộc thi nổi tiếng [Titanic - Machine Learning from Disaster (Kaggle)](https://www.kaggle.com/c/titanic).

---

## 📁 Cấu trúc thư mục


---

## 🧠 Các bước thực hiện

### 1. Xử lý dữ liệu

- Xử lý giá trị thiếu: `Age`, `Embarked`
- Tạo thêm đặc trưng mới: `Family_size`, `Title`
- Mã hóa các cột phân loại (Encoding)

### 2. Tạo pipeline tự động

- Dùng `SimpleImputer`, `StandardScaler` cho dữ liệu số
- Dùng `OneHotEncoder` cho dữ liệu phân loại
- Áp dụng `ColumnTransformer` để xử lý song song

### 3. Huấn luyện mô hình

- Dùng **Logistic Regression** làm mô hình chính
- Có thể mở rộng với: `Random Forest`, `XGBoost`, `SVM`, v.v.
- Tách dữ liệu thành `train` và `validation` để đánh giá

### 4. Đánh giá mô hình

- Accuracy score
- Classification Report
- Confusion Matrix trực quan (dùng seaborn)

---

## 📊 Kết quả hiện tại

| Mô hình              | Accuracy (val) | Ghi chú                  |
|----------------------|----------------|---------------------------|
| Logistic Regression  | xx%            | baseline                  |
| (Random Forest?)     | xx%            | chưa triển khai           |

> 📌 *Bạn có thể điền số liệu vào bảng trên sau khi chạy mô hình.*

---

## 🤖 Học máy phù hợp

Hiện tại mô hình **Logistic Regression** đang cho kết quả khá ổn định và dễ giải thích, phù hợp cho bài toán **phân loại nhị phân** như Titanic. Trong tương lai có thể thử thêm:

- Random Forest (đa chiều, ít overfit)
- Gradient Boosting / XGBoost
- VotingClassifier hoặc Stacking

---

## 🧪 Cách chạy dự án

```bash
git clone https://github.com/dungvnu123/project_titanic_py.git
cd project_titanic_py
jupyter notebook thuc_hanh.ipynb
