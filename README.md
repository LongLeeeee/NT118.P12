<p align="center">
  <img src="PoLoT/logo.png" alt="Welcome" width="50%" />
</p>

# PoLoT

Đây là đồ án môn Phát triển ứng dụng trên thiết bị di động. Mục tiêu của đồ án là xây dựng nên ứng dụng cho phép người dùng detect và submit vị trí của ổ gà một cách tự động hoặc thủ công. Ngoài ra, còn cảnh báo khi đến gần vị trí của ổ gà, liệt kê số ổ gà khi định tuyến đường đi.

Đồ án gồm 2 phần là phần Server và phần Mobile App.

### Server

Server đảm nhận các nhiệm vụ:

- Nhiệm vụ liên quan đến xác thực người dùng như login, register, forgot password,... và nhiệm vụ lưu trữ, kết nối các người dùng.
- Nhiệm vụ liên quan để việc lưu trữ ổ gà, kết nối người dùng đề xây dụng hệ thống bản đồ cảnh báo các vị trí có ổ gà.
  Xem chi tiết [tại đây](https://github.com/LongLeeeee/NT118.P12/tree/main/nodejs_server).

### Mobile App

Mobile App cung cấp giao diện cho người dùng với các chức năng:

- Đăng nhập, đăng ký, khôi phục mật khẩu.
- Tự động phát hiện và thông tin ổ gà về server.
- Lấy thông tin ổ gà hiển thị lên bản đồ.
- Tạo các thống kê liên quan để thời gian di chuyển, quãng đường di chuyển, số lượng ổ gà đã phát hiện.
  Xem chi tiết [tại đây](https://github.com/LongLeeeee/NT118.P12/tree/main/PoLoT).
