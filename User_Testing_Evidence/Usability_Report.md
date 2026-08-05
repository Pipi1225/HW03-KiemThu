# Usability Testing Report

## 1. Kịch Bản Kiểm Thử (Task Scenario)

**Mục tiêu:** Đánh giá mức độ dễ dàng và tính thân thiện của hệ thống đối với người quản trị (Admin) khi thực hiện các nghiệp vụ quản lý người dùng (C1, C2, C3, C4).

### Bối cảnh nghiệp vụ
Mỗi tài khoản trong hệ thống có 4 vai trò bao gồm:
1. Quản trị - Admin
2. Khách - Guest
3. Giảng viên - Lecturer
4. Sinh viên - Student 

Và 2 trạng thái bao gồm:
1. Hoạt động - Active
2. Không hoạt động - Inactive

### Kịch bản (Dành cho người tham gia)
"Bạn là một quản trị viên (Admin) của hệ thống quản lý sự kiện. Nhiệm vụ của bạn là sử dụng hệ thống để quản lý tài khoản người dùng với các công việc sau:
- Tìm kiếm, lọc và xem thông tin trên danh sách người dùng.
- Tạo một người dùng mới và phân quyền cho người đó.
- Xuất danh sách người dùng hiện tại ra file Excel để lưu trữ báo cáo.
- Tìm và xóa một người dùng không còn hoạt động, sau đó xác nhận hoàn tất thao tác xóa."

*(Lưu ý: Chỉ đưa ra kịch bản và mục tiêu để người dùng tự khám phá, không hướng dẫn chi tiết từng bước click chuột vào đâu).*

---

## 2. Bảng Câu Hỏi SUS (SUS Questionare)

*Thang điểm đánh giá: 1 (Hoàn toàn không đồng ý) đến 5 (Hoàn toàn đồng ý)*

1. Tôi nghĩ rằng tôi sẽ muốn sử dụng hệ thống này thường xuyên.
2. Tôi thấy hệ thống này phức tạp một cách không cần thiết.
3. Tôi thấy hệ thống này dễ sử dụng.
4. Tôi nghĩ rằng tôi sẽ cần sự hỗ trợ của người am hiểu kỹ thuật để có thể sử dụng hệ thống này.
5. Tôi thấy các chức năng trong hệ thống này được tích hợp rất tốt.
6. Tôi thấy có quá nhiều sự không nhất quán trong hệ thống này.
7. Tôi có thể hình dung được rằng hầu hết mọi người sẽ học được cách sử dụng hệ thống này rất nhanh.
8. Tôi thấy hệ thống này rất rườm rà và khó sử dụng.
9. Tôi cảm thấy rất tự tin khi sử dụng hệ thống này.
10. Tôi cần phải học rất nhiều điều trước khi có thể bắt đầu sử dụng hệ thống này.

Đường link Google Form để người tham gia điền câu trả lời:
[https://forms.gle/1qjnsDcQQWjxswBY7](https://forms.gle/1qjnsDcQQWjxswBY7)

---

## 3. Báo Cáo Kết Quả Kiểm Thử

### 3.1. Danh sách người tham gia (Participants)

| STT | Họ và tên | Đối tượng (Role) | Thông tin liên hệ |
|---|---|---|---|
| 1 | Nguyễn Tấn Đạt | Sinh viên năm 3 | 033xxxx851 |
| 2 | Nguyễn Thị Cẩm Nhung | Developer (tương tác nhiều với công nghệ) | 090xxxx048 |
| 3 | Nguyễn Tuấn Kiệt | Sinh viên năm 1 | 033xxxx507 |
| 4 | Dương Thúy Mi | Giáo viên | 093xxxx202 |

---

### 3.2. Bảng số liệu kiểm thử (Metrics Table)

*Chú thích định nghĩa **Task Success Rate** cho từng mức độ:*
- **Thành công (Success):** Người dùng tự hoàn thành toàn bộ kịch bản mà không cần bất kỳ sự can thiệp hay chỉ dẫn nào.
- **Một phần (Partial Success):** Người dùng hoàn thành phần lớn kịch bản nhưng cần gợi ý/trợ giúp khi gặp điểm nghẽn, hoặc chỉ làm được một số tác vụ.
- **Thất bại (Failure):** Người dùng bỏ cuộc, hết thời gian (time-out), hoặc đi sai hướng hoàn toàn không thể phục hồi.

| STT | Task Success Rate<br>(Thành công / Một phần / Thất bại) | Thời gian hoàn thành<br>(Phút:Giây) | Số lỗi & Tần suất ngập ngừng<br>(Error & Hesitation Count) | Điểm SUS<br>(SUS Score) | Ghi chú / Điểm nghẽn |
|---|---|---|---|---|---|
| 1 | Một phần | 6:39 | 3 | 100 | File Excel lỗi cấu trúc bắt Repair, không tìm kiếm được user theo họ tên đầy đủ, form tạo user thiếu điều kiện Password bắt buộc từ đầu. |
| 2 | Một phần | 6:40 | 4 | 90 | Tìm kiếm đầy đủ họ tên không ra kết quả, lỗi pagination/lọc chữ viết thường, form tạo user thiếu điều kiện mật khẩu từ đầu. |
| 3 | Một phần | 6:52 | 4 | 87.5 | Khó định vị bộ lọc Role/Status, form tạo user validate lần lượt từng trường (phải bấm submit 3 lần mới xong SĐT/mật khẩu), không thấy nút bỏ lọc Role. |
| 4 | Một phần | 3:49 | 3 | 97.5 | Không thấy nút active/unactive để chỉnh sửa trạng thái, không thấy nút bỏ lọc Role, form tạo user thiếu toast/loading phản hồi ngay. |
| **Trung bình** | - | 6:00 | 3.5 | 93.75 | Hầu hết người dùng gặp điểm nghẽn nghiêm trọng ở file Excel hỏng, chức năng Tìm kiếm/Phân trang và tính năng validation/phản hồi của Form tạo user. |

---

### 3.3. Chi tiết câu hỏi SUS và Cách tính điểm (SUS Scoring Details)

Dưới đây là bảng ghi nhận điểm số trả lời (từ 1 đến 5) của từng người tham gia đối với 10 câu hỏi SUS và kết quả quy đổi điểm:
- **Câu lẻ (1, 3, 5, 7, 9):** `Điểm quy đổi = Điểm trả lời - 1`
- **Câu chẵn (2, 4, 6, 8, 10):** `Điểm quy đổi = 5 - Điểm trả lời`
- **Điểm SUS cá nhân:** `(Tổng điểm quy đổi của 10 câu) * 2.5`

| Người tham gia | Q1 | Q2 | Q3 | Q4 | Q5 | Q6 | Q7 | Q8 | Q9 | Q10 | Tổng điểm quy đổi | Điểm SUS (Tổng * 2.5) |
|---|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| **Người 1** | 5 | 1 | 5 | 1 | 5 | 1 | 5 | 1 | 5 | 1 | 40 | 100 |
| **Người 2** | 4 | 1 | 5 | 2 | 5 | 1 | 5 | 1 | 4 | 2 | 36 | 90 |
| **Người 3** | 4 | 1 | 4 | 2 | 5 | 1 | 5 | 1 | 4 | 2 | 35 | 87.5 |
| **Người 4** | 5 | 1 | 5 | 1 | 4 | 1 | 5 | 1 | 5 | 1 | 39 | 97.5 |
| **Trung bình** | - | - | - | - | - | - | - | - | - | - | - | **93.75** |

---

### 3.4. Nhật ký quan sát chi tiết từng phiên (Per-Session Observation Notes)

#### Phiên kiểm thử số 1: Nguyễn Tấn Đạt
- **Thời gian hoàn thành:** 6 phút 39 giây | **Số lỗi & Ngập ngừng:** 3 | **Điểm SUS:** 100
- **Nhật ký hành vi:**
  - 0:32 - 2:36 (Màn hình C1): Người dùng thử filter User theo Role và Status và tìm kiếm người dùng với từ khóa "Kỳ".
  - 2:38 - 5:10 (Màn hình C2): Người dùng tạo User mới với role là Student và thử tìm kiếm lại nhưng cần sự trợ giúp, sau đó đổi role User thành Lecturer.
  - 5:20 - 6:33 (Màn hình C3): Người dùng Export Excel danh sách về nhưng gặp khó khăn trong việc mở file và cần sự trợ giúp.
  - 6:38 - 7:06 (Màn hình C4): Người dùng xóa User mới tạo ở màn hình C2.

- **Khó khăn & Lỗi SUT bắt gặp theo từng nhiệm vụ:**
  - *Nhiệm vụ 1 (Khám phá & Tìm kiếm):* Không có
  - *Nhiệm vụ 2 (Thêm & Chỉnh sửa user):* 
    - Lúc 3:11 trong Video, thay vì hiện quy định Password ngay từ đầu thì phải ấn Create User rồi người dùng mới biết được định dạng Password bắt buộc ra sao.
    - Lúc 4:12 trong Video, tính năng tìm kiếm User không cho phép nhập toàn bộ họ và tên mà chỉ tìm được bằng họ hoặc bằng tên (A Nguyen), phải có sự trợ giúp mới tìm được User đã tạo.
  - *Nhiệm vụ 3 (Xuất báo cáo Excel):*
    - Lúc 5:36 trong Video, lúc Excel thông báo "We found a problem with some content in...", người dùng không biết nên xử lý ra sao vì thông báo này rất hiếm khi gặp.
  - *Nhiệm vụ 4 (Xóa user & Audit Log):* Không có

- **Phát biểu trực tiếp nổi bật (Think-aloud/Quotes):**
  - *"Ồ, ủa tại sao kỳ quá ha"* - khi Search lại tài khoản vừa tạo

- **Probe Question:**
  - *Ý kiến đóng góp khác (Nếu có):* Không có

#### Phiên kiểm thử số 2: Nguyễn Thị Cẩm Nhung
- **Thời gian hoàn thành:** 6 phút 40 giây | **Số lỗi & Ngập ngừng:** 4 | **Điểm SUS:** 90
- **Nhật ký hành vi:**
  - 0:22 - 1:34 và 4:57 - 6:48  (Màn hình C1): Người dùng muốn thử xem chi tiết User nhưng không có tính năng đó trên SUT. Người dùng thử filter User theo Role. Người dùng để filter Role là Student, sau đó search thử từ khóa "hoàng" thì pagination nhảy liên tục và không đúng kết quả mong muốn và khi search "Hoàng" thì hoạt động đúng. Sau đó người dùng thử search từ khóa "kỳ" và "Kỳ" thì lỗi tương tự xảy ra (kể khi đã nhập từ từ từng ký tự). Người dùng phải chọn Pagination ở dưới bấm vài lần thì mới có kết quả đúng.
  - 1:37 - 3:48 (Màn hình C2): Người dùng tạo User mới với role là Student, sau đó tìm kiếm và đổi First name từ "Duc" thành "Tien".
  - 3:54 - 4:10 (Màn hình C3): Người dùng Export Excel danh sách về và mở file mượt mà.
  - 4:22 - 4:31 (Màn hình C4): Người dùng xóa tài khoản vừa tạo ở bước C2.

- **Khó khăn & Lỗi SUT bắt gặp theo từng nhiệm vụ:**
  - *Nhiệm vụ 1 (Khám phá & Tìm kiếm):*
    - Lúc 0:35 trong Video, người dùng muốn xem chi tiết User nhưng không thể vì SUT không cung cấp tính năng đó.
    - Lúc 5:20 trong Video, người dùng thử Search User bằng từ khóa "hoàng" thì kết quả xuất hiện lại là tên của các User không chứa chữ "hoàng".
  - *Nhiệm vụ 2 (Thêm & Chỉnh sửa user):* 
    - Lúc 1:44 trong Video, khi trỏ chuột vào nút Create User, con trỏ chuột không thay đổi, cũng như đối với các nút hành động khi Popup Modal hiện lên.
    - Lúc 2:46 trong Video, thay vì hiện quy định Password ngay từ đầu thì phải ấn Create User rồi người dùng mới biết được định dạng Password bắt buộc ra sao.
  - *Nhiệm vụ 3 (Xuất báo cáo Excel):* Không có
  - *Nhiệm vụ 4 (Xóa user & Audit Log):* Không có

- **Phát biểu trực tiếp nổi bật (Think-aloud/Quotes):**
  - *"Là sao mình phải bấm vô ở đây hả, làm sao để mình bấm vô được ta"*
  - *"Cái này là UX hơi confused chút xíu, mình tưởng bấm vô đây là coi được detail nhưng mình chỉ coi được danh sách này thôi"*
  - *"Chỗ Create User không có khiến cho con trỏ chuột thành dấu để bấm vô được"*
  - *"Tính năng Search chưa được hoàn thiện lắm"*
  - *"Mình phải Navigate 1 cái thì nó mới ra kết quả mình mong muốn, Paging, cái này xem lại"*

- **Probe Question:**
  - *Ý kiến đóng góp khác (Nếu có):* Cải thiện tính năng tìm kiếm

#### Phiên kiểm thử số 3: Nguyễn Tuấn Kiệt
- **Thời gian hoàn thành:** 6 phút 52 giây | **Số lỗi & Ngập ngừng:** 4 | **Điểm SUS:** 87.5
- **Nhật ký hành vi:**
  - 0:12 - 4:16 (Màn hình C1): Người dùng quyết định tạo User mới rồi mới tìm kiếm, sau đó người dùng tìm kiếm User bằng cách Search từ khóa "cẩm nhung" và filter Role là Guest.
  - 1:39 - 4:09 (Màn hình C2): Người dùng tạo User mới với role là Guest, sau đó tìm kiếm và đổi Role lại thành Admin.
  - 4:28 - 6:21 (Màn hình C3): Người dùng Export Excel danh sách về nhưng hơi lúng túng trong xử lý mở file.
  - 6:28 - 6:49 (Màn hình C4): Người dùng lọc các User có Status là Unactive và tiến hành xóa.

- **Khó khăn & Lỗi SUT bắt gặp theo từng nhiệm vụ:**
  - *Nhiệm vụ 1 (Khám phá & Tìm kiếm):*
    - Lúc 0:29 trong Video, người dùng muốn xem chi tiết User nhưng không thể vì SUT không cung cấp tính năng đó.
    - Lúc 3:25 trong Video, người dùng bối rối muốn tìm kiếm nút Filter Role và Status và cần sự trợ giúp.
  - *Nhiệm vụ 2 (Thêm & Chỉnh sửa user):*
    - Lúc 2:28 trong Video, thay vì hiện quy định Password và Phone Number ngay từ đầu thì phải ấn Create User rồi người dùng mới biết.
  - *Nhiệm vụ 3 (Xuất báo cáo Excel):*
    - Lúc 5:55 trong Video, người dùng không thấy/nhớ về việc bỏ Role (có thể do nút bỏ Role quá khó nhìn).
  - *Nhiệm vụ 4 (Xóa user & Audit Log):* Không có

- **Phát biểu trực tiếp nổi bật (Think-aloud/Quotes):**
  - *"Làm sao để đi vô khám phá chi tiết danh sách"*
  - *"Nút filter ở đâu ta"*
  - *"Sao Kiệt không thấy"*

- **Probe Question:**
  - *Ý kiến đóng góp khác (Nếu có):* làm rõ bộ lọc thông tin khi tìm kiếm 

#### Phiên kiểm thử số 4: Dương Thúy Mi
- **Thời gian hoàn thành:** 3 phút 49 giây | **Số lỗi & Ngập ngừng:** 3 | **Điểm SUS:** 97.5
- **Nhật ký hành vi:**
  - 0:04 - 1:05 (Màn hình C1): Người dùng tìm kiếm User bằng từ khóa "HUY" và sử dụng Filter để lọc ra Student và Status là Unactive.
  - 1:11 - 2:50 (Màn hình C2): Người dùng tạo User mới với role là Admin, sau đó tìm kiếm và đổi Role lại thành Guest.
  - 2:55 - 3:17 (Màn hình C3): Người dùng Export Excel danh sách về và mở file mượt mà.
  - 3:27 - 3:51 (Màn hình C4): Người dùng muốn Unactive tài khoản mình vừa tạo để xóa, nhưng không thấy nút để thực hiện và phải nhờ sự trợ giúp mới thấy.

- **Khó khăn & Lỗi SUT bắt gặp theo từng nhiệm vụ:**
  - *Nhiệm vụ 1 (Khám phá & Tìm kiếm):* Không có
  - *Nhiệm vụ 2 (Thêm & Chỉnh sửa user):*
    - Lúc 1:45 trong Video, thay vì hiện quy định Password và Member Code ngay từ đầu thì phải ấn Create User rồi người dùng mới biết.
    - Lúc 2:16 trong Video, người dùng muốn tìm kiếm lại tài khoản mình vừa tạo nhưng không thấy và phải nhờ trợ giúp mới thấy là chưa bỏ Filter Role.
  - *Nhiệm vụ 3 (Xuất báo cáo Excel):* Không có
  - *Nhiệm vụ 4 (Xóa user & Audit Log):*
    - Lúc 3:37 trong Video, người dùng muốn Unactive tài khoản của mình nhưng không thấy nút bấm Active/Unactive tài khoản, phải có sự trợ giúp mới biết.

- **Phát biểu trực tiếp nổi bật (Think-aloud/Quotes):**
  - *"Ủa sao không có mình ở đây vậy"*
  - *"Là chưa thành công phải hong"*
  - *"À quên quên quên, chưa bỏ bộ lọc ra, hèn gì"*
  - *"Vậy thì sửa cho nó không còn hoạt động, ủa không sửa được"*
  - *"À đây nè, dấu này á hả, không thấy"*

- **Probe Question:**
  - *Ý kiến đóng góp khác (Nếu có):* Không có

---

### 3.5. Phân tích lỗi & Vấn đề (Ranked Findings)

| Vấn đề gặp phải (Friction points / Bugs) | Ảnh minh họa (Screenshot) | Mức độ nghiêm trọng (Severity 0-4) | Đề xuất giải pháp UI/UX |
|---|---|---|---|
| **Lỗi hỏng cấu trúc tệp Excel khi mở (Excel Error):** Người dùng xuất file Excel thành công nhưng khi mở lên Microsoft Excel báo lỗi cấu trúc tệp bắt Repair gây hoang mang (Cả 4 User đều gặp phải, nhưng chỉ có User 1 và User 3 là bối rối, cần sự trợ giúp). | [Xem ảnh](../images/usability-error-hesitant/Excel.jpg) | 3 | Sửa đổi thư viện kết xuất Excel phía Backend để xuất đúng định dạng OpenXML chuẩn, tránh lỗi cấu trúc XML nội bộ. |
| **Tìm kiếm (Search) lỗi phân trang và chữ viết thường:** Khi gõ tìm kiếm viết thường ("hoàng", "kỳ"), kết quả hiển thị lại xuất hiện những User không liên quan và còn bị lỗi pagination nhảy sai lệch, người dùng buộc phải click pagination dưới chân trang mới hiển thị đúng kết quả (User 2 gặp phải). | [Xem ảnh](../images/usability-error-hesitant/Search_User.jpg) | 3 | Khắc phục lỗi đồng bộ dữ liệu pagination khi kích hoạt chức năng tìm kiếm; đảm bảo tìm kiếm không phân biệt chữ hoa/chữ thường. |
| **Tìm kiếm không hỗ trợ lọc họ tên đầy đủ (Full Name):** Khi người dùng vừa tạo tài khoản (ví dụ "A Nguyen" ở User 1) và tìm kiếm lại bằng cụm từ này, hệ thống không trả về kết quả vì thanh tìm kiếm chỉ hỗ trợ đối sánh rời rạc "Họ" hoặc "Tên" (User 1). | [Xem ảnh](../images/usability-error-hesitant/Search_After_Create.jpg) | 3 | Nâng cấp API tìm kiếm ở backend để hỗ trợ truy vấn linh hoạt toàn bộ chuỗi họ tên chứa khoảng trắng (Full Name). |
| **Không thấy nút đổi trạng thái Active/Unactive:** Nút chuyển đổi Active/Unactive được thiết kế dạng Toggle Button nhưng độ tương phản kém và thiếu nhãn hướng dẫn, khiến người dùng không nhận diện được nút để thay đổi trạng thái user (User 4 phải nhờ trợ giúp). | [Xem ảnh](../images/usability-error-hesitant/Set_Unactive.jpg) | 2 | Tăng độ tương phản màu sắc của Toggle Button và bổ sung nhãn văn bản chỉ dẫn kế bên nút. |
| **Khó khăn khi muốn xem thông tin chi tiết người dùng:** Người dùng muốn click vào dòng hoặc avatar của User để xem trang thông tin chi tiết (User Detail) nhưng hệ thống không hỗ trợ tính năng này, gây hiểu lầm về UX (User 2, User 3 gặp phải). | [Xem ảnh](../images/usability-error-hesitant/Detail_User.jpg) | 2 | Bổ sung nút "Xem chi tiết" (View Detail) ở cột Actions hoặc cho phép click vào hàng dữ liệu để hiển thị popup thông tin chi tiết. |
| **Trải nghiệm Validation Form kém (Tuần tự & Thiếu hướng dẫn):** Form tạo mới không ghi rõ quy định mật khẩu/SĐT từ đầu. Khi bấm "Create User", hệ thống chỉ báo lỗi từng trường một (sửa xong lỗi này bấm tiếp mới báo lỗi khác) khiến người dùng phải nhấn nút nhiều lần. | [Xem ảnh](../images/usability-error-hesitant/Create_User.jpg) | 2 | Hiển thị trực quan quy định định dạng kế bên nhãn. Thực hiện validate toàn bộ biểu mẫu và hiển thị thông báo lỗi đồng loạt cho tất cả các trường không hợp lệ trong một lần nhấn nút. |
| **Con trỏ chuột không đổi kiểu khi di chuột lên nút:** Khi người dùng trỏ chuột tới nút "Create User", con trỏ chuột không thay đổi thành hình bàn tay (pointer cursor) khiến họ phân vân không rõ nút có thể bấm được hay không. | [Xem ảnh](../images/usability-error-hesitant/Press_Create_User.jpg) | 1 | Thêm thuộc tính CSS `cursor: pointer` cho toàn bộ các nút bấm (button) trên hệ thống để tăng phản hồi tương tác (feedback). |
| **Bộ lọc thông tin (Filter) kém nổi bật:** Khu vực bộ lọc Role/Status có kích thước nhỏ, biểu tượng không trực quan khiến người dùng mất thời gian tìm kiếm nút lọc (User 3 mất hơn 15s loay hoay). | [Xem ảnh](../images/usability-error-hesitant/Filter_User.jpg) | 2 | Làm nổi bật khu vực bộ lọc trên giao diện và thêm nút "Hủy bộ lọc" (Clear Filter) nhanh bên cạnh. |

*(Chú thích mức độ nghiêm trọng: 1 = Thẩm mỹ, 2 = Nhẹ, 3 = Nặng, 4 = Blocker).*

---

### 3.6. Đề xuất cải thiện ưu tiên (Prioritized Recommendations)

1. **Ưu tiên 1 (High Priority): Sửa lỗi file Excel & Tối ưu Tìm kiếm (Search)**
   - **Đề xuất:** Sửa lỗi cấu trúc file Excel xuất ra để mở được mượt mà trên MS Excel. Tối ưu hóa chức năng API Tìm kiếm phía backend để hỗ trợ tìm kiếm đầy đủ họ và tên có khoảng trắng (Full Name) và khắc phục lỗi phân trang khi gõ tìm kiếm viết thường.
   - **Lý do:** Đây là những điểm nghẽn nghiêm trọng cản trở trực tiếp người dùng hoàn thành công việc kết xuất dữ liệu và tìm kiếm người dùng cụ thể để phân quyền.
2. **Ưu tiên 2 (Medium Priority): Tối ưu biểu mẫu & Validation Form tạo mới**
   - **Đề xuất:** Hiển thị trực quan quy định định dạng mật khẩu/SĐT ngay trong form tạo mới để người dùng biết trước. Sửa đổi validation của biểu mẫu để thông báo lỗi đồng loạt cho tất cả các trường không hợp lệ trong một lần submit. Bổ sung hiệu ứng `cursor: pointer` khi trỏ chuột vào nút bấm.
   - **Lý do:** Giúp giảm thiểu số lần thao tác nhập liệu thừa của người dùng, tăng sự tự tin khi tương tác giao diện và tăng đáng kể tốc độ hoàn thành nhiệm vụ.
3. **Ưu tiên 3 (Low Priority): Tăng cường phản hồi hệ thống (Feedback) & Bộ lọc (Filter)**
   - **Đề xuất:** Bổ sung trang/popup xem thông tin chi tiết người dùng. Cải thiện thiết kế và độ trực quan (tăng tương phản, nhãn hướng dẫn) của Toggle Button Active/Unactive. Thiết kế thêm nút "Xóa nhanh bộ lọc" (Clear Filter).
   - **Lý do:** Tối ưu hóa luồng tương tác khám phá danh sách và quản lý trạng thái, giúp người dùng dễ nhận diện các khu vực thao tác.

---

## 4. Đường Dẫn Minh Chứng Quay Video Màn Hình (Screen Recordings)

Để xác thực tính xác thực của các phiên thử nghiệm khả dụng, toàn bộ video quay màn hình và âm thanh quá trình thực hiện kịch bản của các người tham gia đã được tải lên thư mục lưu trữ trực tuyến:

- **Đường dẫn thư mục Google Drive chứa video:** [Liên kết Google Drive](https://drive.google.com/drive/folders/1BoebOJamcK_G9Xbpi6mvRKpUjvctfNwq?usp=sharing)
- **Đường dẫn trực tiếp đến thư mục Google Drive chứa video:** https://drive.google.com/drive/folders/1BoebOJamcK_G9Xbpi6mvRKpUjvctfNwq?usp=sharing
- **Danh sách file video minh chứng:**
  - `User-1.mp4` (Nguyễn Tấn Đạt)
  - `User-2.mp4` (Nguyễn Thị Cẩm Nhung)
  - `User-3.mp4` (Nguyễn Tuấn Kiệt)
  - `User-4.mp4` (Dương Thúy Mi)