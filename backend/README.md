# Book Management - Backend

Đây là phần Backend của dự án **Book Management**, cung cấp các endpoint API để phần Frontend có thể kết nối. Hệ thống Server API này được xây dựng với nền tảng **Node.js**, framework **Express.js**, và cơ sở dữ liệu **MongoDB**.

## 🛠 Tài liệu kỹ thuật

### Công nghệ sử dụng

- **Node.js & Express.js**: Nền tảng cốt lõi và framework Web API mượt mà, hỗ trợ tạo kiến trúc định tuyến nhanh.
- **MongoDB & Mongoose**: Hệ quản trị cơ sở dữ liệu Document NoSQL. Kết nối qua Object Data Modeling (Mongoose) để thao tác logic với các Model nhanh hơn.
- **Dotenv**: Nạp và quản lý các thiết lập biến môi trường nhạy cảm thông qua file `.env`.
- **CORS**: Cho phép hệ thống xử lý các chia sẻ tài nguyên tới nguồn/domain khác.
- **Body-Parser & Cookie-Parser**: Middleware dùng để trích xuất dữ liệu thân yêu cầu (JSON) và gửi, nhận cookies.
- **Nodemon**: Công cụ dev tiện ích, hỗ trợ tự động reset server Node mỗi khi có thay đổi trong các file mã nguồn.
- **Bảo mật**: Sử dụng gói `md5` để mã hóa mật khẩu, dữ liệu.
- **Mongoose-slug-updater & unidecode**: Hỗ trợ tạo slug từ nội dung để làm đường link thân thiện.

### Yêu cầu hệ thống

- **Node.js**: (Khuyến nghị phiên bản LTS)
- **MongoDB**: Đã cài và đang chạy service MongoDB trên máy tính (hoặc tài khoản MongoDB Atlas online).

---

## 📁 Cấu trúc thư mục

```text
backend/
├── api/             # Nơi chứa các Route và Controller xử lý logic API
├── config/          # Cấu hình hệ thống (Database, App...)
├── helpers/         # Các hàm tiện ích dùng chung
├── models/          # Định nghĩa cấu trúc dữ liệu MongoDB (Mongoose Schema)
├── index.js         # Entry point (Điểm khởi đầu) của ứng dụng Node.js
├── .env             # File lưu trữ biến môi trường (không được commit)
├── package.json     # Chứa danh sách các thư viện và script
└── package-lock.json
```

---

## 🚀 Hướng dẫn cài đặt và chạy dự án

### 1. Cài đặt các thư viện (Dependencies)

Mở terminal tại thư mục gốc của `backend` và chạy lệnh tải về các gói:

```bash
npm install
```

### 2. Cấu hình biến môi trường

Kiểm tra cấu hình trong file `.env` ở trong thư mục backend để cấu hình các kết nối.
Mặc định hệ thống sử dụng các thông số như sau:

```env
PORT=5268
MONGODB_URL=mongodb://localhost:27017/book-management
```

_(Hãy chắc chắn rẳng service MongoDB của bạn đang hoạt động trên port 27017 trước khi khởi động server)._

### 3. Khởi chạy Server

Để chạy API dự án bằng `nodemon` (tự động restart khi sửa code), thực thi lệnh sau trên terminal của backend:

```bash
npm start
```

Nếu cấu hình đúng đắn, thông báo server thành công sẽ xuất hiện API service sẽ chạy trên cổng mặc định: [http://localhost:5268](http://localhost:5268)
