<h2 align="center">
    <a href="https://dainam.edu.vn/vi/khoa-cong-nghe-thong-tin">
    🎓 Faculty of Information Technology (DaiNam University)
    </a>
</h2>

<h2 align="center">
    🐄 HỆ THỐNG NHẬN DIỆN VÀ PHÂN LOẠI VẬT NUÔI BẰNG YOLOv8
</h2>

<div align="center">
    <p align="center">
        <img alt="AIoTLab Logo" width="170" src="https://github.com/user-attachments/assets/711a2cd8-7eb4-4dae-9d90-12c0a0a208a2" />
        <img alt="AIoTLab Logo" width="180" src="https://github.com/user-attachments/assets/dc2ef2b8-9a70-4cfa-9b4b-f6c2f25f1660" />
        <img alt="DaiNam University Logo" width="200" src="https://github.com/user-attachments/assets/77fe0fd1-2e55-4032-be3c-b1a705a1b574" />
    </p>

[![YOLOv8](https://img.shields.io/badge/YOLOv8-Object%20Detection-green?style=for-the-badge)](https://github.com/ultralytics/ultralytics)
[![OpenCV](https://img.shields.io/badge/OpenCV-Computer%20Vision-blue?style=for-the-badge)](https://opencv.org/)
[![Streamlit](https://img.shields.io/badge/Streamlit-Web%20Dashboard-red?style=for-the-badge)](https://streamlit.io/)

</div>

---

# 📖 1. Giới thiệu hệ thống

Trong bối cảnh cuộc cách mạng công nghiệp 4.0 và xu hướng phát triển nông nghiệp thông minh, việc ứng dụng trí tuệ nhân tạo (Artificial Intelligence - AI) vào quản lý chăn nuôi đang ngày càng trở nên quan trọng. Các trang trại hiện đại cần những giải pháp tự động giúp giám sát đàn vật nuôi, thống kê số lượng, giảm chi phí nhân công và nâng cao hiệu quả quản lý.

Đề tài **"Hệ thống Nhận diện và Phân loại Vật nuôi bằng YOLOv8"** được xây dựng nhằm ứng dụng công nghệ Computer Vision và Deep Learning để nhận diện vật nuôi trong hình ảnh, video và camera thời gian thực.

Hệ thống sử dụng mô hình YOLOv8 để phát hiện đối tượng, kết hợp OpenCV để xử lý ảnh/video và Streamlit để xây dựng giao diện Web Dashboard trực quan.

---

# 🎯 2. Mục tiêu đề tài

Mục tiêu chính của hệ thống:

- Xây dựng hệ thống nhận diện vật nuôi bằng trí tuệ nhân tạo.
- Phát hiện vật nuôi trong thời gian thực.
- Hỗ trợ nhận diện từ ảnh, video và camera.
- Thống kê số lượng vật nuôi tự động.
- Lưu lịch sử nhận diện.
- Xuất báo cáo CSV và Excel.
- Hỗ trợ Camera Laptop, IP Camera và ESP32-CAM.
- Xây dựng Dashboard trực quan phục vụ quản lý.

---

# 🔧 3. Công nghệ sử dụng

## 🤖 YOLOv8

YOLOv8 là mô hình phát hiện đối tượng thời gian thực mới nhất của Ultralytics.

Chức năng:

- Nhận diện vật thể.
- Vẽ Bounding Box.
- Hiển thị độ tin cậy.
- Xử lý thời gian thực.
- Độ chính xác cao.

---

## 👁 OpenCV

OpenCV được sử dụng để:

- Đọc ảnh.
- Đọc video.
- Kết nối webcam.
- Kết nối camera IP.
- Kết nối ESP32-CAM.
- Hiển thị kết quả nhận diện.

---

## 🌐 Streamlit

Streamlit được sử dụng để xây dựng giao diện Web.

Chức năng:

- Upload ảnh.
- Upload video.
- Hiển thị camera.
- Dashboard thống kê.
- Xuất dữ liệu.

---

## 💾 Pandas

Pandas được sử dụng để:

- Quản lý dữ liệu.
- Xuất CSV.
- Xuất Excel.
- Thống kê kết quả.

---

## 📊 Matplotlib

Matplotlib được sử dụng để:

- Vẽ biểu đồ cột.
- Vẽ biểu đồ thống kê.
- Hiển thị dữ liệu trực quan.

---

# 🏗️ 4. Kiến trúc hệ thống

```text
                 +------------------+
                 |  Người dùng      |
                 +---------+--------+
                           |
                           |
                           ▼
        +----------------------------------+
        |  Ảnh / Video / Camera / ESP32   |
        +----------------+-----------------+
                         |
                         ▼
                +----------------+
                |    YOLOv8      |
                | Object Detect  |
                +--------+-------+
                         |
                         ▼
                +----------------+
                |    OpenCV      |
                | Image Process  |
                +--------+-------+
                         |
                         ▼
                +----------------+
                |   Streamlit    |
                |   Dashboard    |
                +--------+-------+
                         |
          +--------------+--------------+
          |                             |
          ▼                             ▼
    CSV Report                    Excel Report
```

# 🚀 5. Chức năng hệ thống

## 📷 Nhận diện qua Camera

Hệ thống hỗ trợ:

- Webcam Laptop.
- Camera điện thoại.
- ESP32-CAM.

Tính năng:

- Nhận diện thời gian thực.
- Đếm số lượng vật nuôi.
- Chụp ảnh tự động.
- Lưu dữ liệu CSV.

---

## 🖼 Nhận diện qua Ảnh

Người dùng có thể:

- Upload ảnh.
- Phân tích ảnh.
- Nhận diện vật nuôi.
- Lưu ảnh kết quả.

---

## 🎥 Nhận diện qua Video

Người dùng có thể:

- Upload video.
- Phân tích từng frame.
- Tạm dừng.
- Tiếp tục.
- Tua video.
- Tự động chụp ảnh.
- Xuất dữ liệu CSV.

---

## 📊 Dashboard thống kê

Dashboard hiển thị:

- Tổng số vật nuôi.
- Số lượng từng loại.
- Biểu đồ cột.
- Lịch sử nhận diện.
- Báo cáo tổng hợp.

---

## 💾 Quản lý dữ liệu

Hệ thống hỗ trợ:

- Lưu ảnh.
- Lưu CSV.
- Xuất Excel.
- Xem lịch sử nhận diện.

---

# 🐾 6. Các loại vật nuôi hỗ trợ

| STT | Loài vật |
|------|----------|
| 1 | 🐶 Chó |
| 2 | 🐱 Mèo |
| 3 | 🐄 Bò |
| 4 | 🐑 Cừu |
| 5 | 🐎 Ngựa |
| 6 | 🐔 Gà |
| 7 | 🦆 Vịt |
| 8 | 🐦 Chim |
| 9 | 🦌 Hươu |
| 10 | 🐘 Voi |
| 11 | 🐻 Gấu |
| 12 | 🦒 Hươu cao cổ |

---

# 📸 7. Hình ảnh chức năng

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
  <img src="SODO.png" width="1000"/>
</p>

<p align="center">
<em>Hình 5: Sơ đồ kiến trúc hệ thống</em>
</p>
