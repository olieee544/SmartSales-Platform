# Hướng dẫn sử dụng Git cho dự án SmartSales-Platform

## 1. Cấu trúc phân nhánh

Dự án sử dụng mô hình phân nhánh như sau:

- `main`: nhánh chính (code ổn định, đã review)
- `frontend`: giao diện người dùng
- `backend`: API, xử lý dữ liệu
- `docs`: lưu tài liệu báo cáo, hình ảnh

## 2. Clone dự án về máy

```bash
git clone https://github.com/olieee544/SmartSales-Platform.git
cd SmartSales-Platform
```

---

## 3. Tạo nhánh mới cho từng chức năng

```bash
git checkout -b feature/login-ui
```

---

## 4. Commit thay đổi

```bash
git add .
git commit -m "Thêm giao diện đăng nhập"
```

---

## 5. Push nhánh lên GitHub

```bash
git push origin feature/login-ui
```

---

## 6. Tạo Pull Request (PR)

1. Truy cập GitHub repository.
2. Chọn **Compare & Pull Request**.
3. Gửi PR để merge vào **main** hoặc các nhánh liên quan (**frontend**, **backend**).

---

## 7. Quy ước đặt commit

| Tiền tố     | Ý nghĩa                   |
| ----------- | ------------------------- |
| `feat:`     | Thêm chức năng mới        |
| `fix:`      | Sửa lỗi                   |
| `docs:`     | Cập nhật tài liệu         |
| `refactor:` | Cải tiến code             |
| `style:`    | Thay đổi giao diện, style |

**Ví dụ:**  
`feat: thêm chức năng đăng ký tài khoản`
`fix: sửa lỗi gọi API khi đăng nhập`
`docs: cập nhật hướng dẫn Git`

---

## 8. Cập nhật code mới từ nhánh main

```bash
git checkout main
git pull origin main
git checkout feature/login-ui
git merge main
```

---

## 9. Lưu ý khi làm việc nhóm

- Mỗi thành viên làm việc trên nhánh riêng
- Không commit trực tiếp lên **main**
- Đảm bảo commit rõ ràng, dễ hiểu
- Kiểm tra kỹ trước khi gửi Pull Request

---

### Người phụ trách Git & DevOps

- **Họ tên:** Hong Phuc
- **Vai trò:** Quản lý GitHub, phân nhánh, hướng dẫn deploy  
- **Liên hệ:** Zalo

---
