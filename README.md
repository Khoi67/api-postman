# 🚀 Automated API Testing with Postman CLI & GitHub Actions

![API Tests](https://github.com/Khoi67/api-postman/actions/workflows/postman.yml/badge.svg)


Repository này được sử dụng để **tự động hóa kiểm thử API** bằng **Postman CLI** và tích hợp với **GitHub Actions** trong quy trình CI/CD.

---

## 🎯 Mục đích
- Tự động hóa việc kiểm thử API
- Phát hiện lỗi sớm khi có thay đổi source code
- Giảm phụ thuộc vào việc test thủ công trên Postman
- Áp dụng CI/CD cho QA / Tester

---

## 🛠 Công nghệ sử dụng
- GitHub Actions
- Postman CLI
- Postman Collection
- CI/CD Pipeline

---

## 🔄 Nguyên lý hoạt động

Khi có thay đổi code (push) lên repository:
- GitHub Actions được kích hoạt
- Postman CLI sẽ chạy Postman Collection
- Các API test được thực thi tự động
- Kết quả test được hiển thị trực tiếp trên GitHub Actions

---

## 🔐 Cấu hình Postman API Key

Để chạy được API test, repository cần cấu hình **Postman API Key**.

### Các bước cấu hình:
1. Truy cập **Repository → Settings**
2. Chọn **Secrets and variables → Actions**
3. Thêm secret mới:
   - **Name:** `POSTMAN_API_KEY`
   - **Value:** Postman API Key của bạn

> ⚠️ Không commit API Key trực tiếp vào source code để tránh lộ thông tin bảo mật.
