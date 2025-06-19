# Gym-Manager
# Thành viên nhóm
| STT | Họ và Tên             | Mã sinh viên | Email Phenikaa                            | Email cá nhân (nếu có)             |
|-----|------------------------|--------------|--------------------------------------------|------------------------------------|
| 1   |  Dương Ngọc Anh        | 23010249     | 23010249@st.phenikaa-uni.edu.vn            |                                    |
# 🏋️‍♂️ Ứng dụng Quản lý Phòng Gym – Dự án Java Swing

Đây là ứng dụng quản lý phòng gym được phát triển bằng ngôn ngữ **Java (Swing GUI)** kết hợp với **SQL Server 2022** và thư viện JDBC để kết nối cơ sở dữ liệu. Dự án được thực hiện trong khuôn khổ học phần **Kỹ Thuật Phần Mềm (KTPM)** tại **Trường Đại học Phenikaa**, nhóm sinh viên lớp CSE702025 - Nhóm 12.

---

## 🚀 Chức năng chính

- ✅ **Quản lý học viên**: thêm, sửa, xóa thông tin, lọc theo gói tập, trạng thái tập
- ✅ **Quản lý gói tập**: tạo mới các gói tập (theo tháng, quý...), quy định số buổi và mức giá
- ✅ **Quản lý nhân viên / huấn luyện viên**: phân quyền đăng nhập, theo dõi lịch làm việc
- ✅ **Quản lý thiết bị**: thêm – sửa – xóa các máy móc, thiết bị trong phòng tập
- ✅ **Tư vấn gói tập**: ghi nhận nhu cầu khách hàng và đề xuất gói phù hợp
- ✅ **Thống kê – báo cáo doanh thu**: theo thời gian, theo gói tập, theo nhân viên
- ✅ **Chức năng đăng nhập – phân quyền**: Admin và Nhân viên có quyền truy cập khác nhau

---

## 🛠️ Công nghệ sử dụng

| Thành phần | Công nghệ |
|------------|-----------|
| Giao diện | Java Swing (JFrame, JPanel, JTable...) |
| CSDL | SQL Server 2022 (sử dụng Docker) |
| Kết nối DB | JDBC |
| Môi trường | NetBeans / IntelliJ IDEA |
| Kiểu dữ liệu trao đổi | DAO – Data Access Object pattern |

---

## 🗃️ Cấu trúc dữ liệu chính

- `NguoiDung` (User) – tài khoản đăng nhập
- `HocVien` – thông tin học viên
- `GoiTap` – thông tin gói tập
- `NhanVien` – danh sách nhân viên
- `ThietBi` – thiết bị phòng tập
- `DangKy` – bảng trung gian học viên – gói tập
- `HoaDon` – thống kê doanh thu

---

## 🔌 Yêu cầu cài đặt

- Java 11 trở lên
- SQL Server 2022 (Docker hoặc cài sẵn)
- JDBC Driver cho SQL Server
- IDE: NetBeans / IntelliJ IDEA
- Cấu hình kết nối:
  ```java
  String url = "jdbc:sqlserver://localhost:1433;databaseName=TenCSDL";
  String user = "sa";
  String password = "MatKhauCuaBan";
