# Phân khúc khách hàng và cảnh báo rời bỏ cho doanh nghiệp bán lẻ trực tuyến

Thực tập tốt nghiệp – Khoa Công nghệ Thông tin, Trường Đại học Thăng Long.
Sinh viên: Đào Công Thành (A48653, TE3602) · GVHD: Đinh Thị Thuý

## Giới thiệu
Phân tích hành vi khách hàng bán lẻ trực tuyến để phân khúc và cảnh báo sớm nguy cơ rời bỏ, nhằm tối ưu chi phí.
Dữ liệu: Online Retail II (Chen, 2019)
Nguồn gốc: UCI Machine Learning Repository
Bản CSV dùng trong dự án: Kaggle – Online Retail II UCI

Đang thực hiện. Hiện tại: Giai đoạn 1 – thiết lập cơ sở dữ liệu và EDA.

## Cấu trúc
- data/: nơi đặt dữ liệu gốc 
- notebooks/: 01_eda.ipynb
- docs/: cơ sở lý thuyết
- requirements.txt: thư viện cần cài

## Cách chạy (Giai đoạn 1)

git clone https://github.com/congthanh21/Thuc_Tap_TLU.git
cd Thuc_Tap_TLU
pip install -r requirements.txt
Tải online_retail_II.csv từ link ở trên, đặt vào data/.
PostgreSQL: tạo CSDL bằng pgAdmin 4, Import tệp dữ liệu thô online_retail_II.csv vào bảng staging.
Mở EDA: jupyter lab notebooks/01_eda.ipynb.
## Tiến độ
- [x] Tuần 5–7: môi trường, bảng staging, EDA
- [ ] Tuần 8: làm sạch dữ liệu, mô hình sao
- [ ] Tuần 9: phân khúc RFM, định nghĩa churn
- [ ] Tuần 10: mô hình dự báo và baseline
- [ ] Tuần 11–12: Dashboard Power BI, danh sách 500 khách
- [ ] Tuần 13: đóng gói và hoàn thiện báo cáo
xem phù hợp chưa chỉnh lại giúp mình
