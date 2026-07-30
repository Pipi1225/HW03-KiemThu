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
Viewed shared_gui_checklist.md:1-58
Created Report_ScenarioC_Template.md

Lựa chọn **Scenario C (Admin manages users) với 4 screens** là một quyết định rất chuẩn xác vì nó bao phủ trọn vẹn luồng công việc của một Quản trị viên. 

Dựa trên yêu cầu của đề bài, 4 màn hình (screens) thuộc Scenario C của bạn sẽ là:
1. **(C1) Users list:** Giao diện xem danh sách, bộ lọc tìm kiếm, bộ lọc role/active.
2. **(C2) Assign Role / edit user:** Giao diện/Form cấp quyền và chỉnh sửa người dùng.
3. **(C3) Block-Unblock and Reset-Password:** Các hộp thoại (dialogs) xác nhận khóa/mở khóa và đổi mật khẩu.
4. **(C4) Export to Excel:** Chức năng xuất file Excel và các thông báo trạng thái tải xuống.

Để giúp bạn tiết kiệm thời gian, tôi đã tạo sẵn một file Template Báo Cáo định dạng Markdown chứa khung sườn cho cả 3 Task (1B, 2, 3) tại đây: [Report_ScenarioC_Template.md](file:///d:/DaiHoc/KiemThuPM/HW03/Report_ScenarioC_Template.md).

Dưới đây là hướng dẫn chi tiết cách bạn cần tiến hành các bước tiếp theo:

### 🎯 Task 1B: Thực thi GUI Checklist (Tự làm)
1. Truy cập vào đường link SUT (ngrok URL) được cung cấp trong đề.
2. **Đăng nhập bằng tài khoản Admin:** `admin@gmail.com` / `Admin@123`.
3. Mở file [shared_gui_checklist.md](file:///d:/DaiHoc/KiemThuPM/HW03/shared_gui_checklist.md) của nhóm lên. Lần lượt đi qua 4 màn hình (C1 -> C4) và chấm điểm **Pass / Fail / N/A** cho từng tiêu chí.
4. Chụp lại màn hình với những mục bị **Fail** và ghi chú lý do. (Ví dụ: Chữ bị vỡ khi xem trên màn hình nhỏ, hoặc không có xác nhận khi xóa).
5. Đưa các lỗi này vào file log chung của nhóm và điền Google Form.

### 👥 Task 2: Kiểm thử tính khả dụng (Usability Testing)
Tôi đã giúp bạn thiết kế kịch bản hướng mục tiêu (Goal-oriented) trong file Template. Bạn hãy đưa kịch bản này cho 5 người dùng thực tế thực hiện:

> **Kịch bản cho người test:**
> *"Bạn là quản trị viên hệ thống của khoa. Hãy tìm kiếm một người dùng tên là 'Nguyen Van A' (hoặc một tên cụ thể có trong hệ thống) trong danh sách. Hãy cấp quyền 'Lecturer' cho người này. Sau đó, hãy thử khóa (block) tài khoản của họ và cuối cùng là xuất danh sách toàn bộ người dùng ra file Excel để báo cáo."*

**Lưu ý khi test:** 
- Bạn chỉ quan sát họ làm, không hướng dẫn click ở đâu.
- Yêu cầu họ "think aloud" (nghĩ gì nói nấy). Ví dụ họ phàn nàn: *"Sao cái nút lọc quyền khó tìm thế nhỉ?"* -> Ghi chú ngay lại, đó chính là 1 lỗi Usability.
- Cuối cùng, cho họ chấm điểm SUS (hoặc UEQ-S).

### 📱 Task 3: Test Đa nền tảng (Cross-Browser / Cross-Platform)
Mục tiêu là kiểm tra xem 4 màn hình trên có bị lỗi hiển thị (tràn viền, vỡ nút...) trên các thiết bị khác nhau không. Bạn hãy dùng **BrowserStack** hoặc **LambdaTest** để làm.
- Cần có ít nhất **3 Hệ điều hành** (VD: Windows, macOS, Android).
- Cần có ít nhất **5 Trình duyệt** (VD: Chrome, Safari, Edge, Firefox, Opera).
- Cần đủ **3 Loại thiết bị** (Desktop, Tablet, Phone).

> **⚠️ BẮT BUỘC:** Đừng quên chèn watermark dạng `MSSV@....edu.vn` của bạn vào ảnh chụp màn hình đa nền tảng để tránh bị trừ 0 điểm.

Bạn đã cài đặt và tạo tài khoản BrowserStack/LambdaTest chưa? Nếu bạn cần, tôi có thể hướng dẫn cách kết hợp các tổ hợp thiết bị sao cho tối ưu nhất (ít phải test nhất mà vẫn đủ điều kiện).
```

**3. Verdict:**

**4. Reasoning:** 

**5. Student Fix:**

### Artifact 2: 
**1. Prompt + Tool**
- **Tool:** Gemini 3.5 Flash (Antigravity)
- **Timestamp:** 20:50 26/07/2026
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

**3. Verdict:**

**4. Reasoning:** 

**5. Student Fix:**

### Artifact 3: 
**1. Prompt + Tool**
- **Tool:** Gemini 3.5 Flash (Antigravity)
- **Timestamp:** 13:51 28/07/2026
- **Prompt:**
```text
Screen của tôi hiện tại chỉ là "- C1 - Users list — search, role/active filters, columns", nhưng tôi đã lỡ làm luôn cả tính năng create user trong đây, giờ tôi nên làm gì?
```

```text
Bạn hãy làm phương án 1, chuyển qua bảng C2
```

**2. AI Output:**

**3. Verdict:**

**4. Reasoning:** 

**5. Student Fix:**

### Artifact 4: 
**1. Prompt + Tool**
- **Tool:** Gemini 3.5 Flash
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
Viewed Main_Report.md:310-330
Edited Main_Report.md
Viewed Main_Report.md:75-90
Edited Main_Report.md
Created Bug_Usability_Findings_Log.md

Tôi đã thực hiện cập nhật thêm các lỗi mới bạn vừa phát hiện vào cả báo cáo chính lẫn file log lỗi:

### 1. Cập nhật trong file báo cáo chính ([Main_Report.md](file:///d:/DaiHoc/KiemThuPM/HW03/Main_Report.md))
*   **Bảng C1 - Tiêu chí `IA-01-04`:** Đã chuyển lại từ `Pass` thành `Fail` kèm ghi chú mô tả lỗi thực tế: Khi nhập số trang sai định dạng trong ô "Đến trang" (ví dụ nhập 11/10 hoặc nhập -1) lúc giao diện đang ở tiếng Việt, trình duyệt hiển thị thông báo lỗi hoàn toàn bằng tiếng Anh (`Value must be...`).
*   **Bổ sung 2 lỗi mới vào bảng Task 4:**
    *   `BUG-C1-03`: Lỗi hiển thị đa ngôn ngữ (i18n) cho thông báo validation ở ô nhập số trang phân trang (`IA-01-04`).
    *   `BUG-C1-04` (Functional Bug 2): Lỗi tìm kiếm không chính xác khi gõ đầy đủ họ và tên của user (ví dụ: tìm "Nguyễn Hoàng Kỳ" bị lỗi rỗng, trong khi tìm "Nguyễn Hoàng" thì bình thường).

### 2. Cập nhật trong file log lỗi độc lập ([Bug_Usability_Findings_Log.md](file:///d:/DaiHoc/KiemThuPM/HW03/Bug_Usability_Findings_Log.md))
*   Đã thêm 2 lỗi `BUG-C1-03` và `BUG-C1-04` với đầy đủ các cột thông tin: Mô tả chi tiết lỗi, các bước tái hiện, độ nghiêm trọng đề xuất (Severity), hướng sửa đổi (Suggested fix) và tên ảnh chụp màn hình tương ứng.

Các lỗi này đều rất thực tế và có tính thuyết phục cao đối với giảng viên khi chấm điểm kiểm thử giao diện & độ khả dụng.

Bạn có muốn tiếp tục hoàn thiện phần nào khác không, ví dụ như đề xuất ma trận tương thích cho **Task 3** hoặc viết báo cáo kiểm thử người dùng **Task 2**?
```

**3. Verdict:**

**4. Reasoning:** 

**5. Student Fix:**

### Artifact 5: 
**1. Prompt + Tool**
- **Tool:** Gemini 3.5 Flash
- **Timestamp:** 09:14 30/06/2026
- **Prompt:**

**2. AI Output:**

**3. Verdict:**

**4. Reasoning:** 

**5. Student Fix:**

### Artifact 6: 
**1. Prompt + Tool**
- **Tool:** 
- **Timestamp:** 09:14 30/06/2026
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
Viewed Main_Report.md:75-110
Edited Main_Report.md
Viewed Main_Report.md:137-165
Edited Main_Report.md
Created Bug_Usability_Findings_Log.md

Tôi đã bổ sung thành công 4 lỗi mới vào cả hai tài liệu kiểm thử của bạn:

### 1. Cập nhật trong báo cáo chính ([Main_Report.md](file:///d:/DaiHoc/KiemThuPM/HW03/Main_Report.md))
*   **Bảng C1 (Users List):** Tiêu chí `IA-01-07` (Responsive) đã được sửa thành `Fail` kèm ghi chú về việc sidebar không tự động thu gọn khi thu nhỏ màn hình khiến các cột dữ liệu của bảng bị che khuất.
*   **Bảng C2 (Create / Edit User):**
    *   Tiêu chí `IA-01-07` (Responsive) sửa thành `Fail`: Lỗi form hiển thị quá bé và khó thao tác trên giao diện mobile (zoom out quá mức).
    *   Tiêu chí `IA-02-02` (Labels & Placeholders) sửa thành `Fail`: Lỗi hoán đổi placeholder gợi ý của trường First Name và Last Name cho nhau.
    *   Tiêu chí `IA-02-04` (Error messages) sửa thành `Fail`: Lỗi thông báo quá chung chung `"Invalid email address"` khi người dùng gõ thiếu đuôi tên miền (như `"abc@abccom"`).

### 2. Cập nhật trong file log lỗi độc lập ([Bug_Usability_Findings_Log.md](file:///d:/DaiHoc/KiemThuPM/HW03/Bug_Usability_Findings_Log.md))
Tôi đã thêm 4 dòng lỗi này vào bảng log với các mã định danh tương ứng và đề xuất sẵn tên file ảnh nhúng để bạn tiện lưu trữ trong folder `images`:
*   `BUG-C1-05` (Lỗi sidebar): Đặt tên ảnh là `Screen-C1-IA-01-07.jpg`.
*   `BUG-C2-07` (Lỗi co giãn form trên mobile): Đặt tên ảnh là `Screen-C2-IA-01-07.jpg`.
*   `BUG-C2-08` (Lỗi tráo đổi placeholder): Đặt tên ảnh là `Screen-C2-IA-02-02.jpg`.
*   `BUG-C2-09` (Lỗi email không rõ ràng): Đặt tên ảnh là `Screen-C2-IA-02-04.jpg`.

*Mẹo: Bạn chỉ cần chụp màn hình 4 lỗi này trên SUT, đặt tên theo gợi ý trên rồi lưu vào thư mục `images` là file log sẽ tự động tải và hiển thị ảnh cực kỳ đẹp mắt khi xuất ra file nộp.*

Bạn có cần hỗ trợ hoàn thiện nốt phần nào khác cho báo cáo (ví dụ: Task 3 - Cross Platform, hay Task 11 - AI Critique) không?
````

**3. Verdict:**

**4. Reasoning:** 

**5. Student Fix:**

### Artifact 7: 
**1. Prompt + Tool**
- **Tool:**
- **Timestamp:** 09:14 30/06/2026
- **Prompt:**

**2. AI Output:**

**3. Verdict:**

**4. Reasoning:** 

**5. Student Fix:**

### Artifact 8: 
**1. Prompt + Tool**
- **Tool:**
- **Timestamp:** 09:14 30/06/2026
- **Prompt:**

**2. AI Output:**

**3. Verdict:**

**4. Reasoning:** 

**5. Student Fix:**

### Artifact 9: 
**1. Prompt + Tool**
- **Tool:**
- **Timestamp:** 09:14 30/06/2026
- **Prompt:**

**2. AI Output:**

**3. Verdict:**

**4. Reasoning:** 

**5. Student Fix:**

### Artifact 10: 
**1. Prompt + Tool**
- **Tool:**
- **Timestamp:** 09:14 30/06/2026
- **Prompt:**

**2. AI Output:**

**3. Verdict:**

**4. Reasoning:** 

**5. Student Fix:**

### Artifact 11: 
**1. Prompt + Tool**
- **Tool:**
- **Timestamp:** 09:14 30/06/2026
- **Prompt:**

**2. AI Output:**

**3. Verdict:**

**4. Reasoning:** 

**5. Student Fix:**

### Artifact 12: 
**1. Prompt + Tool**
- **Tool:**
- **Timestamp:** 09:14 30/06/2026
- **Prompt:**

**2. AI Output:**

**3. Verdict:**

**4. Reasoning:** 

**5. Student Fix:**

### Artifact 13: 
**1. Prompt + Tool**
- **Tool:**
- **Timestamp:** 09:14 30/06/2026
- **Prompt:**

**2. AI Output:**

**3. Verdict:**

**4. Reasoning:** 

**5. Student Fix:**

### Artifact 14: 
**1. Prompt + Tool**
- **Tool:**
- **Timestamp:** 09:14 30/06/2026
- **Prompt:**

**2. AI Output:**

**3. Verdict:**

**4. Reasoning:** 

**5. Student Fix:**

### Artifact 15: 
**1. Prompt + Tool**
- **Tool:**
- **Timestamp:** 09:14 30/06/2026
- **Prompt:**

**2. AI Output:**

**3. Verdict:**

**4. Reasoning:** 

**5. Student Fix:**

### Artifact 16: 
**1. Prompt + Tool**
- **Tool:**
- **Timestamp:** 09:14 30/06/2026
- **Prompt:**

**2. AI Output:**

**3. Verdict:**

**4. Reasoning:** 

**5. Student Fix:**

### Artifact 17: 
**1. Prompt + Tool**
- **Tool:**
- **Timestamp:** 09:14 30/06/2026
- **Prompt:**

**2. AI Output:**

**3. Verdict:**

**4. Reasoning:** 

**5. Student Fix:**

### Artifact 18: 
**1. Prompt + Tool**
- **Tool:**
- **Timestamp:** 09:14 30/06/2026
- **Prompt:**

**2. AI Output:**

**3. Verdict:**

**4. Reasoning:** 

**5. Student Fix:**

### Artifact 19: 
**1. Prompt + Tool**
- **Tool:**
- **Timestamp:** 09:14 30/06/2026
- **Prompt:**

**2. AI Output:**

**3. Verdict:**

**4. Reasoning:** 

**5. Student Fix:**

### Artifact 20: 
**1. Prompt + Tool**
- **Tool:**
- **Timestamp:** 09:14 30/06/2026
- **Prompt:**

**2. AI Output:**

**3. Verdict:**

**4. Reasoning:** 

**5. Student Fix:**