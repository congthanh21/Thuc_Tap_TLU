# Phân khúc khách hàng và cảnh báo rời bỏ cho doanh nghiệp bán lẻ trực tuyến

Đồ án thực tập – Khoa Công nghệ Thông tin, Trường Đại học Thăng Long.
Sinh viên: Đào Công Thành (A48653, TE3602) · GVHD: [Họ tên GVHD]

## Giới thiệu
Phân tích hành vi khách hàng bán lẻ trực tuyến để phân khúc và cảnh báo sớm nguy cơ rời bỏ, nhằm tối ưu chi phí chăm sóc.
Dữ liệu: [Online Retail II](https://archive.ics.uci.edu/dataset/502/online+retail+ii) (UCI, CC BY 4.0).

> Đang thực hiện. Hiện tại: Giai đoạn 1 – thiết lập cơ sở dữ liệu và EDA.

## Cấu trúc
- `data/`: nơi đặt dữ liệu gốc (không đưa lên GitHub)
- `notebooks/`: `01_eda.ipynb`
- `sql/`: script PostgreSQL
- `docs/`: cơ sở lý thuyết
- `requirements.txt`: thư viện cần cài

## Cách chạy (Giai đoạn 1)
```bash
git clone https://github.com/congthanh21/Thuc_Tap_TLU.git
cd Thuc_Tap_TLU
pip install -r requirements.txt
```
1. Tải `online_retail_II.csv` từ link ở trên, đặt vào `data/`.
2. PostgreSQL: tạo CSDL bằng pgAdmin 4, chạy phần đầu `sql/02_eda.sql` để tạo bảng staging, rồi import CSV.
3. Mở EDA: `jupyter lab notebooks/01_eda.ipynb` (đổi đường dẫn CSV thành `../data/online_retail_II.csv`).

## Tiến độ
- [x] Tuần 5–7: môi trường, bảng staging, EDA
- [ ] Tuần 8: làm sạch dữ liệu, mô hình sao
- [ ] Tuần 9: phân khúc RFM, định nghĩa churn
- [ ] Tuần 10: mô hình dự báo và baseline
- [ ] Tuần 11–12: Dashboard Power BI, danh sách 500 khách
- [ ] Tuần 13: đóng gói và hoàn thiện báo cáo
