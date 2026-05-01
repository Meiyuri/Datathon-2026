# Datathon 2026

## 1. Cài đặt môi trường
- Ngôn ngữ: Python 3.8+
- Môi trường chạy: Google Colab 
- Các thư viện chính: pandas, numpy, os, matplotlib, seaborn, xgboost, lightgbm, catboost, shap
- Tableau Public 2026.1

## 2. Hướng dẫn chạy

### Phần 1: Trắc nghiệm
*   **File thực thi:** [`Phần_1_Trắc_nghiệm.ipynb`](Phần_1_Trắc_nghiệm.ipynb)
*   **Thao tác:** Chạy (Run All) toàn bộ Notebook. Code sẽ tự động tải dữ liệu, xử lý và in ra màn hình kết quả/lời giải chi tiết cho từng câu hỏi trắc nghiệm.

### Phần 2: Trực quan hóa và Phân tích Dữ liệu (EDA)
Phần này bao gồm 2 file để đối chiếu số liệu và hình ảnh biểu đồ:
*   **File code (Phân tích Insight 1 & 3):** [`Phần_2_EDA_(Phân tích bằng Colab).ipynb`](Phần_2_EDA_(Phân%20tích%20bằng%20Colab).ipynb). Chạy Notebook để xem quá trình xử lý, bóc tách dữ liệu rác và chứng minh các Lỗ hổng trong báo cáo doanh thu, Lỗ hổng R&D/Kiểm soát chất lượng bằng Python.
*   **File Dashboard Tableau (Phân tích Insight 2 & 3):** [`Phần 2 EDA - (Phân tích bằng tableau).twbx`](Phần%202%20EDA%20-%20(Phân%20tích%20bằng%20tableau).twbx). Mở file bằng phần mềm Tableau để xem các biểu đồ trực quan hóa đa chiều trong Lỗ hổng Kho vận/Nghịch lý chuỗi cung ứng (tồn kho, phân rã nguyên nhân hoàn trả....).

### Phần 3: Mô hình Dự báo Doanh thu (Sales Forecasting)
*   **File thực thi:** [`Phần_3_Mô_hình_Dự_báo_Doanh_thu_(Sales_Forecasting).ipynb`](Phần_3_Mô_hình_Dự_báo_Doanh_thu_(Sales_Forecasting).ipynb)
*   **Thao tác:** 
    1. Chạy toàn bộ Notebook. Quá trình này sẽ thực hiện Feature Engineering (tạo siêu đặc trưng thời vụ, sức mua, hiệu ứng chéo).
    2. Chờ hệ thống huấn luyện mô hình Hybrid Ensemble (kết hợp LightGBM, CatBoost, XGBoost).
    3. Trích xuất SHAP Values để giải thích các yếu tố tác động đến doanh thu.
*   **Kết quả đầu ra (Output):** File [`submission.csv`](submission.csv) chứa dự báo cuối cùng sẽ được tự động xuất và lưu tại thư mục làm việc hiện tại sau khi chạy xong.
