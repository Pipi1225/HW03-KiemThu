# Báo cáo Cá nhân - Scenario C: Admin manages users

**Sinh viên thực hiện:** [Điền Tên - MSSV]
**Kịch bản chọn:** Scenario C — Admin manages users (Function group: user administration).

## 1. Lý do chọn 4 màn hình (Screens Selection)
Tôi đã chọn 4 màn hình/chức năng sau thuộc Scenario C để đảm bảo độ bao phủ từ việc xem, chỉnh sửa đến thao tác xuất dữ liệu:
1. **(C1) Users list:** Màn hình danh sách người dùng với bộ lọc tìm kiếm (search), lọc theo quyền (role/active filters), và các cột thông tin.
2. **(C2) Assign Role / edit user:** Màn hình/Form cấp quyền và chỉnh sửa thông tin người dùng.
3. **(C3) Block-Unblock and Reset-Password dialogs:** Các hộp thoại xác nhận khi khóa/mở khóa tài khoản hoặc đặt lại mật khẩu (đánh giá feedback, audit).
4. **(C4) Export to Excel:** Chức năng xuất dữ liệu (đánh giá feedback tải xuống và độ hoàn thiện của cột).

---

## 2. Task 1B: Thực thi GUI Checklist

*Lưu ý: Bảng dưới đây đã được rút gọn để minh họa. Trong file nộp, hãy copy đầy đủ 48 tiêu chí từ file `shared_gui_checklist.md`.*

| ID | Checklist Item | C1 (Users List) | C2 (Assign Role) | C3 (Block/Reset Dialogs) | C4 (Export Excel) | Notes (Lý do Fail & Tên file ảnh) |
|---|---|---|---|---|---|---|
| IA-01-01 | Grid & Spacing | Pass | Pass | Pass | N/A | |
| IA-02-04 | Error Messages | N/A | Fail | N/A | N/A | C2: Không báo lỗi cụ thể khi nhập sai định dạng email. Ảnh: `C2_error_msg.png` |
| ... | ... | ... | ... | ... | ... | ... |

*(Bổ sung danh sách Bugs tìm được ở đây, bao gồm: screen, steps to reproduce, expected vs actual, severity, screenshot)*

---

## 3. Task 2: Usability Testing (Kiểm thử tính khả dụng)

### 3.1. Thiết kế Kịch bản (Task Scenario)
- **Bối cảnh:** Bạn là quản trị viên hệ thống của khoa.
- **Mục tiêu yêu cầu người dùng thực hiện (Goal-oriented):** "Hãy tìm kiếm một người dùng tên là 'Nguyen Van A' trong hệ thống. Hãy cấp quyền 'Lecturer' cho người này. Sau đó, hãy thử khóa (block) tài khoản của họ và xuất danh sách toàn bộ người dùng ra file Excel để báo cáo."

### 3.2. Kết quả đo lường (Metrics Table)
*Đối tượng: 5 người dùng (Sinh viên / Giảng viên ngoài lớp học).*

| Participant | User Profile | Task Success (Full/Partial/Fail) | Time on Task | Errors/Hesitations | SUS / UEQ-S Score |
|---|---|---|---|---|---|
| P1 (Nam - **1234) | Sinh viên năm 3 | Full | 1m 30s | 1 | 85 |
| P2 (...) | ... | ... | ... | ... | ... |
| P3 (...) | ... | ... | ... | ... | ... |
| P4 (...) | ... | ... | ... | ... | ... |
| P5 (...) | ... | ... | ... | ... | ... |

### 3.3. Phân tích & Báo cáo Usability (Usability Report)
*(Nhóm các điểm khó khăn (pain points) của 5 người dùng, xếp hạng độ nghiêm trọng (0-4) kèm ảnh chụp màn hình và đề xuất khắc phục)*

---

## 4. Task 3: Cross-Browser & Cross-Platform Testing

### 4.1. Ma trận tương thích (Compatibility Matrix)
*Yêu cầu bao phủ: Mỗi OS ≥ 1 lần, mỗi Browser ≥ 1 lần, mỗi Device class ≥ 1 lần cho từng màn hình.*

**Màn hình C1 (Users List):**
| Thiết bị (Device) | Hệ điều hành (OS) | Trình duyệt (Browser) | Kết quả (Pass/Fail) & Ghi chú lỗi | Screenshot File |
|---|---|---|---|---|
| Desktop (MacBook) | macOS 14 | Safari | Pass | `C1_mac_safari.png` |
| Tablet (iPad) | iOS 17 | Chrome | Fail (Bảng bị tràn viền) | `C1_ipad_chrome.png` |
| Phone (Galaxy S23) | Android 14 | Edge | Pass | `C1_android_edge.png` |

*(Làm tương tự cho C2, C3, C4 - Phối hợp thêm các Browser khác như Firefox, Opera để đủ 5 trình duyệt)*

### 4.2. Danh sách Lỗi hiển thị đa nền tảng
*(Liệt kê các lỗi layout, overflow, unreadable text tìm thấy trên các thiết bị/trình duyệt cụ thể)*
