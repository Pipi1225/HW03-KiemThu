# README HW03

- Student name: Dương Gia Huy
- Student ID: 23127052

---

## 1. Bảng Tự Đánh Giá (Self-Assessment Table)

| STT | Criteria | Grade | Self-Assessed Grade
|---|---|---|---|
| **1a** | Task 1A — Shared checklist (> 40 items, IA-01...IA-04) + reference sources + AI prompts (group) | 15 | **15** |
| **1b** | Task 1B — Checklist execution on ≥ 3 screens + bug reports (individual) | 15 | **15** |
| **2** | Task 2 — User testing with 5 real users (scenario + 5 sessions + analysis → Usability Report) | 25 | **20** |  
| **3** | Task 3 — Cross-Browser / Cross-Platform matrix (3 OS × 5 browsers × 3 device classes) | 25 | **25** |
| **4** | Bug & Usability Findings submission (Google Form) + aggregated log | 10 | **10** |
| **5** | Agent Skills | 10 | **10** |
| **Total** |  | 100 | **95** |

---

## 2. Tóm Tắt Kết Quả Kiểm Thử (Test Summary)

### 2.1. Kịch bản & Màn hình kiểm thử (Scenario & Screens)
- **Kịch bản lựa chọn:** **Scenario C — Admin manages users** (Nhóm chức năng quản trị tài khoản người dùng trên hệ thống EMS).
- **Danh sách màn hình đã thực hiện kiểm thử:**
  1. **C1 - Users List:** Danh sách người dùng, chức năng tìm kiếm, các bộ lọc theo vai trò (Role), trạng thái hoạt động (Status) và hiển thị cột.
  2. **C2 - Create / Edit User & Assign Role:** Form tạo mới, chỉnh sửa thông tin người dùng và phân quyền tài khoản.
  3. **C3 - Export to Excel:** Tính năng xuất danh sách người dùng ra tệp Excel, kiểm tra tính đầy đủ của dữ liệu cột và phản hồi tải tệp.
  4. **C4 - Delete User Confirmation Dialog & Audit Logs:** Hộp thoại xác nhận xóa người dùng và hiển thị thông tin Audit (ngày tạo, ngày cập nhật, người thao tác).

### 2.2. Số liệu Checklist GUI (Designed / Executed / Passed / Failed)
Tổng số mục kiểm tra được thiết kế trong bộ checklist chung là **50 mục**. Kết quả thực thi chi tiết trên 4 màn hình của hệ thống:

| Màn hình kiểm thử (Screen) | Tổng số mục thiết kế | Số mục được chạy thực tế (Executed) | Đạt (Pass) | Lỗi (Fail) | Không áp dụng (N/A) |
|---|:---:|:---:|:---:|:---:|:---:|
| **C1 - Users List** | 50 | 21 | 18 | 3 | 29 |
| **C2 - Create / Edit User** | 50 | 21 | 12 | 9 | 29 |
| **C3 - Export to Excel** | 50 | 10 | 6 | 4 | 40 |
| **C4 - Delete User & Audit** | 50 | 17 | 14 | 3 | 33 |
| **Tổng cộng (Toàn bộ dự án)** | **50 (Độc lập)** | **69** | **50** | **19** | **131** |

### 2.3. Thống kê Lỗi phát hiện (Bug & Usability Log Count)
Hệ thống ghi nhận tổng cộng **29 lỗi** thực tế trong quá trình kiểm thử checklist GUI. Phân loại theo tính chất và màn hình như sau:
- **Lỗi chức năng (Bug):** 9 lỗi
- **Vấn đề trải nghiệm (Usability):** 20 lỗi

| Màn hình (Screen) | Lỗi chức năng (Bug) | Vấn đề trải nghiệm (Usability) | Tổng số lỗi |
|---|:---:|:---:|:---:|
| **C1 - Users List** | 5 | 3 | **8** |
| **C2 - Create / Edit User** | 1 | 11 | **12** |
| **C3 - Export to Excel** | 3 | 3 | **6** |
| **C4 - Delete User & Audit** | 0 | 3 | **3** |
| **Tổng cộng** | **9** | **20** | **29** |

### 2.4. Kết quả Kiểm thử tính Khả dụng (Usability Testing Summary)
- **Số lượng người tham gia kiểm thử:** 4 người dùng thật 
1. Nguyễn Tấn Đạt - SV năm 3
2. Nguyễn Thị Cẩm Nhung - Developer
3. Nguyễn Tuấn Kiệt - SV năm 1
4. Dương Thúy Mi - Giáo viên


- **Điểm đánh giá hệ thống (SUS Score):**
  - Người tham gia 1: **100 / 100**
  - Người tham gia 2: **90 / 100**
  - Người tham gia 3: **87.5 / 100**
  - Người tham gia 4: **97.5 / 100**
  - **Điểm SUS trung bình của hệ thống:** **93.75 / 100** (Mức độ hài lòng rất cao, tuy nhiên vẫn cần khắc phục các lỗi trải nghiệm).

- **Thống kê vấn đề khả dụng phát hiện qua quan sát (Ranked Usability Issues by Severity):**
  - **Mức độ 4 (Blocker) / Mức độ 0 (None):** 0 lỗi.
  - **Mức độ 3 (Nặng):** 3 lỗi (Excel Error cấu trúc tệp; Search bị lỗi pagination và chữ thường; Search không hỗ trợ tìm kiếm đầy đủ Họ Tên).
  - **Mức độ 2 (Nhẹ):** 4 lỗi (Nút Active/Unactive tương phản kém; Không có trang xem chi tiết User; Validate Form tuần tự từng trường; Filter kích thước nhỏ khó bấm).
  - **Mức độ 1 (Thẩm mỹ):** 1 lỗi (Nút Create User di chuột vào không đổi cursor pointer).
  - **Tổng số lỗi xếp hạng:** 8 lỗi.

### 2.5. Ma trận Kiểm thử tương thích (Compatibility Matrix Coverage)
Ma trận kiểm thử đa cấu hình đã phủ được **28 lượt chạy** (4 màn hình × 7 Run-IDs) bao gồm:
- **3 Hệ điều hành (OS):** Windows 11, macOS 14, Android 15 và Android 16.
- **5 Trình duyệt (Browsers):** Google Chrome, Mozilla Firefox, Microsoft Edge, Apple Safari, Opera.
- **3 Thiết bị (Device Classes):** Máy tính để bàn (Desktop), Máy tính bảng (Tablet), Điện thoại di động (Phone).

### 2.6. Video minh chứng kiểm thử
- **Đường dẫn thư mục Google Drive chứa videos:** [Link Google Drive](https://drive.google.com/drive/folders/1BoebOJamcK_G9Xbpi6mvRKpUjvctfNwq?usp=sharing)
- **Danh sách tệp video minh chứng:**
  - `User-1.mp4` (Nguyễn Tấn Đạt)
  - `User-2.mp4` (Nguyễn Thị Cẩm Nhung)
  - `User-3.mp4` (Nguyễn Tuấn Kiệt)
  - `User-4.mp4` (Dương Thúy Mi)

### 2.7 Video Demo Agent Skill
- **Đường dẫn tới Video Demo Agent Skill:** [Link Youtube Agent Skill](https://youtu.be/ngua00G-mg8)
- **Đường dẫn tới Video Demo /browser của Antigravity:** [Link Youtube Demo Browser Antigravity](https://youtu.be/phtz8jDlCw4)