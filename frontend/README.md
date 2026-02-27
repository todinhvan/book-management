# Book Management - Frontend

Đây là phần Frontend của dự án **Book Management**. Dự án được xây dựng dựa trên framework **Vue.js 3** và công cụ **Vue CLI**.

## 🛠 Tài liệu kỹ thuật

### Công nghệ sử dụng

- **Vue.js 3**: Framework chính để xây dựng giao diện người dùng.
- **Vue Router**: Xử lý điều hướng và định tuyến các trang trong ứng dụng đa tham chiếu (SPA).
- **Axios & Vue-Axios**: Được sử dụng để gửi các yêu cầu HTTP (gọi API) lên Backend.
- **Vue Cookies**: Quản lý phiên làm việc, lưu trữ token hoặc dữ liệu người dùng tại trình duyệt client.
- **Vue Sweetalert2**: Hiển thị các thông báo popup (alert) thân thiện với người dùng.
- **Moment**: Xử lý và định dạng các kiểu dữ liệu thời gian.
- **Core-js**: Polyfill cho phép sử dụng các tính năng mới của JavaScript trên các trình duyệt cũ.

### Yêu cầu hệ thống

- **Node.js**: (Khuyến nghị phiên bản LTS)
- Công cụ quản lý gói **NPM** hoặc **Yarn**

---

## � Cấu trúc thư mục

```text
frontend/
├── public/          # Chứa các file tĩnh (index.html, favicon,...)
├── src/             # Thư mục mã nguồn chính của ứng dụng Vue
│   ├── assets/      # Lưu trữ hình ảnh, CSS, fonts toàn cục
│   ├── components/  # Các component Vue dùng chung (tái sử dụng)
│   ├── router/      # Định nghĩa cài đặt Vue Router
│   ├── views/       # Các màn hình chính phân theo route (Trang chủ, Admin,...)
│   ├── App.vue      # Component gốc (Root Component)
│   └── main.js      # Entry point khởi tạo Vue App
├── package.json     # Chứa danh sách các thư viện và script
├── vue.config.js    # Cấu hình cho Vue CLI
└── babel.config.js  # Cấu hình biên dịch Babel
```

---

## �🚀 Hướng dẫn cài đặt và chạy dự án

### 1. Cài đặt các thư viện (Dependencies)

Mở terminal tại thư mục `frontend` và chạy lệnh sau để tải về các gói cần thiết được khai báo:

```bash
npm install
```

### 2. Khởi chạy dự án ở chế độ phát triển (Development)

Chạy lệnh sau để khởi động server frontend. Dự án đã được cấu hình mặc định để chạy trên cổng **`8091`**.

```bash
npm run serve
```

Sau khi khởi chạy thành công, hãy mở trình duyệt web và truy cập vào địa chỉ: [http://localhost:8091](http://localhost:8091)

### 3. Build dự án cho môi trường sản xuất (Production)

Để đóng gói và tối ưu ứng dụng cho việc triển khai trên server (deploy), chạy lệnh sau:

```bash
npm run build
```

Kết quả bản build (gồm file HTML, JS, CSS đã nén) sẽ nằm trong thư mục `dist`.

### 4. Kiểm tra mã nguồn (Linting)

Để tự động tìm và sửa các lỗi viết code dựa trên tiêu chuẩn ESlint (đã thiết lập sẵn), chạy lệnh:

```bash
npm run lint
```
