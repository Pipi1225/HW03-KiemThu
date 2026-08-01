/browser Hãy thực hiện kiểm thử tự động giao diện (GUI Usability) đối với màn hình C4 - Delete User Confirmation Dialog & Audit Logs trên môi trường web.
Các bước thực hiện:
1. Truy cập trang chủ: https://prod-dev.ems-fitus.cloud/
2. Đăng nhập với tài khoản:
   - Email: admin@gmail.com
   - Mật khẩu: Admin@123
3. Điều hướng tới trang Quản trị danh sách người dùng: https://prod-dev.ems-fitus.cloud/dashboard/admin/users
4. Thao tác kích hoạt phần C4 (Delete User Dialog):
   - Tìm một người dùng trong bảng danh sách và nhấn vào biểu tượng Thùng rác màu đỏ (Delete User icon).
   - Khi hộp thoại xác nhận xóa (Delete Confirmation Dialog) hiện lên, hãy chụp ảnh màn hình lại.
   - Thử rê chuột (hover) vào nút Xác nhận (Delete) và nút Hủy (Cancel) để xem hiệu ứng hover, thử tắt hộp thoại bằng cách click ra ngoài (backdrop click) hoặc nhấn Esc để kiểm tra tính năng đóng.
5. Thao tác kiểm tra phần C4 (Audit Created & Updated):
   - Quan sát các cột hoặc khu vực hiển thị thông tin Audit (ngày tạo Created At, ngày cập nhật Updated At, người tạo/cập nhật nếu có).
   - Chụp ảnh màn hình các cột/thông tin này.
6. Đọc checklist từ tệp: d:\DaiHoc\KiemThuPM\HW03\shared_gui_checklist.md
7. Đối chiếu các ảnh chụp màn hình C4 với checklist để tìm lỗi giao diện (UI/UX) và lỗi trải nghiệm người dùng (Usability) liên quan đến:
   - Màu sắc cảnh báo của nút hành động nguy hiểm (IA-04-06)
   - Đa ngôn ngữ trên popup cảnh báo xóa (IA-01-04)
   - Đóng popup an toàn (IA-03-03 / IA-04-03)
   - Định dạng ngày giờ hiển thị ở phần Audit (IA-02-09)
8. Tạo một tệp mới tên là d:\DaiHoc\KiemThuPM\HW03\Bug_C4.md và ghi nhận kết quả dưới dạng Markdown với bảng danh sách lỗi phát hiện được. 
Yêu cầu định dạng của Bug_C4.md:
- Mỗi lỗi phải có ID dạng BUG-C4-XX.
- Cột "Steps/Heuristic" phải được định dạng theo cấu trúc: **Mã_Heuristic**<br>1. Bước 1<br>2. Bước 2... (sử dụng thẻ <br> thay vì ký tự ->).
- Nếu không phát hiện lỗi nào, hãy ghi nhận màn hình đạt chuẩn và lập bảng liệt kê các điểm sáng thiết kế đạt điểm Pass.