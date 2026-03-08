# 🚦 Traffic Light Controller with FSM (STM32)

## 📌 Giới thiệu
Dự án tập trung vào việc thiết kế và hiện thực hệ thống điều khiển đèn giao thông sử dụng vi điều khiển **STM32F103**.  
Hệ thống được quản lý bằng **Finite State Machine (FSM)** kết hợp với **bộ định thời (Schedule)** để tối ưu hóa việc thực thi các tác vụ.

---

## ⚙️ Các chế độ hoạt động

- **NORMAL MODE**  
  Tự động điều khiển đèn giao thông tại hai tuyến đường theo chu kỳ **Đỏ – Xanh – Vàng**.

- **MANUAL MODE**  
  Cho phép chuyển trạng thái đèn thủ công thông qua nút nhấn.

- **MODIFY MODE**  
  Chế độ cài đặt và tùy chỉnh thời gian sáng của các đèn **Đỏ, Vàng, Xanh**.

- **Chế độ người đi bộ**  
  Kích hoạt trạng thái ưu tiên cho người đi bộ khi nhận tín hiệu từ nút nhấn tương ứng.

---

## 👥 Phân công nhiệm vụ (Nhóm 18)

| Họ và Tên | MSSV | Nhiệm vụ | Hoàn thành |
|-----------|------|----------|-----------|
| Nguyễn Văn Hiếu | 2310967 | Task LED, kiểm tra trên mạch thật | 100% |
| Nguyễn Minh Hạnh | 2310895 | Task LCD I2C, kiểm tra trên mạch thật | 100% |
| Trần Đình Hoàng | 2311075 | Task Schedule, bổ sung chế độ người đi bộ | 100% |

---

## 🔧 Thông số kỹ thuật

- **Vi điều khiển**  
  STM32F103C6 (Mô phỏng) và STM32F103RBTx (Mạch thật)

- **Giao thức hiển thị**  
  LCD 16x2 giao tiếp **I2C** để hiển thị chế độ hoạt động và thời gian đếm ngược.

- **Cấu trúc dữ liệu**  
  Bộ định thời sử dụng **Linked List** để tối ưu hàm update với độ phức tạp **O(1)**.

---

## 🛠 Công cụ sử dụng

- **STM32CubeIDE** – Lập trình Embedded C  
- **Proteus** – Mô phỏng hệ thống
