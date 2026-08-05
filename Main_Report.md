# HW03: GUI Usability

**Kịch bản chọn:** Scenario C — Admin manages users (Function group: user administration).

**Bao gồm các Screen:**
- C1 - Users List — Search, Role/Active Filters, Columns
- C2 - Create / Edit User & Assign Role
- C3 - Export to Excel — Column Completeness and Download Feedback
- C4 - Delete User Confirmation Dialog & Audit Logs

## Task 1: GUI Checklist

### Part A: Shared Checklist

| ID | Khía Cạnh | Mục Kiểm Tra (Checklist Item Description) | Ánh Xạ Heuristics / Nguyên Tắc |
|---|---|---|---|
| **IA-01** | **General UI** | **IA-01: General UI Standards (Layout, Typography, Color, Consistency, i18n)** | |
| IA-01-01 | General UI | Hệ thống lưới và khoảng cách (Grid & Spacing) căn lề nhất quán trên toàn màn hình. | Nielsen #4: Consistency |
| IA-01-02 | General UI | Font chữ (typography) nhất quán về kích thước, độ dày (bold/regular) và phân cấp tiêu đề. | Nielsen #4: Consistency |
| IA-01-03 | General UI | Màu sắc của các nút hành động (Primary, Secondary) và trạng thái nhất quán. | Norman: Signifiers |
| IA-01-04 | General UI | Đa ngôn ngữ (EN/VI) hoạt động đầy đủ, không bị dịch thiếu hoặc chồng lấp chữ. | Nielsen #4: Consistency |
| IA-01-05 | General UI | Trạng thái rỗng (Empty state) được hiển thị rõ ràng khi không có sự kiện/dữ liệu nào. | Nielsen #1: Visibility |
| IA-01-06 | General UI | Trạng thái đang tải (Loading state/skeleton) hiển thị khi kéo dữ liệu chậm. | Nielsen #1: Visibility |
| IA-01-07 | General UI | Trang web tương thích tốt và tự động co giãn (Responsive) trên màn hình. | Nielsen #4: Consistency |
| IA-01-08 | General UI | Các hình ảnh (Thumbnail/Banner) không bị méo tỉ lệ hiển thị (tỷ lệ 4:3 và 24:9) trên các kích thước màn hình khác nhau. | Shneiderman: Aesthetics |
| IA-01-09 | General UI | Các icon được căn chỉnh đúng tâm so với nhãn text bên cạnh. | Shneiderman: Aesthetics |
| IA-01-10 | General UI | Độ tương phản màu sắc giữa văn bản và nền đủ rõ ràng (Accessibility WCAG). | Nielsen #4: Consistency |
| IA-01-11 | General UI | Các liên kết ngoài (External links) mở ở tab mới, liên kết nội bộ (Internal links) mở ở tab hiện tại. | Nielsen #3: User Control |
| IA-01-12 | General UI | Ảnh Thumbnail (4:3) và Banner (24:9) không bị cắt xén mất nội dung quan trọng. | Nielsen #4: Consistency |
| **IA-02** | **Forms** | **IA-02: Forms (Labels, Validation, Errors, Required Fields, Rich Text)** | |
| IA-02-01 | Forms | Các trường bắt buộc nhập (Required fields) được đánh dấu ký hiệu trực quan (ví dụ dấu `*`). | Norman: Constraints |
| IA-02-02 | Forms | Nhãn (Labels) của trường nhập liệu luôn hiển thị rõ ràng và đi sát với ô nhập liệu. | Nielsen #6: Recognition |
| IA-02-03 | Forms | Validation thời gian thực báo lỗi đỏ trực quan ngay dưới trường nhập liệu bị lỗi. | Nielsen #5: Error Prev. |
| IA-02-04 | Forms | Thông báo lỗi cụ thể, hướng dẫn cách khắc phục thay vì báo lỗi chung chung. | Nielsen #10: Help & Error |
| IA-02-05 | Forms | Định dạng tải lên (Upload file/image) kiểm tra đúng định dạng và dung lượng tối đa. | Norman: Constraints |
| IA-02-06 | Forms | Trình soạn thảo Rich Text hiển thị đầy đủ thanh công cụ và hoạt động mượt mà. | Nielsen #7: Flexibility |
| IA-02-07 | Forms | Người dùng có thể nhấn `Tab` để di chuyển tuần tự qua các ô nhập liệu trong form. | Nielsen #7: Flexibility |
| IA-02-08 | Forms | Các nút Submit/Save bị vô hiệu hóa (disabled) khi form chưa điền đủ thông tin hợp lệ. | Nielsen #5: Error Prev. |
| IA-02-09 | Forms | Định dạng ngày giờ hiển thị theo chuẩn cục bộ dễ đọc đối với người dùng Việt Nam. | Nielsen #2: Match System |
| IA-02-10 | Forms | Nút xóa nhanh (clear button) hoặc reset form hoạt động chính xác. | Nielsen #3: User Control |
| IA-02-11 | Forms | Trình duyệt hỗ trợ tính năng tự động điền (autofill) cho các trường thông tin cơ bản. | Nielsen #7: Flexibility |
| IA-02-12 | Forms | Ô nhập mật khẩu hỗ trợ tính năng toggle ẩn/hiện mật khẩu trực quan bằng biểu tượng con mắt. | Nielsen #7: Flexibility |
| **IA-03** | **Navigation** | **IA-03: Navigation (Menus, Breadcrumbs, Sidebar, Tabs, Back actions, Deep links)** | |
| IA-03-01 | Navigation | Menu điều hướng chính luôn cố định hoặc dễ dàng truy cập ở đầu trang/thanh bên. | Nielsen #6: Recognition |
| IA-03-02 | Navigation | Trạng thái hiện tại của trang (Active state) được làm nổi bật trên menu điều hướng. | Nielsen #1: Visibility |
| IA-03-03 | Navigation | Nút quay lại (Back/Return action) đưa người dùng về đúng trang trước đó, không mất trạng thái. | Nielsen #3: User Control |
| IA-03-04 | Navigation | Liên kết sâu (Deep links) dẫn trực tiếp đến trang chi tiết sự kiện mà không bị lỗi 404. | Nielsen #4: Consistency |
| IA-03-05 | Navigation | Breadcrumbs hiển thị đúng phân cấp thư mục và có thể click để quay về thư mục cha. | Nielsen #6: Recognition |
| IA-03-06 | Navigation | Tính năng kéo thả thay đổi thứ tự (Reorder) hiển thị trực quan (dòng bị kéo mờ opacity-50) và các nút thao tác khác tạm thời bị vô hiệu hóa. | Norman: Feedback |
| IA-03-07 | Navigation | Các tab chuyển đổi nhanh hoạt động độc lập và tải đúng dữ liệu tương ứng. | Nielsen #7: Flexibility |
| IA-03-08 | Navigation | Không có liên kết nào bị hỏng (Broken links / 404 error) trên toàn giao diện. | Nielsen #4: Consistency |
| IA-03-09 | Navigation | Nút "Cuộn lên đầu trang" (Back to top) hiển thị khi người dùng cuộn xuống sâu (nếu có). | Nielsen #7: Flexibility |
| IA-03-10 | Navigation | Thanh bên sidebar có thể thu gọn/mở rộng mượt mà và không che khuất nội dung chính. | Nielsen #3: User Control |
| IA-03-11 | Navigation | Đường dẫn URL trên thanh địa chỉ thay đổi tương ứng khi chuyển đổi qua lại giữa các tab hoặc bộ lọc. | Nielsen #4: Consistency |
| IA-03-12 | Navigation | Giao diện kéo thả (Reorder) hiển thị biểu tượng tay cầm (drag handle) rõ ràng để gợi ý khả năng tương tác. | Norman: Signifiers |
| **IA-04** | **Feedback** | **IA-04: Feedback & State (Toasts, Badges, Confirmations, Progress Bars, Status Colors)** | |
| IA-04-01 | Feedback | Thông báo nổi (Toasts) xuất hiện ngay sau khi thực hiện hành động và tự động tắt sau 3-5s. | Norman: Feedback |
| IA-04-02 | Feedback | Toasts có màu sắc phân biệt rõ ràng: Xanh (Thành công), Đỏ (Lỗi), Vàng (Cảnh báo). | Nielsen #8: Aesthetic |
| IA-04-03 | Feedback | Hộp thoại xác nhận (Confirmation dialog) xuất hiện trước các hành động hủy/xóa quan trọng. | Nielsen #5: Error Prev. |
| IA-04-04 | Feedback | Huy hiệu (Badges) hiển thị chính xác số lượng thông báo; trạng thái vé thay đổi tương ứng khi được phê duyệt/hủy. | Nielsen #1: Visibility |
| IA-04-05 | Feedback | Thanh tiến trình (Progress bar) hoặc vòng xoay tải (Spinner) xuất hiện khi hệ thống xử lý. | Nielsen #1: Visibility |
| IA-04-06 | Feedback | Trạng thái hiển thị màu sắc tương thích với ngữ nghĩa (Ví dụ: APPROVED màu xanh lá, REJECTED màu đỏ). | Nielsen #2: Match System |
| IA-04-07 | Feedback | Chấm đỏ thông báo (Notification dot) hiển thị động ngay khi có thay đổi trạng thái đăng ký. | Nielsen #1: Visibility |
| IA-04-08 | Feedback | Hộp thoại chi tiết ảnh (Lightbox) mở rộng mượt mà khi click vào ảnh đính kèm. | Nielsen #7: Flexibility |
| IA-04-09 | Feedback | Cập nhật dữ liệu thời gian thực (Real-time update) mà không cần người dùng reload trang. | Norman: Feedback |
| IA-04-10 | Feedback | Hiển thị thông báo rõ ràng khi mất kết nối mạng Internet. | Nielsen #1: Visibility |
| IA-04-11 | Feedback | Hệ thống vô hiệu hóa nút gửi hoặc ngăn chặn gửi dữ liệu trùng lặp khi người dùng click đúp nút Submit. | Nielsen #5: Error Prev. |
| IA-04-12 | Feedback | Mã QR/Barcode trên vé hiển thị rõ nét (không bị mờ), có kích thước tối thiểu đảm bảo quét được bằng ứng dụng camera thông thường. | Nielsen #1: Visibility |
| IA-04-13 | Feedback | Ô nhập liệu (text box) hiển thị hiệu ứng viền/nổi bật trực quan (focus state) khi nhấp chuột vào để người dùng nhận biết rõ ràng đang thao tác/nhập liệu. | Norman: Feedback |
| IA-04-14 | Feedback | Các nút secondary actions phải được vô hiệu hóa (disabled + đổi con trỏ) khi không có gì để thực hiện, hoặc phải hiển thị phản hồi rõ ràng (toast/thông báo) nếu vẫn cho phép bấm mà không có tác dụng gì | Norman: Feedback + Signifiers |

### Part B: Execution on Scenario

**C1 - Users list — Search, Role/Active Filters, Columns:**

| ID | Khía Cạnh | Mục Kiểm Tra (Checklist Item Description) | Ánh Xạ Heuristics / Nguyên Tắc | Screen 1 - C1 (Pass/Fail/NA) | Ghi Chú Lỗi (Notes) |
|---|---|---|---|---|---|
| **IA-01** | **General UI** | **IA-01: General UI Standards (Layout, Typography, Color, Consistency, i18n)** | | |
| IA-01-01 | General UI | Hệ thống lưới và khoảng cách (Grid & Spacing) căn lề nhất quán trên toàn màn hình. | Nielsen #4: Consistency | Pass | |
| IA-01-02 | General UI | Font chữ (typography) nhất quán về kích thước, độ dày (bold/regular) và phân cấp tiêu đề. | Nielsen #4: Consistency | Pass | |
| IA-01-03 | General UI | Màu sắc của các nút hành động (Primary, Secondary) và trạng thái nhất quán. | Norman: Signifiers | Pass | |
| IA-01-04 | General UI | Đa ngôn ngữ (EN/VI) hoạt động đầy đủ, không bị dịch thiếu hoặc chồng lấp chữ. | Nielsen #4: Consistency | Fail | Lỗi i18n: Tại ô nhập liệu phân trang 'Đến trang', khi thiết lập giao diện tiếng Việt và nhập giá trị không hợp lệ (ví dụ: nhập số trang vượt quá giới hạn như 11/10, hoặc số âm như -1), trình duyệt hiển thị thông báo lỗi bằng tiếng Anh ('Value must be less than or equal to...' / 'Value must be greater than or equal to...') thay vì tiếng Việt. [Xem ảnh](images/bug-defect/Screen-C1-IA-01-04a.jpg) [Xem ảnh](images/bug-defect/Screen-C1-IA-01-04b.jpg) |
| IA-01-05 | General UI | Trạng thái rỗng (Empty state) được hiển thị rõ ràng khi không có sự kiện/dữ liệu nào. | Nielsen #1: Visibility | Pass | |
| IA-01-06 | General UI | Trạng thái đang tải (Loading state/skeleton) hiển thị khi kéo dữ liệu chậm. | Nielsen #1: Visibility | Pass | |
| IA-01-07 | General UI | Trang web tương thích tốt và tự động co giãn (Responsive) trên màn hình. | Nielsen #4: Consistency | Fail | Lỗi responsive: Sidebar không tự động thu gọn lại khi thu nhỏ màn hình trình duyệt, dẫn đến các cột thông tin của bảng Users list bị che khuất và không thể xem được đầy đủ dữ liệu (chỉ hiển thị đủ khi Admin chủ động click thu gọn sidebar thủ công). [Xem ảnh](images/bug-defect/Screen-C1-IA-01-07.jpg) |
| IA-01-08 | General UI | Các hình ảnh (Thumbnail/Banner) không bị méo tỉ lệ hiển thị (tỷ lệ 4:3 và 24:9) trên các kích thước màn hình khác nhau. | Shneiderman: Aesthetics | N/A | |
| IA-01-09 | General UI | Các icon được căn chỉnh đúng tâm so với nhãn text bên cạnh. | Shneiderman: Aesthetics | Pass | |
| IA-01-10 | General UI | Độ tương phản màu sắc giữa văn bản và nền đủ rõ ràng (Accessibility WCAG). | Nielsen #4: Consistency | Pass | |
| IA-01-11 | General UI | Các liên kết ngoài (External links) mở ở tab mới, liên kết nội bộ (Internal links) mở ở tab hiện tại. | Nielsen #3: User Control | N/A | |
| IA-01-12 | General UI | Ảnh Thumbnail (4:3) và Banner (24:9) không bị cắt xén mất nội dung quan trọng. | Nielsen #4: Consistency | N/A | |
| **IA-02** | **Forms** | **IA-02: Forms (Labels, Validation, Errors, Required Fields, Rich Text)** | | |
| IA-02-01 | Forms | Các trường bắt buộc nhập (Required fields) được đánh dấu ký hiệu trực quan (ví dụ dấu `*`). | Norman: Constraints | N/A | |
| IA-02-02 | Forms | Nhãn (Labels) của trường nhập liệu luôn hiển thị rõ ràng và đi sát với ô nhập liệu. | Nielsen #6: Recognition | Pass | |
| IA-02-03 | Forms | Validation thời gian thực báo lỗi đỏ trực quan ngay dưới trường nhập liệu bị lỗi. | Nielsen #5: Error Prev. | N/A | |
| IA-02-04 | Forms | Thông báo lỗi cụ thể, hướng dẫn cách khắc phục thay vì báo lỗi chung chung. | Nielsen #10: Help & Error | Pass | |
| IA-02-05 | Forms | Định dạng tải lên (Upload file/image) kiểm tra đúng định dạng và dung lượng tối đa. | Norman: Constraints | N/A | |
| IA-02-06 | Forms | Trình soạn thảo Rich Text hiển thị đầy đủ thanh công cụ và hoạt động mượt mà. | Nielsen #7: Flexibility | N/A | |
| IA-02-07 | Forms | Người dùng có thể nhấn `Tab` để di chuyển tuần tự qua các ô nhập liệu trong form. | Nielsen #7: Flexibility | Pass | |
| IA-02-08 | Forms | Các nút Submit/Save bị vô hiệu hóa (disabled) khi form chưa điền đủ thông tin hợp lệ. | Nielsen #5: Error Prev. | N/A | |
| IA-02-09 | Forms | Định dạng ngày giờ hiển thị theo chuẩn cục bộ dễ đọc đối với người dùng Việt Nam. | Nielsen #2: Match System | N/A | |
| IA-02-10 | Forms | Nút xóa nhanh (clear button) hoặc reset form hoạt động chính xác. | Nielsen #3: User Control | N/A | |
| IA-02-11 | Forms | Trình duyệt hỗ trợ tính năng tự động điền (autofill) cho các trường thông tin cơ bản. | Nielsen #7: Flexibility | N/A | |
| IA-02-12 | Forms | Ô nhập mật khẩu hỗ trợ tính năng toggle ẩn/hiện mật khẩu trực quan bằng biểu tượng con mắt. | Nielsen #7: Flexibility | N/A | |
| **IA-03** | **Navigation** | **IA-03: Navigation (Menus, Breadcrumbs, Sidebar, Tabs, Back actions, Deep links)** | | |
| IA-03-01 | Navigation | Menu điều hướng chính luôn cố định hoặc dễ dàng truy cập ở đầu trang/thanh bên. | Nielsen #6: Recognition | Pass | |
| IA-03-02 | Navigation | Trạng thái hiện tại của trang (Active state) được làm nổi bật trên menu điều hướng. | Nielsen #1: Visibility | Pass | |
| IA-03-03 | Navigation | Nút quay lại (Back/Return action) đưa người dùng về đúng trang trước đó, không mất trạng thái. | Nielsen #3: User Control | N/A | |
| IA-03-04 | Navigation | Liên kết sâu (Deep links) dẫn trực tiếp đến trang chi tiết sự kiện mà không bị lỗi 404. | Nielsen #4: Consistency | N/A | |
| IA-03-05 | Navigation | Breadcrumbs hiển thị đúng phân cấp thư mục và có thể click để quay về thư mục cha. | Nielsen #6: Recognition | N/A | |
| IA-03-06 | Navigation | Tính năng kéo thả thay đổi thứ tự (Reorder) hiển thị trực quan (dòng bị kéo mờ opacity-50) và các nút thao tác khác tạm thời bị vô hiệu hóa. | Norman: Feedback | N/A | |
| IA-03-07 | Navigation | Các tab chuyển đổi nhanh hoạt động độc lập và tải đúng dữ liệu tương ứng. | Nielsen #7: Flexibility | N/A | |
| IA-03-08 | Navigation | Không có liên kết nào bị hỏng (Broken links / 404 error) trên toàn giao diện. | Nielsen #4: Consistency | Pass | |
| IA-03-09 | Navigation | Nút "Cuộn lên đầu trang" (Back to top) hiển thị khi người dùng cuộn xuống sâu (nếu có). | Nielsen #7: Flexibility | N/A | |
| IA-03-10 | Navigation | Thanh bên sidebar có thể thu gọn/mở rộng mượt mà và không che khuất nội dung chính. | Nielsen #3: User Control | Pass | |
| IA-03-11 | Navigation | Đường dẫn URL trên thanh địa chỉ thay đổi tương ứng khi chuyển đổi qua lại giữa các tab hoặc bộ lọc. | Nielsen #4: Consistency | Pass | |
| IA-03-12 | Navigation | Giao diện kéo thả (Reorder) hiển thị biểu tượng tay cầm (drag handle) rõ ràng để gợi ý khả năng tương tác. | Norman: Signifiers | N/A | |
| **IA-04** | **Feedback** | **IA-04: Feedback & State (Toasts, Badges, Confirmations, Progress Bars, Status Colors)** | | |
| IA-04-01 | Feedback | Thông báo nổi (Toasts) xuất hiện ngay sau khi thực hiện hành động và tự động tắt sau 3-5s. | Norman: Feedback | N/A | |
| IA-04-02 | Feedback | Toasts có màu sắc phân biệt rõ ràng: Xanh (Thành công), Đỏ (Lỗi), Vàng (Cảnh báo). | Nielsen #8: Aesthetic | N/A | |
| IA-04-03 | Feedback | Hộp thoại xác nhận (Confirmation dialog) xuất hiện trước các hành động hủy/xóa quan trọng. | Nielsen #5: Error Prev. | N/A | |
| IA-04-04 | Feedback | Huy hiệu (Badges) hiển thị chính xác số lượng thông báo; trạng thái vé thay đổi tương ứng khi được phê duyệt/hủy. | Nielsen #1: Visibility | N/A | |
| IA-04-05 | Feedback | Thanh tiến trình (Progress bar) hoặc vòng xoay tải (Spinner) xuất hiện khi hệ thống xử lý. | Nielsen #1: Visibility | Pass | |
| IA-04-06 | Feedback | Trạng thái hiển thị màu sắc tương thích với ngữ nghĩa (Ví dụ: APPROVED màu xanh lá, REJECTED màu đỏ). | Nielsen #2: Match System | Pass | |
| IA-04-07 | Feedback | Chấm đỏ thông báo (Notification dot) hiển thị động ngay khi có thay đổi trạng thái đăng ký. | Nielsen #1: Visibility | N/A | |
| IA-04-08 | Feedback | Hộp thoại chi tiết ảnh (Lightbox) mở rộng mượt mà khi click vào ảnh đính kèm. | Nielsen #7: Flexibility | N/A | |
| IA-04-09 | Feedback | Cập nhật dữ liệu thời gian thực (Real-time update) mà không cần người dùng reload trang. | Norman: Feedback | Fail | Hệ thống không tự động cập nhật danh sách người dùng theo thời gian thực. Khi chỉnh sửa tên user ở tab Admin 1 (ví dụ đổi từ "def abc" thành "B A"), tab Admin 2 bên cạnh vẫn hiển thị tên cũ là "def abc" cho đến khi reload trang thủ công. [Xem ảnh](images/bug-defect/Screen-C1-IA-04-09a.jpg) [Xem ảnh](images/bug-defect/Screen-C1-IA-04-09b.jpg) |
| IA-04-10 | Feedback | Hiển thị thông báo rõ ràng khi mất kết nối mạng Internet. | Nielsen #1: Visibility | N/A | |
| IA-04-11 | Feedback | Hệ thống vô hiệu hóa nút gửi hoặc ngăn chặn gửi dữ liệu trùng lặp khi người dùng click đúp nút Submit. | Nielsen #5: Error Prev. | N/A | |
| IA-04-12 | Feedback | Mã QR/Barcode trên vé hiển thị rõ nét (không bị mờ), có kích thước tối thiểu đảm bảo quét được bằng ứng dụng camera thông thường. | Nielsen #1: Visibility | N/A | |
| IA-04-13 | Feedback | Ô nhập liệu (text box) hiển thị hiệu ứng viền/nổi bật trực quan (focus state) khi nhấp chuột vào để người dùng nhận biết rõ ràng đang thao tác/nhập liệu. | Norman: Feedback | Pass | |
| IA-04-14 | Feedback | Các nút secondary actions phải được vô hiệu hóa (disabled + đổi con trỏ) khi không có gì để thực hiện, hoặc phải hiển thị phản hồi rõ ràng (toast/thông báo) nếu vẫn cho phép bấm mà không có tác dụng gì | Norman: Feedback + Signifiers | N/A | |

<br>

**C2 - Create / Edit User & Assign Role:**

| ID | Khía Cạnh | Mục Kiểm Tra (Checklist Item Description) | Ánh Xạ Heuristics / Nguyên Tắc | Screen 2 - C2 (Pass/Fail/NA) | Ghi Chú Lỗi (Notes) |
|---|---|---|---|---|---|
| **IA-01** | **General UI** | **IA-01: General UI Standards (Layout, Typography, Color, Consistency, i18n)** | | | |
| IA-01-01 | General UI | Hệ thống lưới và khoảng cách (Grid & Spacing) căn lề nhất quán trên toàn màn hình. | Nielsen #4: Consistency | Pass | |
| IA-01-02 | General UI | Font chữ (typography) nhất quán về kích thước, độ dày (bold/regular) và phân cấp tiêu đề. | Nielsen #4: Consistency | Pass | |
| IA-01-03 | General UI | Màu sắc của các nút hành động (Primary, Secondary) và trạng thái nhất quán. | Norman: Signifiers | Pass | |
| IA-01-04 | General UI | Đa ngôn ngữ (EN/VI) hoạt động đầy đủ, không bị dịch thiếu hoặc chồng lấp chữ. | Nielsen #4: Consistency | Fail | Lỗi i18n: Khi nhập email không đúng định dạng trong form "Tạo người dùng mới", thông báo lỗi của trình duyệt hiển thị bằng tiếng Anh ("Please include an '@' in the email address..."), trong khi các trường lỗi khác và toàn bộ giao diện đang hiển thị tiếng Việt bình thường. [Xem ảnh](images/bug-defect/Screen-C2-IA-01-04.jpg) |
| IA-01-05 | General UI | Trạng thái rỗng (Empty state) được hiển thị rõ ràng khi không có sự kiện/dữ liệu nào. | Nielsen #1: Visibility | N/A | |
| IA-01-06 | General UI | Trạng thái đang tải (Loading state/skeleton) hiển thị khi kéo dữ liệu chậm. | Nielsen #1: Visibility | N/A | |
| IA-01-07 | General UI | Trang web tương thích tốt và tự động co giãn (Responsive) trên màn hình. | Nielsen #4: Consistency | Fail | Lỗi responsive: Khi hiển thị trên các màn hình nhỏ (như thiết bị di động), form Create User bị thu nhỏ kích thước (zoom out) quá mức, dẫn đến chữ và các trường nhập liệu cực kỳ nhỏ, rất khó để Admin nhìn rõ và nhấp chọn chính xác. [Xem ảnh](images/bug-defect/Screen-C2-IA-01-07.jpg) |
| IA-01-08 | General UI | Các hình ảnh (Thumbnail/Banner) không bị méo tỉ lệ hiển thị (tỷ lệ 4:3 và 24:9) trên các kích thước màn hình khác nhau. | Shneiderman: Aesthetics | N/A | |
| IA-01-09 | General UI | Các icon được căn chỉnh đúng tâm so với nhãn text bên cạnh. | Shneiderman: Aesthetics | Pass | |
| IA-01-10 | General UI | Độ tương phản màu sắc giữa văn bản và nền đủ rõ ràng (Accessibility WCAG). | Nielsen #4: Consistency | Pass | |
| IA-01-11 | General UI | Các liên kết ngoài (External links) mở ở tab mới, liên kết nội bộ (Internal links) mở ở tab hiện tại. | Nielsen #3: User Control | N/A | |
| IA-01-12 | General UI | Ảnh Thumbnail (4:3) và Banner (24:9) không bị cắt xén mất nội dung quan trọng. | Nielsen #4: Consistency | N/A | |
| **IA-02** | **Forms** | **IA-02: Forms (Labels, Validation, Errors, Required Fields, Rich Text)** | | | |
| IA-02-01 | Forms | Các trường bắt buộc nhập (Required fields) được đánh dấu ký hiệu trực quan (ví dụ dấu `*`). | Norman: Constraints | Fail | Form "Tạo người dùng mới" không hiển thị dấu hoa thị màu đỏ `*` cạnh các trường bắt buộc, nhưng khi nhấn "Create User" hệ thống lại báo lỗi bắt buộc nhập (ví dụ: "Last name is required", "First name is required", "Role is required"). [Xem ảnh](images/bug-defect/Screen-C2-IA-02-01.jpg) |
| IA-02-02 | Forms | Nhãn (Labels) của trường nhập liệu luôn hiển thị rõ ràng và đi sát với ô nhập liệu. | Nielsen #6: Recognition | Fail | Lỗi gợi ý (placeholder): Trong form Create User, ô nhập liệu trường First Name hiển thị placeholder gợi ý là "Last name", còn trường Last name hiển thị placeholder gợi ý là "First name" (bị tráo đổi nội dung placeholder ngược nhau). [Xem ảnh](images/bug-defect/Screen-C2-IA-02-02.jpg) |
| IA-02-03 | Forms | Validation thời gian thực báo lỗi đỏ trực quan ngay dưới trường nhập liệu bị lỗi. | Nielsen #5: Error Prev. | Fail | Không có validation thời gian thực cho trường email (ví dụ nhập "a" nhưng không báo lỗi gì trước khi submit). Chỉ sau khi nhấn "Create User" thì lỗi mới được hiển thị. [Xem ảnh](images/bug-defect/Screen-C2-IA-02-03.jpg) |
| IA-02-04 | Forms | Thông báo lỗi cụ thể, hướng dẫn cách khắc phục thay vì báo lỗi chung chung. | Nielsen #10: Help & Error | Fail | Lỗi nội dung thông báo: Khi người dùng nhập email thiếu tên miền (ví dụ: "abc@abccom"), hệ thống báo lỗi chung chung là "Invalid email address" thay vì chỉ dẫn rõ ràng là người dùng đang thiếu đuôi tên miền (domain extension). [Xem ảnh](images/bug-defect/Screen-C2-IA-02-04.jpg) |
| IA-02-05 | Forms | Định dạng tải lên (Upload file/image) kiểm tra đúng định dạng và dung lượng tối đa. | Norman: Constraints | N/A | |
| IA-02-06 | Forms | Trình soạn thảo Rich Text hiển thị đầy đủ thanh công cụ và hoạt động mượt mà. | Nielsen #7: Flexibility | N/A | |
| IA-02-07 | Forms | Người dùng có thể nhấn `Tab` để di chuyển tuần tự qua các ô nhập liệu trong form. | Nielsen #7: Flexibility | Pass | |
| IA-02-08 | Forms | Các nút Submit/Save bị vô hiệu hóa (disabled) khi form chưa điền đủ thông tin hợp lệ. | Nielsen #5: Error Prev. | Fail | Nút "Create User" vẫn có thể nhấn được (không bị disabled hay chuyển màu xám) ngay cả khi form chưa hợp lệ (ví dụ bỏ trống email, nhập số điện thoại sai định dạng là "a"). [Xem ảnh](images/bug-defect/Screen-C2-IA-02-08.jpg) |
| IA-02-09 | Forms | Định dạng ngày giờ hiển thị theo chuẩn cục bộ dễ đọc đối với người dùng Việt Nam. | Nielsen #2: Match System | N/A | |
| IA-02-10 | Forms | Nút xóa nhanh (clear button) hoặc reset form hoạt động chính xác. | Nielsen #3: User Control | N/A | |
| IA-02-11 | Forms | Trình duyệt hỗ trợ tính năng tự động điền (autofill) cho các trường thông tin cơ bản. | Nielsen #7: Flexibility | N/A | |
| IA-02-12 | Forms | Ô nhập mật khẩu hỗ trợ tính năng toggle ẩn/hiện mật khẩu trực quan bằng biểu tượng con mắt. | Nielsen #7: Flexibility | Pass | |
| **IA-03** | **Navigation** | **IA-03: Navigation (Menus, Breadcrumbs, Sidebar, Tabs, Back actions, Deep links)** | | | |
| IA-03-01 | Navigation | Menu điều hướng chính luôn cố định hoặc dễ dàng truy cập ở đầu trang/thanh bên. | Nielsen #6: Recognition | N/A | |
| IA-03-02 | Navigation | Trạng thái hiện tại của trang (Active state) được làm nổi bật trên menu điều hướng. | Nielsen #1: Visibility | N/A | |
| IA-03-03 | Navigation | Nút quay lại (Back/Return action) đưa người dùng về đúng trang trước đó, không mất trạng thái. | Nielsen #3: User Control | N/A | |
| IA-03-04 | Navigation | Liên kết sâu (Deep links) dẫn trực tiếp đến trang chi tiết sự kiện mà không bị lỗi 404. | Nielsen #4: Consistency | N/A | |
| IA-03-05 | Navigation | Breadcrumbs hiển thị đúng phân cấp thư mục và có thể click để quay về thư mục cha. | Nielsen #6: Recognition | N/A | |
| IA-03-06 | Navigation | Tính năng kéo thả thay đổi thứ tự (Reorder) hiển thị trực quan (dòng bị kéo mờ opacity-50) và các nút thao tác khác tạm thời bị vô hiệu hóa. | Norman: Feedback | N/A | |
| IA-03-07 | Navigation | Các tab chuyển đổi nhanh hoạt động độc lập và tải đúng dữ liệu tương ứng. | Nielsen #7: Flexibility | N/A | |
| IA-03-08 | Navigation | Không có liên kết nào bị hỏng (Broken links / 404 error) trên toàn giao diện. | Nielsen #4: Consistency | N/A | |
| IA-03-09 | Navigation | Nút "Cuộn lên đầu trang" (Back to top) hiển thị khi người dùng cuộn xuống sâu (nếu có). | Nielsen #7: Flexibility | N/A | |
| IA-03-10 | Navigation | Thanh bên sidebar có thể thu gọn/mở rộng mượt mà và không che khuất nội dung chính. | Nielsen #3: User Control | N/A | |
| IA-03-11 | Navigation | Đường dẫn URL trên thanh địa chỉ thay đổi tương ứng khi chuyển đổi qua lại giữa các tab hoặc bộ lọc. | Nielsen #4: Consistency | N/A | |
| IA-03-12 | Navigation | Giao diện kéo thả (Reorder) hiển thị biểu tượng tay cầm (drag handle) rõ ràng để gợi ý khả năng tương tác. | Norman: Signifiers | N/A | |
| **IA-04** | **Feedback** | **IA-04: Feedback & State (Toasts, Badges, Confirmations, Progress Bars, Status Colors)** | | | |
| IA-04-01 | Feedback | Thông báo nổi (Toasts) xuất hiện ngay sau khi thực hiện hành động và tự động tắt sau 3-5s. | Norman: Feedback | Fail | Không hiển thị Toast thông báo sau khi tạo người dùng thành công để xác nhận hành động đã hoàn tất. [Xem ảnh](images/bug-defect/Screen-C2-IA-04-01a.jpg) [Xem ảnh](images/bug-defect/Screen-C2-IA-04-01b.jpg) |
| IA-04-02 | Feedback | Toasts có màu sắc phân biệt rõ ràng: Xanh (Thành công), Đỏ (Lỗi), Vàng (Cảnh báo). | Nielsen #8: Aesthetic | N/A | |
| IA-04-03 | Feedback | Hộp thoại xác nhận (Confirmation dialog) xuất hiện trước các hành động hủy/xóa quan trọng. | Nielsen #5: Error Prev. | N/A | |
| IA-04-04 | Feedback | Huy hiệu (Badges) hiển thị chính xác số lượng thông báo; trạng thái vé thay đổi tương ứng khi được phê duyệt/hủy. | Nielsen #1: Visibility | N/A | |
| IA-04-05 | Feedback | Thanh tiến trình (Progress bar) hoặc vòng xoay tải (Spinner) xuất hiện khi hệ thống xử lý. | Nielsen #1: Visibility | Pass | |
| IA-04-06 | Feedback | Trạng thái hiển thị màu sắc tương thích với ngữ nghĩa (Ví dụ: APPROVED màu xanh lá, REJECTED màu đỏ). | Nielsen #2: Match System | Pass | |
| IA-04-07 | Feedback | Chấm đỏ thông báo (Notification dot) hiển thị động ngay khi có thay đổi trạng thái đăng ký. | Nielsen #1: Visibility | N/A | |
| IA-04-08 | Feedback | Hộp thoại chi tiết ảnh (Lightbox) mở rộng mượt mà khi click vào ảnh đính kèm. | Nielsen #7: Flexibility | N/A | |
| IA-04-09 | Feedback | Cập nhật dữ liệu thời gian thực (Real-time update) mà không cần người dùng reload trang. | Norman: Feedback | N/A | |
| IA-04-10 | Feedback | Hiển thị thông báo rõ ràng khi mất kết nối mạng Internet. | Nielsen #1: Visibility | Fail | Khi mất kết nối mạng đột ngột và nhấn "Create User", hệ thống hiển thị thông báo lỗi thô sơ và tối nghĩa: "Failed to fetch" trực tiếp trên form thay vì đưa ra cảnh báo mất kết nối thân thiện. [Xem ảnh](images/bug-defect/Screen-C2-IA-04-10.jpg) |
| IA-04-11 | Feedback | Hệ thống vô hiệu hóa nút gửi hoặc ngăn chặn gửi dữ liệu trùng lặp khi người dùng click đúp nút Submit. | Nielsen #5: Error Prev. | Pass | |
| IA-04-12 | Feedback | Mã QR/Barcode trên vé hiển thị rõ nét (không bị mờ), có kích thước tối thiểu đảm bảo quét được bằng ứng dụng camera thông thường. | Nielsen #1: Visibility | N/A | |
| IA-04-13 | Feedback | Ô nhập liệu (text box) hiển thị hiệu ứng viền/nổi bật trực quan (focus state) khi nhấp chuột vào để người dùng nhận biết rõ ràng đang thao tác/nhập liệu. | Norman: Feedback | Pass | |
| IA-04-14 | Feedback | Các nút secondary actions phải được vô hiệu hóa (disabled + đổi con trỏ) khi không có gì để thực hiện, hoặc phải hiển thị phản hồi rõ ràng (toast/thông báo) nếu vẫn cho phép bấm mà không có tác dụng gì | Norman: Feedback + Signifiers | Pass | |

<br>

**C3 - Export to Excel — Column Completeness and Download Feedback:**

| ID | Khía Cạnh | Mục Kiểm Tra (Checklist Item Description) | Ánh Xạ Heuristics / Nguyên Tắc | Screen 3 - C3 (Pass/Fail/NA) | Ghi Chú Lỗi (Notes) |
|---|---|---|---|---|---|
| **IA-01** | **General UI** | **IA-01: General UI Standards (Layout, Typography, Color, Consistency, i18n)** | | | |
| IA-01-01 | General UI | Hệ thống lưới và khoảng cách (Grid & Spacing) căn lề nhất quán trên toàn màn hình. | Nielsen #4: Consistency | Pass | |
| IA-01-02 | General UI | Font chữ (typography) nhất quán về kích thước, độ dày (bold/regular) và phân cấp tiêu đề. | Nielsen #4: Consistency | Pass | |
| IA-01-03 | General UI | Màu sắc của các nút hành động (Primary, Secondary) và trạng thái nhất quán. | Norman: Signifiers | Pass | |
| IA-01-04 | General UI | Đa ngôn ngữ (EN/VI) hoạt động đầy đủ, không bị dịch thiếu hoặc chồng lấp chữ. | Nielsen #4: Consistency | Fail | Lỗi i18n: Nội dung và tiêu đề các cột trong file Excel xuất ra hiển thị cố định bằng tiếng Anh (Last Name, First Name, Card Code...), không dịch theo ngôn ngữ Việt Nam của hệ thống. [Xem ảnh](images/bug-defect/Screen-C3-IA-01-04.jpg) |
| IA-01-05 | General UI | Trạng thái rỗng (Empty state) được hiển thị rõ ràng khi không có sự kiện/dữ liệu nào. | Nielsen #1: Visibility | N/A | |
| IA-01-06 | General UI | Trạng thái đang tải (Loading state/skeleton) hiển thị khi kéo dữ liệu chậm. | Nielsen #1: Visibility | N/A | |
| IA-01-07 | General UI | Trang web tương thích tốt và tự động co giãn (Responsive) trên màn hình. | Nielsen #4: Consistency | N/A | |
| IA-01-08 | General UI | Các hình ảnh (Thumbnail/Banner) không bị méo tỉ lệ hiển thị (tỷ lệ 4:3 và 24:9) trên các kích thước màn hình khác nhau. | Shneiderman: Aesthetics | N/A | |
| IA-01-09 | General UI | Các icon được căn chỉnh đúng tâm so với nhãn text bên cạnh. | Shneiderman: Aesthetics | Pass | |
| IA-01-10 | General UI | Độ tương phản màu sắc giữa văn bản và nền đủ rõ ràng (Accessibility WCAG). | Nielsen #4: Consistency | Pass | |
| IA-01-11 | General UI | Các liên kết ngoài (External links) mở ở tab mới, liên kết nội bộ (Internal links) mở ở tab hiện tại. | Nielsen #3: User Control | N/A | |
| IA-01-12 | General UI | Ảnh Thumbnail (4:3) và Banner (24:9) không bị cắt xén mất nội dung quan trọng. | Nielsen #4: Consistency | N/A | |
| **IA-02** | **Forms** | **IA-02: Forms (Labels, Validation, Errors, Required Fields, Rich Text)** | | | |
| IA-02-01 | Forms | Các trường bắt buộc nhập (Required fields) được đánh dấu ký hiệu trực quan (ví dụ dấu `*`). | Norman: Constraints | N/A | |
| IA-02-02 | Forms | Nhãn (Labels) của trường nhập liệu luôn hiển thị rõ ràng và đi sát với ô nhập liệu. | Nielsen #6: Recognition | N/A | |
| IA-02-03 | Forms | Validation thời gian thực báo lỗi đỏ trực quan ngay dưới trường nhập liệu bị lỗi. | Nielsen #5: Error Prev. | N/A | |
| IA-02-04 | Forms | Thông báo lỗi cụ thể, hướng dẫn cách khắc phục thay vì báo lỗi chung chung. | Nielsen #10: Help & Error | N/A | |
| IA-02-05 | Forms | Định dạng tải lên (Upload file/image) kiểm tra đúng định dạng và dung lượng tối đa. | Norman: Constraints | N/A | |
| IA-02-06 | Forms | Trình soạn thảo Rich Text hiển thị đầy đủ thanh công cụ và hoạt động mượt mà. | Nielsen #7: Flexibility | N/A | |
| IA-02-07 | Forms | Người dùng có thể nhấn `Tab` để di chuyển tuần tự qua các ô nhập liệu trong form. | Nielsen #7: Flexibility | N/A | |
| IA-02-08 | Forms | Các nút Submit/Save bị vô hiệu hóa (disabled) khi form chưa điền đủ thông tin hợp lệ. | Nielsen #5: Error Prev. | N/A | |
| IA-02-09 | Forms | Định dạng ngày giờ hiển thị theo chuẩn cục bộ dễ đọc đối với người dùng Việt Nam. | Nielsen #2: Match System | Fail | Lỗi định dạng: Dòng thông tin phụ 'Export date: 7/28/2026' hiển thị sai định dạng Việt Nam (m/d/yyyy), không nhất quán với cột dữ liệu 'Created At' vốn dùng dd/mm/yyyy. [Xem ảnh](images/bug-defect/Screen-C3-IA-02-09.jpg) |
| IA-02-10 | Forms | Nút xóa nhanh (clear button) hoặc reset form hoạt động chính xác. | Nielsen #3: User Control | N/A | |
| IA-02-11 | Forms | Trình duyệt hỗ trợ tính năng tự động điền (autofill) cho các trường thông tin cơ bản. | Nielsen #7: Flexibility | N/A | |
| IA-02-12 | Forms | Ô nhập mật khẩu hỗ trợ tính năng toggle ẩn/hiện mật khẩu trực quan bằng biểu tượng con mắt. | Nielsen #7: Flexibility | N/A | |
| **IA-03** | **Navigation** | **IA-03: Navigation (Menus, Breadcrumbs, Sidebar, Tabs, Back actions, Deep links)** | | | |
| IA-03-01 | Navigation | Menu điều hướng chính luôn cố định hoặc dễ dàng truy cập ở đầu trang/thanh bên. | Nielsen #6: Recognition | N/A | |
| IA-03-02 | Navigation | Trạng thái hiện tại của trang (Active state) được làm nổi bật trên menu điều hướng. | Nielsen #1: Visibility | N/A | |
| IA-03-03 | Navigation | Nút quay lại (Back/Return action) đưa người dùng về đúng trang trước đó, không mất trạng thái. | Nielsen #3: User Control | N/A | |
| IA-03-04 | Navigation | Liên kết sâu (Deep links) dẫn trực tiếp đến trang chi tiết sự kiện mà không bị lỗi 404. | Nielsen #4: Consistency | N/A | |
| IA-03-05 | Navigation | Breadcrumbs hiển thị đúng phân cấp thư mục và có thể click để quay về thư mục cha. | Nielsen #6: Recognition | N/A | |
| IA-03-06 | Navigation | Tính năng kéo thả thay đổi thứ tự (Reorder) hiển thị trực quan (dòng bị kéo mờ opacity-50) và các nút thao tác khác tạm thời bị vô hiệu hóa. | Norman: Feedback | N/A | |
| IA-03-07 | Navigation | Các tab chuyển đổi nhanh hoạt động độc lập và tải đúng dữ liệu tương ứng. | Nielsen #7: Flexibility | N/A | |
| IA-03-08 | Navigation | Không có liên kết nào bị hỏng (Broken links / 404 error) trên toàn giao diện. | Nielsen #4: Consistency | N/A | |
| IA-03-09 | Navigation | Nút "Cuộn lên đầu trang" (Back to top) hiển thị khi người dùng cuộn xuống sâu (nếu có). | Nielsen #7: Flexibility | N/A | |
| IA-03-10 | Navigation | Thanh bên sidebar có thể thu gọn/mở rộng mượt mà và không che khuất nội dung chính. | Nielsen #3: User Control | N/A | |
| IA-03-11 | Navigation | Đường dẫn URL trên thanh địa chỉ thay đổi tương ứng khi chuyển đổi qua lại giữa các tab hoặc bộ lọc. | Nielsen #4: Consistency | N/A | |
| IA-03-12 | Navigation | Giao diện kéo thả (Reorder) hiển thị biểu tượng tay cầm (drag handle) rõ ràng để gợi ý khả năng tương tác. | Norman: Signifiers | N/A | |
| **IA-04** | **Feedback** | **IA-04: Feedback & State (Toasts, Badges, Confirmations, Progress Bars, Status Colors)** | | | |
| IA-04-01 | Feedback | Thông báo nổi (Toasts) xuất hiện ngay sau khi thực hiện hành động và tự động tắt sau 3-5s. | Norman: Feedback | Fail | Lỗi Toast: Giao diện hệ thống không hiển thị bất kỳ thông báo Toast success nào để xác nhận việc xuất dữ liệu và tải file Excel hoàn tất. [Xem ảnh](images/bug-defect/Screen-C3-IA-04-01.jpg) |
| IA-04-02 | Feedback | Toasts có màu sắc phân biệt rõ ràng: Xanh (Thành công), Đỏ (Lỗi), Vàng (Cảnh báo). | Nielsen #8: Aesthetic | N/A | |
| IA-04-03 | Feedback | Hộp thoại xác nhận (Confirmation dialog) xuất hiện trước các hành động hủy/xóa quan trọng. | Nielsen #5: Error Prev. | N/A | |
| IA-04-04 | Feedback | Huy hiệu (Badges) hiển thị chính xác số lượng thông báo; trạng thái vé thay đổi tương ứng khi được phê duyệt/hủy. | Nielsen #1: Visibility | N/A | |
| IA-04-05 | Feedback | Thanh tiến trình (Progress bar) hoặc vòng xoay tải (Spinner) xuất hiện khi hệ thống xử lý. | Nielsen #1: Visibility | N/A | |
| IA-04-06 | Feedback | Trạng thái hiển thị màu sắc tương thích với ngữ nghĩa (Ví dụ: APPROVED màu xanh lá, REJECTED màu đỏ). | Nielsen #2: Match System | N/A | |
| IA-04-07 | Feedback | Chấm đỏ thông báo (Notification dot) hiển thị động ngay khi có thay đổi trạng thái đăng ký. | Nielsen #1: Visibility | N/A | |
| IA-04-08 | Feedback | Hộp thoại chi tiết ảnh (Lightbox) mở rộng mượt mà khi click vào ảnh đính kèm. | Nielsen #7: Flexibility | N/A | |
| IA-04-09 | Feedback | Cập nhật dữ liệu thời gian thực (Real-time update) mà không cần người dùng reload trang. | Norman: Feedback | Pass | |
| IA-04-10 | Feedback | Hiển thị thông báo rõ ràng khi mất kết nối mạng Internet. | Nielsen #1: Visibility | Fail | Lỗi ngoại tuyến: Khi nhấn nút 'Export' lúc mất kết nối mạng, hệ thống không đưa ra bất cứ phản hồi hay thông điệp cảnh báo nào (im lặng hoàn toàn). [Xem ảnh](images/bug-defect/Screen-C3-IA-04-10.jpg) |
| IA-04-11 | Feedback | Hệ thống vô hiệu hóa nút gửi hoặc ngăn chặn gửi dữ liệu trùng lặp khi người dùng click đúp nút Submit. | Nielsen #5: Error Prev. | N/A | |
| IA-04-12 | Feedback | Mã QR/Barcode trên vé hiển thị rõ nét (không bị mờ), có kích thước tối thiểu đảm bảo quét được bằng ứng dụng camera thông thường. | Nielsen #1: Visibility | N/A | |
| IA-04-13 | Feedback | Ô nhập liệu (text box) hiển thị hiệu ứng viền/nổi bật trực quan (focus state) khi nhấp chuột vào để người dùng nhận biết rõ ràng đang thao tác/nhập liệu. | Norman: Feedback | N/A | |
| IA-04-14 | Feedback | Các nút secondary actions phải được vô hiệu hóa (disabled + đổi con trỏ) khi không có gì để thực hiện, hoặc phải hiển thị phản hồi rõ ràng (toast/thông báo) nếu vẫn cho phép bấm mà không có tác dụng gì | Norman: Feedback + Signifiers | N/A | |

**C4 - Delete User Confirmation Dialog & Audit Logs:**

| ID | Khía Cạnh | Mục Kiểm Tra (Checklist Item Description) | Ánh Xạ Heuristics / Nguyên Tắc | Screen 4 - C4 (Pass/Fail/NA) | Ghi Chú Lỗi (Notes) |
|---|---|---|---|---|---|
| **IA-01** | **General UI** | **IA-01: General UI Standards (Layout, Typography, Color, Consistency, i18n)** | | | |
| IA-01-01 | General UI | Hệ thống lưới và khoảng cách (Grid & Spacing) căn lề nhất quán trên toàn màn hình. | Nielsen #4: Consistency | Pass | |
| IA-01-02 | General UI | Font chữ (typography) nhất quán về kích thước, độ dày (bold/regular) và phân cấp tiêu đề. | Nielsen #4: Consistency | Pass | |
| IA-01-03 | General UI | Màu sắc của các nút hành động (Primary, Secondary) và trạng thái nhất quán. | Norman: Signifiers | Pass | |
| IA-01-04 | General UI | Đa ngôn ngữ (EN/VI) hoạt động đầy đủ, không bị dịch thiếu hoặc chồng lấp chữ. | Nielsen #4: Consistency | Pass | |
| IA-01-05 | General UI | Trạng thái rỗng (Empty state) được hiển thị rõ ràng khi không có sự kiện/dữ liệu nào. | Nielsen #1: Visibility | Pass | |
| IA-01-06 | General UI | Trạng thái đang tải (Loading state/skeleton) hiển thị khi kéo dữ liệu chậm. | Nielsen #1: Visibility | N/A | |
| IA-01-07 | General UI | Trang web tương thích tốt và tự động co giãn (Responsive) trên màn hình. | Nielsen #4: Consistency | Fail | Lỗi responsive: Bảng danh sách bị vỡ cột trên màn hình di động nhỏ (iPhone SE). Hộp thoại xác nhận xóa cũng xuất hiện lệch ngoài khung nhìn hiển thị, phải cuộn trang thủ công để tìm. [Xem ảnh](images/bug-defect/Screen-C4-IA-01-07.jpg) |
| IA-01-08 | General UI | Các hình ảnh (Thumbnail/Banner) không bị méo tỉ lệ hiển thị (tỷ lệ 4:3 và 24:9) trên các kích thước màn hình khác nhau. | Shneiderman: Aesthetics | N/A | |
| IA-01-09 | General UI | Các icon được căn chỉnh đúng tâm so với nhãn text bên cạnh. | Shneiderman: Aesthetics | Pass | |
| IA-01-10 | General UI | Độ tương phản màu sắc giữa văn bản và nền đủ rõ ràng (Accessibility WCAG). | Nielsen #4: Consistency | Pass | |
| IA-01-11 | General UI | Các liên kết ngoài (External links) mở ở tab mới, liên kết nội bộ (Internal links) mở ở tab hiện tại. | Nielsen #3: User Control | N/A | |
| IA-01-12 | General UI | Ảnh Thumbnail (4:3) và Banner (24:9) không bị cắt xén mất nội dung quan trọng. | Nielsen #4: Consistency | N/A | |
| **IA-02** | **Forms** | **IA-02: Forms (Labels, Validation, Errors, Required Fields, Rich Text)** | | | |
| IA-02-01 | Forms | Các trường bắt buộc nhập (Required fields) được đánh dấu ký hiệu trực quan (ví dụ dấu `*`). | Norman: Constraints | N/A | |
| IA-02-02 | Forms | Nhãn (Labels) của trường nhập liệu luôn hiển thị rõ ràng và đi sát với ô nhập liệu. | Nielsen #6: Recognition | N/A | |
| IA-02-03 | Forms | Validation thời gian thực báo lỗi đỏ trực quan ngay dưới trường nhập liệu bị lỗi. | Nielsen #5: Error Prev. | N/A | |
| IA-02-04 | Forms | Thông báo lỗi cụ thể, hướng dẫn cách khắc phục thay vì báo lỗi chung chung. | Nielsen #10: Help & Error | N/A | |
| IA-02-05 | Forms | Định dạng tải lên (Upload file/image) kiểm tra đúng định dạng và dung lượng tối đa. | Norman: Constraints | N/A | |
| IA-02-06 | Forms | Trình soạn thảo Rich Text hiển thị đầy đủ thanh công cụ và hoạt động mượt mà. | Nielsen #7: Flexibility | N/A | |
| IA-02-07 | Forms | Người dùng có thể nhấn `Tab` để di chuyển tuần tự qua các ô nhập liệu trong form. | Nielsen #7: Flexibility | N/A | |
| IA-02-08 | Forms | Các nút Submit/Save bị vô hiệu hóa (disabled) khi form chưa điền đủ thông tin hợp lệ. | Nielsen #5: Error Prev. | N/A | |
| IA-02-09 | Forms | Định dạng ngày giờ hiển thị theo chuẩn cục bộ dễ đọc đối với người dùng Việt Nam. | Nielsen #2: Match System | Pass | |
| IA-02-10 | Forms | Nút xóa nhanh (clear button) hoặc reset form hoạt động chính xác. | Nielsen #3: User Control | N/A | |
| IA-02-11 | Forms | Trình duyệt hỗ trợ tính năng tự động điền (autofill) cho các trường thông tin cơ bản. | Nielsen #7: Flexibility | N/A | |
| IA-02-12 | Forms | Ô nhập mật khẩu hỗ trợ tính năng toggle ẩn/hiện mật khẩu trực quan bằng biểu tượng con mắt. | Nielsen #7: Flexibility | N/A | |
| **IA-03** | **Navigation** | **IA-03: Navigation (Menus, Breadcrumbs, Sidebar, Tabs, Back actions, Deep links)** | | | |
| IA-03-01 | Navigation | Menu điều hướng chính luôn cố định hoặc dễ dàng truy cập ở đầu trang/thanh bên. | Nielsen #6: Recognition | N/A | |
| IA-03-02 | Navigation | Trạng thái hiện tại của trang (Active state) được làm nổi bật trên menu điều hướng. | Nielsen #1: Visibility | N/A | |
| IA-03-03 | Navigation | Nút quay lại (Back/Return action) đưa người dùng về đúng trang trước đó, không mất trạng thái. | Nielsen #3: User Control | Pass | |
| IA-03-04 | Navigation | Liên kết sâu (Deep links) dẫn trực tiếp đến trang chi tiết sự kiện mà không bị lỗi 404. | Nielsen #4: Consistency | N/A | |
| IA-03-05 | Navigation | Breadcrumbs hiển thị đúng phân cấp thư mục và có thể click để quay về thư mục cha. | Nielsen #6: Recognition | N/A | |
| IA-03-06 | Navigation | Tính năng kéo thả thay đổi thứ tự (Reorder) hiển thị trực quan (dòng bị kéo mờ opacity-50) và các nút thao tác khác tạm thời bị vô hiệu hóa. | Norman: Feedback | N/A | |
| IA-03-07 | Navigation | Các tab chuyển đổi nhanh hoạt động độc lập và tải đúng dữ liệu tương ứng. | Nielsen #7: Flexibility | N/A | |
| IA-03-08 | Navigation | Không có liên kết nào bị hỏng (Broken links / 404 error) trên toàn giao diện. | Nielsen #4: Consistency | N/A | |
| IA-03-09 | Navigation | Nút "Cuộn lên đầu trang" (Back to top) hiển thị khi người dùng cuộn xuống sâu (nếu có). | Nielsen #7: Flexibility | N/A | |
| IA-03-10 | Navigation | Thanh bên sidebar có thể thu gọn/mở rộng mượt mà và không che khuất nội dung chính. | Nielsen #3: User Control | N/A | |
| IA-03-11 | Navigation | Đường dẫn URL trên thanh địa chỉ thay đổi tương ứng khi chuyển đổi qua lại giữa các tab hoặc bộ lọc. | Nielsen #4: Consistency | N/A | |
| IA-03-12 | Navigation | Giao diện kéo thả (Reorder) hiển thị biểu tượng tay cầm (drag handle) rõ ràng để gợi ý khả năng tương tác. | Norman: Signifiers | N/A | |
| **IA-04** | **Feedback** | **IA-04: Feedback & State (Toasts, Badges, Confirmations, Progress Bars, Status Colors)** | | | |
| IA-04-01 | Feedback | Thông báo nổi (Toasts) xuất hiện ngay sau khi thực hiện hành động và tự động tắt sau 3-5s. | Norman: Feedback | Fail | Lỗi phản hồi: Giao diện không hiển thị thông báo Toast success nào sau khi xóa người dùng thành công để xác nhận thao tác. [Xem ảnh](images/bug-defect/Screen-C4-IA-04-01a.jpg) [Xem ảnh](images/bug-defect/Screen-C4-IA-04-01b.jpg) |
| IA-04-02 | Feedback | Toasts có màu sắc phân biệt rõ ràng: Xanh (Thành công), Đỏ (Lỗi), Vàng (Cảnh báo). | Nielsen #8: Aesthetic | N/A | |
| IA-04-03 | Feedback | Hộp thoại xác nhận (Confirmation dialog) xuất hiện trước các hành động hủy/xóa quan trọng. | Nielsen #5: Error Prev. | Pass | |
| IA-04-04 | Feedback | Huy hiệu (Badges) hiển thị chính xác số lượng thông báo; trạng thái vé thay đổi tương ứng khi được phê duyệt/hủy. | Nielsen #1: Visibility | N/A | |
| IA-04-05 | Feedback | Thanh tiến trình (Progress bar) hoặc vòng xoay tải (Spinner) xuất hiện khi hệ thống xử lý. | Nielsen #1: Visibility | Pass | |
| IA-04-06 | Feedback | Trạng thái hiển thị màu sắc tương thích với ngữ nghĩa (Ví dụ: APPROVED màu xanh lá, REJECTED màu đỏ). | Nielsen #2: Match System | Pass | |
| IA-04-07 | Feedback | Chấm đỏ thông báo (Notification dot) hiển thị động ngay khi có thay đổi trạng thái đăng ký. | Nielsen #1: Visibility | N/A | |
| IA-04-08 | Feedback | Hộp thoại chi tiết ảnh (Lightbox) mở rộng mượt mà khi click vào ảnh đính kèm. | Nielsen #7: Flexibility | N/A | |
| IA-04-09 | Feedback | Cập nhật dữ liệu thời gian thực (Real-time update) mà không cần người dùng reload trang. | Norman: Feedback | N/A | |
| IA-04-10 | Feedback | Hiển thị thông báo rõ ràng khi mất kết nối mạng Internet. | Nielsen #1: Visibility | Fail | Lỗi ngoại tuyến: Khi mất mạng, nút Xác nhận trong hộp thoại xóa nhấn vào không đưa ra bất kỳ phản hồi hay cảnh báo lỗi nào (im lặng hoàn toàn). [Xem ảnh](images/bug-defect/Screen-C4-IA-04-10.jpg) |
| IA-04-11 | Feedback | Hệ thống vô hiệu hóa nút gửi hoặc ngăn chặn gửi dữ liệu trùng lặp khi người dùng click đúp nút Submit. | Nielsen #5: Error Prev. | Pass | |
| IA-04-12 | Feedback | Mã QR/Barcode trên vé hiển thị rõ nét (không bị mờ), có kích thước tối thiểu đảm bảo quét được bằng ứng dụng camera thông thường. | Nielsen #1: Visibility | N/A | |
| IA-04-13 | Feedback | Ô nhập liệu (text box) hiển thị hiệu ứng viền/nổi bật trực quan (focus state) khi nhấp chuột vào để người dùng nhận biết rõ ràng đang thao tác/nhập liệu. | Norman: Feedback | N/A | |
| IA-04-14 | Feedback | Các nút secondary actions phải được vô hiệu hóa (disabled + đổi con trỏ) khi không có gì để thực hiện, hoặc phải hiển thị phản hồi rõ ràng (toast/thông báo) nếu vẫn cho phép bấm mà không có tác dụng gì | Norman: Feedback + Signifiers | Pass | |

## Task 2: User Testing & Usability Report

### 1. Kịch Bản Kiểm Thử (Task Scenario)

**Mục tiêu:** Đánh giá mức độ dễ dàng và tính thân thiện của hệ thống đối với người quản trị (Admin) khi thực hiện các nghiệp vụ quản lý người dùng (C1, C2, C3, C4).

#### Bối cảnh nghiệp vụ
Mỗi tài khoản trong hệ thống có 4 vai trò bao gồm:
1. Quản trị - Admin
2. Khách - Guest
3. Giảng viên - Lecturer
4. Sinh viên - Student 

Và 2 trạng thái bao gồm:
1. Hoạt động - Active
2. Không hoạt động - Inactive

#### Kịch bản (Dành cho người tham gia)
"Bạn là một quản trị viên (Admin) của hệ thống quản lý sự kiện. Nhiệm vụ của bạn là sử dụng hệ thống để quản lý tài khoản người dùng với các công việc sau:
- Tìm kiếm, lọc và xem thông tin trên danh sách người dùng.
- Tạo một người dùng mới và phân quyền cho người đó.
- Xuất danh sách người dùng hiện tại ra file Excel để lưu trữ báo cáo.
- Tìm và xóa một người dùng không còn hoạt động, sau đó xác nhận hoàn tất thao tác xóa."

*(Lưu ý: Chỉ đưa ra kịch bản và mục tiêu để người dùng tự khám phá, không hướng dẫn chi tiết từng bước click chuột vào đâu).*

---

### 2. Bảng Câu Hỏi SUS (SUS Questionare)

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

### 3. Báo Cáo Kết Quả Kiểm Thử

#### 3.1. Danh sách người tham gia (Participants)

| STT | Họ và tên | Đối tượng (Role) | Thông tin liên hệ |
|---|---|---|---|
| 1 | Nguyễn Tấn Đạt | Sinh viên năm 3 | 033xxxx851 |
| 2 | Nguyễn Thị Cẩm Nhung | Developer (tương tác nhiều với công nghệ) | 090xxxx048 |
| 3 | Nguyễn Tuấn Kiệt | Sinh viên năm 1 | 033xxxx507 |
| 4 | Dương Thúy Mi | Giáo viên | 093xxxx202 |

---

#### 3.2. Bảng số liệu kiểm thử (Metrics Table)

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

#### 3.3. Chi tiết câu hỏi SUS và Cách tính điểm (SUS Scoring Details)

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

#### 3.4. Nhật ký quan sát chi tiết từng phiên (Per-Session Observation Notes)

**Phiên kiểm thử số 1: Nguyễn Tấn Đạt**
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

**Phiên kiểm thử số 2: Nguyễn Thị Cẩm Nhung**
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

**Phiên kiểm thử số 3: Nguyễn Tuấn Kiệt**
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

**Phiên kiểm thử số 4: Dương Thúy Mi**
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

#### 3.5. Phân tích lỗi & Vấn đề (Ranked Findings)

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

#### 3.6. Đề xuất cải thiện ưu tiên (Prioritized Recommendations)

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

### 4. Đường Dẫn Minh Chứng Quay Video Màn Hình (Screen Recordings)

Để xác thực tính xác thực của các phiên thử nghiệm khả dụng, toàn bộ video quay màn hình và âm thanh quá trình thực hiện kịch bản của các người tham gia đã được tải lên thư mục lưu trữ trực tuyến:

- **Đường dẫn thư mục Google Drive chứa video:** [Liên kết Google Drive](https://drive.google.com/drive/folders/1BoebOJamcK_G9Xbpi6mvRKpUjvctfNwq?usp=sharing)
- **Đường dẫn trực tiếp đến thư mục Google Drive chứa video:** https://drive.google.com/drive/folders/1BoebOJamcK_G9Xbpi6mvRKpUjvctfNwq?usp=sharing
- **Danh sách file video minh chứng:**
  - `User-1.mp4`
  - `User-2.mp4`
  - `User-3.mp4`
  - `User-4.mp4`

## Task 3: Cross-Browser / Cross-Platform

### 1. C1 - Users List — Search, Role/Active Filters, Columns

| Run ID | Thiết bị (Device) | Hệ điều hành (OS) | Trình duyệt (Browser) | Kết quả (Pass/Fail) & Ghi chú lỗi | Screenshot Link |
|---|---|---|---|---|---|
| C1-Run-01 | Desktop | Windows 11 | Chrome | Pass | [Xem ảnh](images/cross-testing/C1-Desktop-Windows-Chrome.jpg) |
| C1-Run-02 | Desktop | Windows 11 | Opera | Pass | [Xem ảnh](images/cross-testing/C1-Desktop-Windows-Opera.jpg) |
| C1-Run-03 | Desktop | Windows 11 | Edge | Pass | [Xem ảnh](images/cross-testing/C1-Desktop-Windows-Edge.jpg) |
| C1-Run-04 | Desktop | Windows 11 | Firefox | Pass | [Xem ảnh](images/cross-testing/C1-Desktop-Windows-Firefox.jpg) |
| C1-Run-05 | Desktop | macOS 14 | Safari | Pass | [Xem ảnh](images/cross-testing/C1-Desktop-macOS-Safari.jpg) |
| C1-Run-06 | Tablet | Android 15 | Chrome | Pass | [Xem ảnh](images/cross-testing/C1-Tablet-Android-Chrome.jpg) |
| C1-Run-07 | Phone | Android 16 | Chrome | Fail (Bảng thông tin của các User mất hết toàn bộ các cột, chỉ còn đúng cột Actions (Hành động) để chỉnh sửa/xóa User) | [Xem ảnh](images/cross-testing/C1-Phone-Android-Chrome.jpg) |

<br>

### 2. C2 - Create / Edit User & Assign Role

| Run ID | Thiết bị (Device) | Hệ điều hành (OS) | Trình duyệt (Browser) | Kết quả (Pass/Fail) & Ghi chú lỗi | Screenshot Link |
|---|---|---|---|---|---|
| C2-Run-01 | Desktop | Windows 11 | Chrome | Pass | [Xem ảnh](images/cross-testing/C2-Desktop-Windows-Chrome.jpg) |
| C2-Run-02 | Desktop | Windows 11 | Opera | Pass | [Xem ảnh](images/cross-testing/C2-Desktop-Windows-Opera.jpg) |
| C2-Run-03 | Desktop | Windows 11 | Edge | Pass | [Xem ảnh](images/cross-testing/C2-Desktop-Windows-Edge.jpg) |
| C2-Run-04 | Desktop | Windows 11 | Firefox | Pass | [Xem ảnh](images/cross-testing/C2-Desktop-Windows-Firefox.jpg) |
| C2-Run-05 | Desktop | macOS 14 | Safari | Pass | [Xem ảnh](images/cross-testing/C2-Desktop-macOS-Safari.jpg) |
| C2-Run-06 | Tablet | Android 15 | Chrome | Pass | [Xem ảnh](images/cross-testing/C2-Tablet-Android-Chrome.jpg) |
| C2-Run-07 | Phone | Android 16 | Chrome | Fail (Dialog tạo User mới rất nhỏ, khó có thể thao tác/chọn trên điện thoại được và cũng không thể xác định được User đã tạo mới hay chưa do không thấy nội dung bảng) | [Xem ảnh](images/cross-testing/C2-Phone-Android-Chrome.jpg) |

<br>

### 3. C3 - Export to Excel — Column Completeness and Download Feedback

| Run ID | Thiết bị (Device) | Hệ điều hành (OS) | Trình duyệt (Browser) | Kết quả (Pass/Fail) & Ghi chú lỗi | Screenshot Link |
|---|---|---|---|---|---|
| C3-Run-01 | Desktop | Windows 11 | Chrome | Fail (Thao tác xuất thành công nhưng tệp mở ra bị cảnh báo lỗi cấu trúc BUG-C3-01) | [Xem ảnh](images/cross-testing/C3-Desktop-Windows-Chrome-1.jpg) <br> [Xem ảnh](images/cross-testing/C3-Desktop-Windows-Chrome-2.jpg) |
| C3-Run-02 | Desktop | Windows 11 | Opera | Fail (Thao tác xuất thành công nhưng tệp mở ra bị cảnh báo lỗi cấu trúc như C3-Run-01) | [Xem ảnh](images/cross-testing/C3-Desktop-Windows-Opera-1.jpg) <br> [Xem ảnh](images/cross-testing/C3-Desktop-Windows-Opera-2.jpg) |
| C3-Run-03 | Desktop | Windows 11 | Edge | Fail (Thao tác xuất thành công nhưng tệp mở ra bị cảnh báo lỗi cấu trúc như C3-Run-01) | [Xem ảnh](images/cross-testing/C3-Desktop-Windows-Edge-1.jpg) <br> [Xem ảnh](images/cross-testing/C3-Desktop-Windows-Edge-2.jpg) |
| C3-Run-04 | Desktop | Windows 11 | Firefox | Fail (Thao tác xuất thành công nhưng tệp mở ra bị cảnh báo lỗi cấu trúc như C3-Run-01) | [Xem ảnh](images/cross-testing/C3-Desktop-Windows-Firefox-1.jpg) <br> [Xem ảnh](images/cross-testing/C3-Desktop-Windows-Firefox-2.jpg) |
| C3-Run-05 | Desktop | macOS 14 | Safari | Pass | [Xem ảnh](images/cross-testing/C3-Desktop-macOS-Safari-1.jpg) <br> [Xem ảnh](images/cross-testing/C3-Desktop-macOS-Safari-2.jpg) <br> [Xem ảnh](images/cross-testing/C3-Desktop-macOS-Safari-3.jpg) |
| C3-Run-06 | Tablet | Android 15 | Chrome | Pass | [Xem ảnh](images/cross-testing/C3-Tablet-Android-Chrome-1.jpg) <br> [Xem ảnh](images/cross-testing/C3-Tablet-Android-Chrome-2.jpg) |
| C3-Run-07 | Phone | Android 16 | Chrome | Pass | [Xem ảnh](images/cross-testing/C3-Phone-Android-Chrome-1.jpg) <br> [Xem ảnh](images/cross-testing/C3-Phone-Android-Chrome-2.jpg) |

<br>

### 4. C4 - Delete User Confirmation Dialog & Audit Logs

| Run ID | Thiết bị (Device) | Hệ điều hành (OS) | Trình duyệt (Browser) | Kết quả (Pass/Fail) & Ghi chú lỗi | Screenshot Link |
|---|---|---|---|---|---|
| C4-Run-01 | Desktop | Windows 11 | Chrome | Pass | [Xem ảnh](images/cross-testing/C4-Desktop-Windows-Chrome.jpg) |
| C4-Run-02 | Desktop | Windows 11 | Opera | Pass | [Xem ảnh](images/cross-testing/C4-Desktop-Windows-Opera.jpg) |
| C4-Run-03 | Desktop | Windows 11 | Edge | Pass | [Xem ảnh](images/cross-testing/C4-Desktop-Windows-Edge.jpg) |
| C4-Run-04 | Desktop | Windows 11 | Firefox | Pass | [Xem ảnh](images/cross-testing/C4-Desktop-Windows-Firefox.jpg) |
| C4-Run-05 | Desktop | macOS 14 | Safari | Pass | [Xem ảnh](images/cross-testing/C4-Desktop-macOS-Safari.jpg) |
| C4-Run-06 | Tablet | Android 15 | Chrome | Pass | [Xem ảnh](images/cross-testing/C4-Tablet-Android-Chrome.jpg) |
| C4-Run-07 | Phone | Android 16 | Chrome | Fail (Dialog xóa User rất nhỏ và để xem hết toàn bộ dialog thì phải kéo nhỏ hết mức hay kéo màn hình sang vị trí dialog, đồng thời không thể thấy Audit Logs created hay updated do bảng mất hầu như toàn bộ các cột) | [Xem ảnh](images/cross-testing/C4-Phone-Android-Chrome.jpg) |