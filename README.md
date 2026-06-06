<h2 align="center"> <a href="https://dainam.edu.vn/vi/khoa-cong-nghe-thong-tin"> 🎓 Faculty of Information Technology (DaiNam University) </a> </h2> <h2 align="center"> CHAT ROOM DÙNG UDP MULTICAST </h2> <div align="center"> <p align="center"> <img alt="AIoTLab Logo" width="170" src="https://github.com/user-attachments/assets/711a2cd8-7eb4-4dae-9d90-12c0a0a208a2" /> <img alt="AIoTLab Logo" width="180" src="https://github.com/user-attachments/assets/dc2ef2b8-9a70-4cfa-9b4b-f6c2f25f1660" /> <img alt="DaiNam University Logo" width="200" src="https://github.com/user-attachments/assets/77fe0fd1-2e55-4032-be3c-b1a705a1b574" /> </p>

# 📖 Giới thiệu

Hệ thống nhận diện và phân loại vật nuôi là ứng dụng sử dụng trí tuệ nhân tạo (AI) kết hợp mô hình YOLOv8 nhằm phát hiện, nhận diện và thống kê các loại vật nuôi từ ảnh, video hoặc camera thời gian thực.

Hệ thống hỗ trợ:

- Nhận diện vật nuôi theo thời gian thực.
- Đếm số lượng vật nuôi.
- Chụp ảnh tự động khi phát hiện vật nuôi.
- Lưu lịch sử nhận diện vào CSV.
- Xuất dữ liệu Excel.
- Hỗ trợ Webcam, Camera IP và ESP32-CAM.
- Dashboard thống kê trực quan.

---

# 🎯 Mục tiêu

- Xây dựng hệ thống nhận diện vật nuôi bằng AI.
- Hỗ trợ ảnh, video và camera.
- Thống kê số lượng vật nuôi.
- Lưu dữ liệu tự động.
- Hỗ trợ quản lý vật nuôi trong trang trại.

---

# 🔧 Công nghệ sử dụng

## 🤖 YOLOv8

- Nhận diện đối tượng thời gian thực.
- Độ chính xác cao.
- Tốc độ xử lý nhanh.

## 👁 OpenCV

- Xử lý ảnh.
- Xử lý video.
- Kết nối camera.

## 🌐 Streamlit

- Giao diện Web Dashboard.
- Hiển thị thống kê.
- Quản lý dữ liệu.

## 💾 Pandas

- Lưu dữ liệu CSV.
- Xuất báo cáo Excel.

---

# 🏗️ Kiến trúc hệ thống

```text
Camera / Ảnh / Video
          │
          ▼
       YOLOv8
          │
          ▼
     Nhận diện vật nuôi
          │
          ▼
    OpenCV xử lý ảnh
          │
          ▼
     Streamlit Dashboard
          │
          ▼
CSV / Excel / Thống kê
```

# 🚀 Chức năng chính

## 📷 Nhận diện qua Camera

- Webcam Laptop
- Camera điện thoại
- ESP32-CAM
- Nhận diện thời gian thực
- Tự động chụp ảnh

## 🖼 Nhận diện qua Ảnh

- Upload ảnh
- Phân tích ảnh
- Lưu ảnh kết quả

## 🎥 Nhận diện qua Video

- Upload video
- Phân tích từng frame
- Tạm dừng / Tiếp tục
- Tự động chụp ảnh
- Xuất CSV

## 📊 Dashboard

- Tổng số vật nuôi
- Biểu đồ thống kê
- Bảng dữ liệu
- Lịch sử nhận diện

---

# 📸 Hình ảnh minh họa

<p align="center">
<img src="docs/home.png" width="900">
</p>

<p align="center">
<em>Hình 1. Giao diện trang chủ</em>
</p>

<p align="center">
<img src="docs/camera.png" width="900">
</p>

<p align="center">
<em>Hình 2. Nhận diện qua Camera</em>
</p>

<p align="center">
<img src="docs/image.png" width="900">
</p>

<p align="center">
<em>Hình 3. Nhận diện qua Ảnh</em>
</p>

<p align="center">
<img src="docs/video.png" width="900">
</p>

<p align="center">
<em>Hình 4. Nhận diện qua Video</em>
</p>

<p align="center">
<img src="SODO.png" width="1000">
</p>

<p align="center">
<em>Hình 5. Sơ đồ hệ thống</em>
</p>

---

# 📂 Cấu trúc thư mục

```text
AnimalDetection/
│
├── app.py
├── requirements.txt
├── yolov8s.pt
│
├── docs/
│   ├── home.png
│   ├── image.png
│   ├── video.png
│   ├── camera.png
│   └── SODO.png
│
├── ket_qua/
│   ├── anh/
│   ├── csv/
│   └── lich_su_nhan_dien.csv
│
└── models/
    └── yolov8s.pt
```

# 🐾 Vật nuôi hỗ trợ

| STT | Loài |
|-----|-------|
| 1 | Chó |
| 2 | Mèo |
| 3 | Bò |
| 4 | Cừu |
| 5 | Ngựa |
| 6 | Gà |
| 7 | Vịt |
| 8 | Chim |
| 9 | Hươu |
| 10 | Voi |
| 11 | Gấu |
| 12 | Hươu cao cổ |

---

# ⚙️ Cài đặt

## Cài thư viện

```bash
pip install -r requirements.txt
```

## Chạy chương trình

```bash
streamlit run app.py
```

# 📊 Kết quả đầu ra

Hệ thống sẽ:

✅ Nhận diện vật nuôi

✅ Hiển thị độ tin cậy

✅ Vẽ Bounding Box

✅ Đếm số lượng

✅ Lưu CSV

✅ Xuất Excel

✅ Tự động chụp ảnh

✅ Dashboard thống kê

---

# 🔮 Hướng phát triển

- Train mô hình riêng.
- Kết nối MySQL.
- Kết nối Cloud.
- Cảnh báo qua Email/Zalo.
- Tích hợp IoT cho trang trại thông minh.
- Quản lý vật nuôi bằng AI.

---

# 👨‍💻 Thành viên thực hiện

| Họ tên | MSSV |
|Dương Xuân Thành |1671020291|


---

<div align="center">

### 🏆 ĐỒ ÁN TRÍ TUỆ NHÂN TẠO

### 🐄 HỆ THỐNG NHẬN DIỆN VÀ PHÂN LOẠI VẬT NUÔI BẰNG YOLOv8

Faculty of Information Technology - Dai Nam University

</div>
