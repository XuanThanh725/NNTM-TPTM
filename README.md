<h2 align="center">
    <a href="https://dainam.edu.vn/vi/khoa-cong-nghe-thong-tin">
    🎓 Faculty of Information Technology (DaiNam University)
    </a>
</h2>

<h2 align="center">
    🐄 HỆ THỐNG NHẬN DIỆN & PHÂN LOẠI VẬT NUÔI BẰNG YOLOv8
</h2>

<div align="center">
    <p align="center">
        <img alt="AIoTLab Logo" width="170" src="https://github.com/user-attachments/assets/711a2cd8-7eb4-4dae-9d90-12c0a0a208a2" />
        <img alt="AIoTLab Logo" width="180" src="https://github.com/user-attachments/assets/dc2ef2b8-9a70-4cfa-9b4b-f6c2f25f1660" />
        <img alt="DaiNam University Logo" width="200" src="https://github.com/user-attachments/assets/77fe0fd1-2e55-4032-be3c-b1a705a1b574" />
    </p>

[![YOLOv8](https://img.shields.io/badge/YOLOv8-Object%20Detection-green?style=for-the-badge)]
[![OpenCV](https://img.shields.io/badge/OpenCV-Computer%20Vision-blue?style=for-the-badge)]
[![Streamlit](https://img.shields.io/badge/Streamlit-Web%20Dashboard-red?style=for-the-badge)]

</div>

---

# 📖 1. Giới thiệu hệ thống

Hệ thống nhận diện và phân loại vật nuôi là ứng dụng sử dụng trí tuệ nhân tạo (AI) kết hợp mô hình YOLOv8 để phát hiện, nhận diện và thống kê các loại vật nuôi từ hình ảnh, video hoặc camera thời gian thực.

Hệ thống hỗ trợ:

- Nhận diện vật nuôi theo thời gian thực.
- Phân loại nhiều loài vật nuôi khác nhau.
- Đếm số lượng từng loại vật nuôi.
- Chụp ảnh tự động khi phát hiện vật nuôi.
- Lưu lịch sử nhận diện vào CSV.
- Xuất báo cáo thống kê.
- Hỗ trợ Webcam, Camera IP và ESP32-CAM.
- Dashboard trực quan với biểu đồ thống kê.

---

# 🔧 2. Công nghệ sử dụng

## 🤖 YOLOv8
- Phát hiện đối tượng thời gian thực.
- Nhận diện vật nuôi với độ chính xác cao.
- Hiển thị Bounding Box và độ tin cậy.

## 👁 OpenCV
- Xử lý ảnh và video.
- Kết nối Webcam, Camera IP và ESP32-CAM.
- Chụp ảnh tự động.

## 🌐 Streamlit
- Xây dựng Dashboard Web.
- Hiển thị biểu đồ và thống kê.
- Quản lý dữ liệu nhận diện.

## 💾 Pandas + CSV
- Lưu lịch sử nhận diện.
- Xuất báo cáo thống kê.
- Quản lý dữ liệu vật nuôi.

## 📷 Camera
- Webcam Laptop.
- Camera điện thoại IP Webcam.
- ESP32-CAM.

---

# 🚀 3. Chức năng chính

## 📷 Nhận diện qua Camera

- Nhận diện vật nuôi thời gian thực.
- Hiển thị Bounding Box.
- Hiển thị độ tin cậy.
- Tự động chụp ảnh khi phát hiện.
- Tự động lưu CSV.
- Thống kê số lượng vật nuôi.

## 🖼 Nhận diện qua Ảnh

- Upload ảnh.
- Phân tích ảnh.
- Hiển thị kết quả trực tiếp.
- Lưu ảnh kết quả.
- Xuất dữ liệu CSV.

## 🎥 Nhận diện qua Video

- Upload video.
- Phân tích từng frame.
- Tạm dừng / Tiếp tục.
- Thanh tiến trình xử lý.
- Chụp ảnh khi phát hiện vật nuôi.
- Thống kê số lượng từng loại.
- Xuất CSV sau khi hoàn thành.

## 📊 Dashboard

- Tổng số vật nuôi.
- Thống kê theo từng loại.
- Biểu đồ cột.
- Biểu đồ tròn.
- Bảng dữ liệu chi tiết.
- Cảnh báo khi số lượng vượt ngưỡng.

## 💾 Quản lý dữ liệu

- Lưu ảnh kết quả.
- Lưu CSV.
- Xem lịch sử nhận diện.
- Tải dữ liệu Excel.
- Tải dữ liệu CSV.

---

# 📸 4. Hình ảnh chức năng

<p align="center">
  <img src="docs/home.png" width="900"/>
</p>

<p align="center">
  <em>Hình 1: Giao diện trang chủ</em>
</p>

<p align="center">
  <img src="docs/camera.png" width="900"/>
</p>

<p align="center">
  <em>Hình 2: Nhận diện qua Camera</em>
</p>

<p align="center">
  <img src="docs/image.png" width="900"/>
</p>

<p align="center">
  <em>Hình 3: Nhận diện qua Ảnh</em>
</p>

<p align="center">
  <img src="docs/video.png" width="900"/>
</p>

<p align="center">
  <em>Hình 4: Nhận diện qua Video</em>
</p>

<p align="center">
  <img src="docs/dashboard.png" width="900"/>
</p>

<p align="center">
  <em>Hình 5: Dashboard thống kê</em>
</p>

<p align="center">
  <img src="SODO.png" width="1000"/>
</p>

<p align="center">
  <em>Hình 6: Sơ đồ kiến trúc hệ thống nhận diện và phân loại vật nuôi</em>
</p>

---

# 📂 5. Cấu trúc dự án

```text
AnimalDetection/
│
├── app.py
├── requirements.txt
├── yolov8s.pt
│
├── docs/
│   ├── home.png
│   ├── camera.png
│   ├── image.png
│   ├── video.png
│   ├── dashboard.png
│   └── SODO.png
│
├── ket_qua/
│   ├── anh/
│   ├── camera/
│   ├── video/
│   ├── csv/
│   └── lich_su_nhan_dien.csv
│
├── data/
│   └── thong_ke.xlsx
│
└── models/
    └── yolov8s.pt
