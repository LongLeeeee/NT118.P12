## Các tính năng chính ServerServer

### Xác thực người dùng (Auth)

- <strong>Đăng kí/Đăng nhập</strong>
  - người dùng tạo tài với email và password
  - Ngoài ra còn đăng nhập thông qua tài khoản **Google** và **Facebook**.
- <strong>Quên mật khẩu</strong>
  - Gửi mã OTP về email đã đăng ký để xác minh
  - Đặt lại mật khẩu thông qua mã OTP
- <strong>Token</strong>
  - Sử dụng **JWT** để xác thực người dùng sau khi đăng nhập
  - Token được lưu trữ cục bộ trên ứng dụng và gửi kèm các request

### Phát hiện ổ gà

- Thu thập dữ liệu từ **cảm biến gia tốc (accelerometer)** trên điện thoại.
- Nhận diện ổ gà dựa trên ngưỡng dao động bất thường.
- Ghi lại tọa độ GPS, thời gian và phân loại ổ gà.
- Gửi thông tin về server qua RESTful API

## Backend Server

### Công nghệ sử dụng

- **Ngôn ngữ:** Nodejs
- **Framework:** Express.js
- **Cơ sở dữ liệu:** MongoDB
- **Xác thực:** JWT, Google OAuth2, Facebook Login

### API xác thực

| Phương thức | Endpoint                     | Mô tả                           |
| ----------- | ---------------------------- | ------------------------------- |
| `POST`      | `/api/users/register`        | `Đăng kí tài khoản`             |
| `POST`      | `/api/users/login`           | `Đăng nhập bằng email/pasword`  |
| `POST`      | `/api/user/google-sign-in`   | `Đăng nhập bằng Google`         |
| `POST`      | `/api/user/facebook-sign-in` | `Đăng nhập bằng FFacebook`      |
| `POST`      | `/api/user/forgot-pasword`   | `Gửi OTP đến email`             |
| `POST`      | `/api/user/verify`           | `Xác thực OTP`                  |
| `PUT`       | `/api/user/edit`             | `Thay đổi thông tin người dùng` |
