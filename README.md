# Phân khúc khách hàng và cảnh báo rời bỏ cho doanh nghiệp bán lẻ trực tuyến

Thực tập tốt nghiệp – Khoa Công nghệ Thông tin, Trường Đại học Thăng Long.
Sinh viên: Đào Công Thành (A48653, TE3602) · GVHD: Đinh Thị Thuý

## Giới thiệu
Phân tích hành vi khách hàng bán lẻ trực tuyến để phân khúc và cảnh báo sớm nguy cơ rời bỏ, nhằm tối ưu chi phí.

Dữ liệu: **Online Retail II** (Chen, 2019).
- Nguồn gốc: [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/502/online+retail+ii)
- Bản CSV dùng trong dự án: [Kaggle – Online Retail II UCI](https://www.kaggle.com/datasets/mashlyn/online-retail-ii-uci)

> Đang thực hiện. Hiện tại: Giai đoạn 1 – thiết lập cơ sở dữ liệu và EDA.

## Cấu trúc
- `data/`: nơi đặt dữ liệu gốc (không đưa lên GitHub)
- `notebooks/`: `01_eda.ipynb` (EDA), 02_clean_and_build_dw (làm sạch, mô hình sao), 03_rfm_segmentation (RFM, phân khúc), 04_churn_label_and_features (định nghĩa churn, đặc trưng), 05_model_training_evaluation (huấn luyện, đánh giá).
- `docs/`: cơ sở lý thuyết
- `requirements.txt`: thư viện cần cài

## Cách chạy 
Môi trường đã chạy: Python 3.12, PostgreSQL, pgAdmin 4.

```bash
git clone https://github.com/congthanh21/Thuc_Tap_TLU.git
cd Thuc_Tap_TLU
pip install -r requirements.txt
```
1. Tải `online_retail_II.csv` từ link Kaggle ở trên, đặt vào `data/`.
2. PostgreSQL: tạo CSDL bằng pgAdmin 4, Import tệp dữ liệu thô `online_retail_II.csv` vào bảng staging `staging_retail`.
4. Mở EDA: `jupyter lab notebooks/01_eda.ipynb`
5. Chạy tuần tự các file từ 02 đến trong thư mục notebooks/. Dữ liệu đầu ra của bước trước sẽ được lưu vào PostgreSQL để làm đầu vào cho bước sau.

## Tiến độ
- [x] Tuần 5–7: môi trường, bảng staging, EDA
- [x] Tuần 8: làm sạch dữ liệu, mô hình sao
- [x] Tuần 9: phân khúc RFM, định nghĩa churn
- [x] Tuần 10: mô hình dự báo và baseline
- [ ] Tuần 11–12: Dashboard Power BI, danh sách 500 khách
- [ ] Tuần 13: đóng gói và hoàn thiện báo cáo
