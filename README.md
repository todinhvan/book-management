# 📚 Dự án: Book Management (Hệ thống Quản lý Sách)

Chào mừng bạn đến với dự án **Book Management**. Đây là một hệ thống ứng dụng web quản lý các đầu sách linh hoạt, được cấu trúc và xây dựng theo mô hình Client - Server tách biệt, đem lại trải nghiệm tương tác với hệ thống sách mượt mà trực quan.

- Đây là đồ án môn học CT449 - Phát triển ứng dụng Web - CTU

## ✨ Giới thiệu tổng quan

Dự án được phân chia rạch ròi thành 2 mảng chính:

- **Frontend (Giao diện người dùng):** Ứng dụng Single Page Application xây dựng trên công nghệ **Vue.js 3** tiên tiến, cung cấp hiệu năng điều hướng cao mà không phải reload trang web.
- **Backend (Hệ thống Server API):** Xây dựng trên nền tảng **Node.js / Express.js**, chịu trách nhiệm xử lý các thao tác logic nghiệp vụ, bảo mật và tương tác với cơ sở dữ liệu linh hoạt **MongoDB**.

## 📁 Cấu trúc thư mục

Toàn bộ dự án nằm chung trong một kho lưu trữ và được tổ chức như sau:

```text
/
├── backend/    # Mã nguồn, logic nghiệp vụ, API, và liên kết database
├── frontend/   # Mã nguồn giao diện Vue, layout, trang cho người dùng
└── README.md   # File hướng dẫn cấu trúc tổng quan
```

## ⚙️ Hướng dẫn cấu hình và cài đặt dự án

Vì đây là ứng dụng 2 thành phần độc lập, bạn cần chạy song song cả thư mục **backend** và **frontend** trong 2 cửa sổ terminal riêng biệt.
**Lưu ý quan trọng**: Đảm bảo rằng máy chủ MongoDB của bạn đã được bật và cài đặt thành công Node.js trước khi bắt tay vào thiết lập.

> **Trình tự khuyến nghị**: Khởi chạy API Backend trước, tiếp theo mới khởi chạy Giao diện Frontend.

### 🔌 1. API Server (Backend)

Phần này kết nối đến CSDL giúp xử lý dữ liệu hệ thống.

👉 **Xin vui lòng tham khảo thiết lập tại:** [Tài liệu & Cài đặt Backend](./backend/README.md)

### 🎨 2. Giao diện (Frontend)

Phần này giao tiếp với API backend để hiển thị dữ liệu tới người dùng cuối.

👉 **Xin vui lòng tham khảo thiết lập tại:** [Tài liệu & Cài đặt Frontend](./frontend/README.md)

---

_Chúc bạn có quá trình trải nghiệm, phát triển và thử nghiệm dự án thuận lợi!_
