# AI AUDIT REPORT

- Student name: Dương Gia Huy
- Student ID: 23127052

## AI-generated Artifact

Em đã sử dụng AI cho những task sau đây:

### Artifact 1: 
**1. Prompt + Tool**
- **Tool:** Gemini 3.1 Pro (Antigravity)
- **Timestamp:** 20:50 26/07/2026
- **Prompt:**
```text
[shared_gui_checklist.md](file;file:///d:/DaiHoc/KiemThuPM/HW03/shared_gui_checklist.md) 
Nhóm tôi đã có shared check list, và tôi đã quyết định (cũng đã thông báo cho nhóm) là mình sẽ làm Scenario C, 4 screen.
```

**2. AI Output:**
```text
AI đề xuất chia Scenario C thành 4 màn hình (C1 - C4) để bao phủ quy trình làm việc của Admin và tạo sẵn khung sườn báo cáo Report_ScenarioC_Template.md chứa checklist, kịch bản thử nghiệm và ma trận cross-platform.
```

**3. Verdict:**

**4. Reasoning:** 

**5. Student Fix:**

### Artifact 2: 
**1. Prompt + Tool**
- **Tool:** Gemini 3.5 Flash (Antigravity)
- **Timestamp:** 13:25 28/07/2026
- **Prompt:**
```text
[Main_Report.md](file;file:///d:/DaiHoc/KiemThuPM/HW03/Main_Report.md) 
Bây giờ trong Part B:  Execution on Scenario, ở phần **C1 - Users list — Search, Role/Active Filters, Columns:**.
với từng cột Fail, bạn hãy điền giúp tôi các Notes, cũng như generate ra "Bug & Usability Findings Log — and include 
it in your submission. The log must consolidate everything you sent to the form, with at least 
these columns: ID · Scenario/Screen · Type (Bug | Usability) · Description · Steps/Heuristic · 
Severity · Suggested fix · Screenshot ref · Form-submission timestamp"

- IA-01-04: Fail do khi nhập trường email trong "tạo người dùng mới" ,mặc dù để là tiếng Việt như lỗi trả về (khi chỉ nhập trường email là "a") thì lại để là "Please include an '@' in the email address. 'a' is missing a '@'.", còn lại các trường khác (nếu có báo lỗi) thì là tiếng Việt bình thường.
- IA-02-01: Fail do một số trường trong form" tạo người dùng mới" không có dấu '*' nhưng khi ấn Create User thì lại trở thành "Last name is required", "First name is required", "Role is required"...
- IA-02-03: Sau khi ấn submit thì mới hiện lỗi, trong khi đó nếu trường email chỉ có nội dung "a" thì không hiện gì cả (trước đó không bấm gì hết)
- IA-02-08: Khi bỏ trống email, để phone number là "a", nút "Create User" không bị vô hiệu hóa hay bôi đen và có thể bấm (sau đó báo lỗi)
- IA-04-01: Sau khi tạo user mới hợp lệ, không có toast nào hiển thị là đã tạo thành công cả.
- IA-04-09: Khi mở 2 tab admin kế cạnh nhau, sau khi chỉnh sửa tên của 1 user, chỉ có tab Admin chỉnh sửa trực tiếp là thay đổi (đổi từ def abc sang B A), tab Admin còn lại user đó vẫn để tên cũ (def abc)
- IA-04-10: Sau khi điền đầy đủ thông tin để tạo User mới, khi nhấn Create User mà bị mất kết nối mạng đột ngột thì chỉ hiện dòng lỗi "Failed to fetch" tối nghĩa trong form tạo user.
- Functional Bug 1: Nếu nhập nội dung vào thanh "search users" quá nhanh, đôi lúc sẽ không tìm được user mặc dù user đó có tồn tại trong hệ thống (trong ảnh là tôi kiếm "Tôi là Admin", nhưng khi nhập "Tôi là" rất nhanh hoặc nhập sẵn "Tôi l" và nhập chữ "à" nhanh - không phải copy chữ, thì nó lại không hiện gì, nhưng khi nhập từ tốn, thì lại hiện ra)
```

**2. AI Output:**
```text
AI đã cập nhật lỗi thực tế vào cột Notes của bảng C1 trong Main_Report.md, thêm phần Task 4 (Bug & Usability Findings Log) và tạo riêng file Bug_Usability_Findings_Log.md với đầy đủ cột theo yêu cầu để nộp.
```

**3. Verdict:**

**4. Reasoning:** 

**5. Student Fix:**

### Artifact 3: 
**1. Prompt + Tool**
- **Tool:** Gemini 3.5 Flash (Antigravity)
- **Timestamp:** 13:49 - 13:51 28/07/2026
- **Prompt:**
```text
Screen của tôi hiện tại chỉ là "- C1 - Users list — search, role/active filters, columns", nhưng tôi đã lỡ làm luôn cả tính năng create user trong đây, giờ tôi nên làm gì?
```

```text
Bạn hãy làm phương án 1, chuyển qua bảng C2
```

**2. AI Output:**
```text
AI đề xuất chuyển các lỗi liên quan đến việc điền form (Tạo mới/Chỉnh sửa User) từ màn hình C1 sang C2 để đảm bảo logic. AI đã tự động cập nhật lại tên C2 và di chuyển các tiêu chí tương ứng sang C2 trong cả báo cáo chính và log lỗi.
```

**3. Verdict:**

**4. Reasoning:** 

**5. Student Fix:**

### Artifact 4: 
**1. Prompt + Tool**
- **Tool:** Gemini 3.5 Flash (Antigravity)
- **Timestamp:** 14:20 28/07/2026
- **Prompt:**
```text
[Main_Report.md](file;file:///d:/DaiHoc/KiemThuPM/HW03/Main_Report.md) 
Hiện tại thì tại C1 vẫn còn 1 số lỗi
- IA-01-04: Khi nhập các giá trị không hợp lệ và để ngôn ngữ là tiếng Việt(ví dụ chỉ có 10 trang, nhập 11 thì thay vì báo bằng tiếng Việt, nó ghi ra "Value must be less than or equal to 10." và nhập -1 thì "Value must be greater than or equal to 1.
"
- Functional Bug 2: Khi nhập "Nguyễn Hoàng" vòa thanh Search User, nó hoạt động đúng và lọc ra những người có "nguyễn hoàng" trong họ tên, nhưng khi nhập đầy đủ "Nguyễn Hoàng Kỳ", không có gì hiện rra cả
```

**2. AI Output:**
```text
AI đã cập nhật lỗi đa ngôn ngữ (IA-01-04) và lỗi tìm kiếm (Functional Bug 2) vào bảng C1 trong báo cáo chính, đồng thời thêm chúng vào file Bug_Usability_Findings_Log.md kèm mô tả, độ nghiêm trọng và gợi ý sửa chữa.
```

**3. Verdict:**

**4. Reasoning:** 

**5. Student Fix:**

### Artifact 5: 
**1. Prompt + Tool**
- **Tool:** Gemini 3.5 Flash (Antigravity)
- **Timestamp:** 15:09 28/07/2026
- **Prompt:**
````text
Tôi có tìm thêm 4 lỗi nữa, bạn hãy bổ sung giúp tôi.
Trong C1 - Users list — Search, Role/Active Filters, Columns
- IA-01-07: Sidebar không tự động co giãn (thu lại) khi kéo nhỏ màn hình, từ đó khiến cho các cột bảng bị che khuất, không thấy được (nếu thu lại sidebar sẽ thấy được)
Trong C2 - Create / Edit User & Assign Role:

- IA-01-07: Khi trên màn hình nhỏ (như điện thoại), form Create User bị thu nhỏ tới mức khó nhìn thấy và bấm vào các trường của form
- IA-02-02: Hiện tại trong form, trường First Name có placeholder là Last name, trường Last name có placeholder là First name
- IA-02-04: Khi người dùng nhập "abc@abccom" vào trường Email, thay vì nói rõ người dùng đang thiếu tên miền (domain) thì lại ghi chung chung chỉ là "Invalid email address"
```

**2. AI Output:**
```text
AI đã bổ sung thêm 4 lỗi về hiển thị (Sidebar, co giãn form trên mobile) và trải nghiệm (Placeholder, Error message) vào cả bảng C1, C2 trong Main_Report.md và tạo mã lỗi tương ứng trong Bug_Usability_Findings_Log.md kèm gợi ý tên ảnh chụp.
```

**3. Verdict:**

**4. Reasoning:** 

**5. Student Fix:**

### Artifact 6: 
**1. Prompt + Tool**
- **Tool:** Gemini 3.5 Flash (Antigravity)
- **Timestamp:** 22:21 28/07/2026
- **Prompt:**
```text
Tôi đã đổi vị trí C3, C4. Cũng như tìm ra 6 lỗi ở phần C3, bạn hãy điền giúp tôi [Main_Report.md](file;file:///d:/DaiHoc/KiemThuPM/HW03/Main_Report.md) , [Bug_Usability_Findings_Log.md](file;file:///d:/DaiHoc/KiemThuPM/HW03/Bug_Usability_Findings_Log.md) :
- Functional Bug 1: Khi export file và nội dung file lên, thay vì nội dung của file hiện lên thì lại là dòng thông báo lỗi: "We found a problem with some content in 'users-export-...'. Do you want us to try to recover as much as we can? If you trust the source of this workbook, click Yes." và thông báo đã Repairs thành công sau khi ấn Yes.
- Functional Bug 2: Hiện tại trong nội dung file, đề mục column Card Code đang bị viết sai (đúng phải để là Member Code để đồng nhất với nội dung trong C-1 và C-2)
- IA-01-04: Nội dung, format của file export excel hiện tại chỉ cố định bằng tiếng Anh (Last Name, First Name, Email, Phone, Card Code...), không có cách hay phương thức nào để chuyển đổi sang tiếng Việt.
- IA-02-09: Hiện tại mục column Created At đang để đúng định dạng format dễ đọc, chuẩn Việt Nam (dd/mm/yyyy giờ:phút), nhưng ngay dưới đề mục USER REPORT lại để nội dung là: "Export date: 7/28/2026 | Exporter: Admin Tôi là" (theo định dạng m/d/yyyy).
- IA-04-01: Sau khi export và tải file thành công về, trang hiển thị hiện tại không có bất kỳ toast gì về việc đã export và lưu file thành công.
- IA-04-10: Khi đang bị mất internet và ấn nút Export (Xuất), hệ thống không có thông báo hay toast thông báo lỗi cho người dùng (sau khi nhấn không có gì xảy ra cả)
```

**2. AI Output:**
```text
AI đã ghi nhận 6 lỗi của chức năng Xuất Excel (màn hình C3), bao gồm lỗi hỏng file (Repair), định dạng ngày giờ, đa ngôn ngữ, mất kết nối mạng và thiếu thông báo. Cả file báo cáo chính và file log lỗi đều đã được cập nhật.
```

**3. Verdict:**

**4. Reasoning:** 

**5. Student Fix:**

### Artifact 7: 
**1. Prompt + Tool**
- **Tool:** Gemini 3.1 Pro (Antigravity)
- **Timestamp:** 15:32 29/07/2026
- **Prompt:**
```text
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
```

**2. AI Output:**
```text
AI đã dùng Agent tự động duyệt web để kiểm thử màn hình C4. Kết quả C4 đạt điểm Pass hoàn hảo ở các tiêu chí đa ngôn ngữ, màu cảnh báo, định dạng ngày và đóng hộp thoại. AI đã cập nhật kết quả vào báo cáo và tạo file Bug_C4.md.
```

**3. Verdict:**

**4. Reasoning:** 

**5. Student Fix:**

### Artifact 8: 
**1. Prompt + Tool**
- **Tool:** Gemini 3.5 Flash (Antigravity)
- **Timestamp:** 1:06 30/07/2026
- **Prompt:**
```text
Không hẳn là không có lỗi đâu, tôi đã tìm thấy được 3 lỗi của phần C4
- IA-01-07: Khi sử dụng các thiết bị như iPhone SE, hay iPhone bằng devtool trên web hoặc cửa số đủ nhỏ, bản thân giao diện user management đã bị hỏng (mất hết các cột, khó chọn) và đồng thời còn bị 1 vấn đề là tôi phải kéo màn hình để di chuyển đến nội dung dialog hiện lên (delete user dialog)
- IA-04-01: Sau khi xóa không có toast hay thông báo để cho người dùng biết là đã xóa thành công user rồi
- IA-04-10: Khi mất internet, vẫn có thể bấm vào nút delete (thùng rác) để mở dialog xóa user, nhưng nó bị 1 vấn đề là khi bấm Xác nhận, không có gì xyả ra cả, không có thông báo cũng như toast hay gì hiện lên
```

**2. AI Output:**
```text
AI đã ghi nhận thêm 3 lỗi Usability mới của màn hình C4 (lỗi vỡ layout trên thiết bị nhỏ, không có toast khi xóa và không phản hồi khi mất mạng). File Bug_C4.md, log lỗi và báo cáo chính đã được cập nhật từ Pass sang Fail.
```

**3. Verdict:**

**4. Reasoning:** 

**5. Student Fix:**

### Artifact 9: 
**1. Prompt + Tool**
- **Tool:** Gemini 3.5 Flash (Antigravity)
- **Timestamp:** 15:42 30/07/2026
- **Prompt:**
```text
Bạn hãy generate giúp tôi bảng ở Task 3 cho gọn gàng và bao trọn hết 4 screen với (3 operating systems — e.g. Windows, macOS, and Android or iOS, 5 browsers — e.g. Chrome, Firefox, Safari, Edge, and Opera (or Samsung Internet on 
mobile), 3 device classes — desktop, tablet, and phone). Phần kết quả hãy để tôi điền (để trống)
```

**2. AI Output:**
```text
AI đã tạo ma trận tương thích cho Task 3 (Cross-Browser/Platform) gồm 4 bảng ứng với 4 màn hình, bao quát đủ 3 hệ điều hành, 3 loại thiết bị và 5 trình duyệt để sinh viên điền kết quả.
```

**3. Verdict:**

**4. Reasoning:** 

**5. Student Fix:**

### Artifact 10: 
**1. Prompt + Tool**
- **Tool:** Gemini 3.5 Flash (Antigravity)
- **Timestamp:** 16:47 30/07/2026
- **Prompt:**
```text
Bạn hãy giúp tôi điều chỉnh lại đường link ảnh, hiện tại thay vì vào thẳng images/tên file ảnh. Thì giờ tôi dời vào thêm 1 folder nữa (thành images/bug-defect/tên file ảnh)
```

**2. AI Output:**
```text
AI đã dùng script Python tự động cập nhật hàng loạt đường dẫn hình ảnh của các lỗi (bugs) trong Bug_C4.md và Bug_Usability_Findings_Log.md sang thư mục mới `images/bug-defect/`.
```

**3. Verdict:**

**4. Reasoning:** 

**5. Student Fix:**

### Artifact 11: 
**1. Prompt + Tool**
- **Tool:** Gemini 3.1 Pro (Antigravity)
- **Timestamp:** 15:22 31/07/2026
- **Prompt:**
```text
Bạn hãy viết khung sườn cho phần Task 2 Scenario C — Admin manages users (Function group: user administration).

Bao gồm các Screen:
- C1 - Users List — Search, Role/Active Filters, Columns
- C2 - Create / Edit User & Assign Role
- C3 - Export to Excel — Column Completeness and Download Feedback
- C4 - Delete User Confirmation Dialog & Audit Logs
```

**2. AI Output:**
```text
AI đã tạo khung sườn cho Task 2 (Usability Testing) và chèn vào Main_Report.md. Khung này bao gồm kịch bản thử nghiệm hướng mục tiêu, 10 câu hỏi SUS tiếng Việt và các bảng trống cho người tham gia, số liệu và lỗi.
```

**3. Verdict:**

**4. Reasoning:** 

**5. Student Fix:**

### Artifact 12: 
**1. Prompt + Tool**
- **Tool:** Gemini 3.5 Flash (Antigravity)
- **Timestamp:** 21:07 01/08/2026
- **Prompt:**
```text
Bạn hãy generate giúp tôi 1 file riêng có kịch bản để cho người dùng E2E đọc (1 file .md tôi sẽ tự xuất pdf sau)
```

**2. AI Output:**
```text
AI đã sinh riêng file Usability_Testing_Scenario.md với định dạng rõ ràng, lịch sự để làm hướng dẫn kiểm thử cho 5 người tham gia, bao gồm kịch bản thực hành và bảng đánh giá SUS.
```

**3. Verdict:**

**4. Reasoning:** 

**5. Student Fix:**