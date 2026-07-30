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
| IA-01-04 | General UI | Đa ngôn ngữ (EN/VI) hoạt động đầy đủ, không bị dịch thiếu hoặc chồng lấp chữ. | Nielsen #4: Consistency | Fail | Lỗi i18n: Tại ô nhập liệu phân trang 'Đến trang', khi thiết lập giao diện tiếng Việt và nhập giá trị không hợp lệ (ví dụ: nhập số trang vượt quá giới hạn như 11/10, hoặc số âm như -1), trình duyệt hiển thị thông báo lỗi bằng tiếng Anh ('Value must be less than or equal to...' / 'Value must be greater than or equal to...') thay vì tiếng Việt. |
| IA-01-05 | General UI | Trạng thái rỗng (Empty state) được hiển thị rõ ràng khi không có sự kiện/dữ liệu nào. | Nielsen #1: Visibility | Pass | |
| IA-01-06 | General UI | Trạng thái đang tải (Loading state/skeleton) hiển thị khi kéo dữ liệu chậm. | Nielsen #1: Visibility | Pass | |
| IA-01-07 | General UI | Trang web tương thích tốt và tự động co giãn (Responsive) trên màn hình. | Nielsen #4: Consistency | Fail | Lỗi responsive: Sidebar không tự động thu gọn lại khi thu nhỏ màn hình trình duyệt, dẫn đến các cột thông tin của bảng Users list bị che khuất và không thể xem được đầy đủ dữ liệu (chỉ hiển thị đủ khi Admin chủ động click thu gọn sidebar thủ công). |
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
| IA-04-09 | Feedback | Cập nhật dữ liệu thời gian thực (Real-time update) mà không cần người dùng reload trang. | Norman: Feedback | Fail | Hệ thống không tự động cập nhật danh sách người dùng theo thời gian thực. Khi chỉnh sửa tên user ở tab Admin 1 (ví dụ đổi từ "def abc" thành "B A"), tab Admin 2 bên cạnh vẫn hiển thị tên cũ là "def abc" cho đến khi reload trang thủ công. |
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
| IA-01-04 | General UI | Đa ngôn ngữ (EN/VI) hoạt động đầy đủ, không bị dịch thiếu hoặc chồng lấp chữ. | Nielsen #4: Consistency | Fail | Lỗi i18n: Khi nhập email không đúng định dạng trong form "Tạo người dùng mới", thông báo lỗi của trình duyệt hiển thị bằng tiếng Anh ("Please include an '@' in the email address..."), trong khi các trường lỗi khác và toàn bộ giao diện đang hiển thị tiếng Việt bình thường. |
| IA-01-05 | General UI | Trạng thái rỗng (Empty state) được hiển thị rõ ràng khi không có sự kiện/dữ liệu nào. | Nielsen #1: Visibility | N/A | |
| IA-01-06 | General UI | Trạng thái đang tải (Loading state/skeleton) hiển thị khi kéo dữ liệu chậm. | Nielsen #1: Visibility | N/A | |
| IA-01-07 | General UI | Trang web tương thích tốt và tự động co giãn (Responsive) trên màn hình. | Nielsen #4: Consistency | Fail | Lỗi responsive: Khi hiển thị trên các màn hình nhỏ (như thiết bị di động), form Create User bị thu nhỏ kích thước (zoom out) quá mức, dẫn đến chữ và các trường nhập liệu cực kỳ nhỏ, rất khó để Admin nhìn rõ và nhấp chọn chính xác. |
| IA-01-08 | General UI | Các hình ảnh (Thumbnail/Banner) không bị méo tỉ lệ hiển thị (tỷ lệ 4:3 và 24:9) trên các kích thước màn hình khác nhau. | Shneiderman: Aesthetics | N/A | |
| IA-01-09 | General UI | Các icon được căn chỉnh đúng tâm so với nhãn text bên cạnh. | Shneiderman: Aesthetics | Pass | |
| IA-01-10 | General UI | Độ tương phản màu sắc giữa văn bản và nền đủ rõ ràng (Accessibility WCAG). | Nielsen #4: Consistency | Pass | |
| IA-01-11 | General UI | Các liên kết ngoài (External links) mở ở tab mới, liên kết nội bộ (Internal links) mở ở tab hiện tại. | Nielsen #3: User Control | N/A | |
| IA-01-12 | General UI | Ảnh Thumbnail (4:3) và Banner (24:9) không bị cắt xén mất nội dung quan trọng. | Nielsen #4: Consistency | N/A | |
| **IA-02** | **Forms** | **IA-02: Forms (Labels, Validation, Errors, Required Fields, Rich Text)** | | | |
| IA-02-01 | Forms | Các trường bắt buộc nhập (Required fields) được đánh dấu ký hiệu trực quan (ví dụ dấu `*`). | Norman: Constraints | Fail | Form "Tạo người dùng mới" không hiển thị dấu hoa thị màu đỏ `*` cạnh các trường bắt buộc, nhưng khi nhấn "Create User" hệ thống lại báo lỗi bắt buộc nhập (ví dụ: "Last name is required", "First name is required", "Role is required"). |
| IA-02-02 | Forms | Nhãn (Labels) của trường nhập liệu luôn hiển thị rõ ràng và đi sát với ô nhập liệu. | Nielsen #6: Recognition | Fail | Lỗi gợi ý (placeholder): Trong form Create User, ô nhập liệu trường First Name hiển thị placeholder gợi ý là "Last name", còn trường Last name hiển thị placeholder gợi ý là "First name" (bị tráo đổi nội dung placeholder ngược nhau). |
| IA-02-03 | Forms | Validation thời gian thực báo lỗi đỏ trực quan ngay dưới trường nhập liệu bị lỗi. | Nielsen #5: Error Prev. | Fail | Không có validation thời gian thực cho trường email (ví dụ nhập "a" nhưng không báo lỗi gì trước khi submit). Chỉ sau khi nhấn "Create User" thì lỗi mới được hiển thị. |
| IA-02-04 | Forms | Thông báo lỗi cụ thể, hướng dẫn cách khắc phục thay vì báo lỗi chung chung. | Nielsen #10: Help & Error | Fail | Lỗi nội dung thông báo: Khi người dùng nhập email thiếu tên miền (ví dụ: "abc@abccom"), hệ thống báo lỗi chung chung là "Invalid email address" thay vì chỉ dẫn rõ ràng là người dùng đang thiếu đuôi tên miền (domain extension). |
| IA-02-05 | Forms | Định dạng tải lên (Upload file/image) kiểm tra đúng định dạng và dung lượng tối đa. | Norman: Constraints | N/A | |
| IA-02-06 | Forms | Trình soạn thảo Rich Text hiển thị đầy đủ thanh công cụ và hoạt động mượt mà. | Nielsen #7: Flexibility | N/A | |
| IA-02-07 | Forms | Người dùng có thể nhấn `Tab` để di chuyển tuần tự qua các ô nhập liệu trong form. | Nielsen #7: Flexibility | Pass | |
| IA-02-08 | Forms | Các nút Submit/Save bị vô hiệu hóa (disabled) khi form chưa điền đủ thông tin hợp lệ. | Nielsen #5: Error Prev. | Fail | Nút "Create User" vẫn có thể nhấn được (không bị disabled hay chuyển màu xám) ngay cả khi form chưa hợp lệ (ví dụ bỏ trống email, nhập số điện thoại sai định dạng là "a"). |
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
| IA-04-01 | Feedback | Thông báo nổi (Toasts) xuất hiện ngay sau khi thực hiện hành động và tự động tắt sau 3-5s. | Norman: Feedback | Fail | Không hiển thị Toast thông báo sau khi tạo người dùng thành công để xác nhận hành động đã hoàn tất. |
| IA-04-02 | Feedback | Toasts có màu sắc phân biệt rõ ràng: Xanh (Thành công), Đỏ (Lỗi), Vàng (Cảnh báo). | Nielsen #8: Aesthetic | N/A | |
| IA-04-03 | Feedback | Hộp thoại xác nhận (Confirmation dialog) xuất hiện trước các hành động hủy/xóa quan trọng. | Nielsen #5: Error Prev. | N/A | |
| IA-04-04 | Feedback | Huy hiệu (Badges) hiển thị chính xác số lượng thông báo; trạng thái vé thay đổi tương ứng khi được phê duyệt/hủy. | Nielsen #1: Visibility | N/A | |
| IA-04-05 | Feedback | Thanh tiến trình (Progress bar) hoặc vòng xoay tải (Spinner) xuất hiện khi hệ thống xử lý. | Nielsen #1: Visibility | Pass | |
| IA-04-06 | Feedback | Trạng thái hiển thị màu sắc tương thích với ngữ nghĩa (Ví dụ: APPROVED màu xanh lá, REJECTED màu đỏ). | Nielsen #2: Match System | Pass | |
| IA-04-07 | Feedback | Chấm đỏ thông báo (Notification dot) hiển thị động ngay khi có thay đổi trạng thái đăng ký. | Nielsen #1: Visibility | N/A | |
| IA-04-08 | Feedback | Hộp thoại chi tiết ảnh (Lightbox) mở rộng mượt mà khi click vào ảnh đính kèm. | Nielsen #7: Flexibility | N/A | |
| IA-04-09 | Feedback | Cập nhật dữ liệu thời gian thực (Real-time update) mà không cần người dùng reload trang. | Norman: Feedback | N/A | |
| IA-04-10 | Feedback | Hiển thị thông báo rõ ràng khi mất kết nối mạng Internet. | Nielsen #1: Visibility | Fail | Khi mất kết nối mạng đột ngột và nhấn "Create User", hệ thống hiển thị thông báo lỗi thô sơ và tối nghĩa: "Failed to fetch" trực tiếp trên form thay vì đưa ra cảnh báo mất kết nối thân thiện. |
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
| IA-01-04 | General UI | Đa ngôn ngữ (EN/VI) hoạt động đầy đủ, không bị dịch thiếu hoặc chồng lấp chữ. | Nielsen #4: Consistency | Fail | Lỗi i18n: Nội dung và tiêu đề các cột trong file Excel xuất ra hiển thị cố định bằng tiếng Anh (Last Name, First Name, Card Code...), không dịch theo ngôn ngữ Việt Nam của hệ thống. |
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
| IA-02-09 | Forms | Định dạng ngày giờ hiển thị theo chuẩn cục bộ dễ đọc đối với người dùng Việt Nam. | Nielsen #2: Match System | Fail | Lỗi định dạng: Dòng thông tin phụ 'Export date: 7/28/2026' hiển thị sai định dạng Việt Nam (m/d/yyyy), không nhất quán với cột dữ liệu 'Created At' vốn dùng dd/mm/yyyy. |
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
| IA-04-01 | Feedback | Thông báo nổi (Toasts) xuất hiện ngay sau khi thực hiện hành động và tự động tắt sau 3-5s. | Norman: Feedback | Fail | Lỗi Toast: Giao diện hệ thống không hiển thị bất kỳ thông báo Toast success nào để xác nhận việc xuất dữ liệu và tải file Excel hoàn tất. |
| IA-04-02 | Feedback | Toasts có màu sắc phân biệt rõ ràng: Xanh (Thành công), Đỏ (Lỗi), Vàng (Cảnh báo). | Nielsen #8: Aesthetic | N/A | |
| IA-04-03 | Feedback | Hộp thoại xác nhận (Confirmation dialog) xuất hiện trước các hành động hủy/xóa quan trọng. | Nielsen #5: Error Prev. | N/A | |
| IA-04-04 | Feedback | Huy hiệu (Badges) hiển thị chính xác số lượng thông báo; trạng thái vé thay đổi tương ứng khi được phê duyệt/hủy. | Nielsen #1: Visibility | N/A | |
| IA-04-05 | Feedback | Thanh tiến trình (Progress bar) hoặc vòng xoay tải (Spinner) xuất hiện khi hệ thống xử lý. | Nielsen #1: Visibility | N/A | |
| IA-04-06 | Feedback | Trạng thái hiển thị màu sắc tương thích với ngữ nghĩa (Ví dụ: APPROVED màu xanh lá, REJECTED màu đỏ). | Nielsen #2: Match System | N/A | |
| IA-04-07 | Feedback | Chấm đỏ thông báo (Notification dot) hiển thị động ngay khi có thay đổi trạng thái đăng ký. | Nielsen #1: Visibility | N/A | |
| IA-04-08 | Feedback | Hộp thoại chi tiết ảnh (Lightbox) mở rộng mượt mà khi click vào ảnh đính kèm. | Nielsen #7: Flexibility | N/A | |
| IA-04-09 | Feedback | Cập nhật dữ liệu thời gian thực (Real-time update) mà không cần người dùng reload trang. | Norman: Feedback | Pass | |
| IA-04-10 | Feedback | Hiển thị thông báo rõ ràng khi mất kết nối mạng Internet. | Nielsen #1: Visibility | Fail | Lỗi ngoại tuyến: Khi nhấn nút 'Export' lúc mất kết nối mạng, hệ thống không đưa ra bất cứ phản hồi hay thông điệp cảnh báo nào (im lặng hoàn toàn). |
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
| IA-01-07 | General UI | Trang web tương thích tốt và tự động co giãn (Responsive) trên màn hình. | Nielsen #4: Consistency | Fail | Lỗi responsive: Bảng danh sách bị vỡ cột trên màn hình di động nhỏ (iPhone SE). Hộp thoại xác nhận xóa cũng xuất hiện lệch ngoài khung nhìn hiển thị, phải cuộn trang thủ công để tìm. |
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
| IA-04-01 | Feedback | Thông báo nổi (Toasts) xuất hiện ngay sau khi thực hiện hành động và tự động tắt sau 3-5s. | Norman: Feedback | Fail | Lỗi phản hồi: Giao diện không hiển thị thông báo Toast success nào sau khi xóa người dùng thành công để xác nhận thao tác. |
| IA-04-02 | Feedback | Toasts có màu sắc phân biệt rõ ràng: Xanh (Thành công), Đỏ (Lỗi), Vàng (Cảnh báo). | Nielsen #8: Aesthetic | N/A | |
| IA-04-03 | Feedback | Hộp thoại xác nhận (Confirmation dialog) xuất hiện trước các hành động hủy/xóa quan trọng. | Nielsen #5: Error Prev. | Pass | |
| IA-04-04 | Feedback | Huy hiệu (Badges) hiển thị chính xác số lượng thông báo; trạng thái vé thay đổi tương ứng khi được phê duyệt/hủy. | Nielsen #1: Visibility | N/A | |
| IA-04-05 | Feedback | Thanh tiến trình (Progress bar) hoặc vòng xoay tải (Spinner) xuất hiện khi hệ thống xử lý. | Nielsen #1: Visibility | Pass | |
| IA-04-06 | Feedback | Trạng thái hiển thị màu sắc tương thích với ngữ nghĩa (Ví dụ: APPROVED màu xanh lá, REJECTED màu đỏ). | Nielsen #2: Match System | Pass | |
| IA-04-07 | Feedback | Chấm đỏ thông báo (Notification dot) hiển thị động ngay khi có thay đổi trạng thái đăng ký. | Nielsen #1: Visibility | N/A | |
| IA-04-08 | Feedback | Hộp thoại chi tiết ảnh (Lightbox) mở rộng mượt mà khi click vào ảnh đính kèm. | Nielsen #7: Flexibility | N/A | |
| IA-04-09 | Feedback | Cập nhật dữ liệu thời gian thực (Real-time update) mà không cần người dùng reload trang. | Norman: Feedback | N/A | |
| IA-04-10 | Feedback | Hiển thị thông báo rõ ràng khi mất kết nối mạng Internet. | Nielsen #1: Visibility | Fail | Lỗi ngoại tuyến: Khi mất mạng, nút Xác nhận trong hộp thoại xóa nhấn vào không đưa ra bất kỳ phản hồi hay cảnh báo lỗi nào (im lặng hoàn toàn). |
| IA-04-11 | Feedback | Hệ thống vô hiệu hóa nút gửi hoặc ngăn chặn gửi dữ liệu trùng lặp khi người dùng click đúp nút Submit. | Nielsen #5: Error Prev. | Pass | |
| IA-04-12 | Feedback | Mã QR/Barcode trên vé hiển thị rõ nét (không bị mờ), có kích thước tối thiểu đảm bảo quét được bằng ứng dụng camera thông thường. | Nielsen #1: Visibility | N/A | |
| IA-04-13 | Feedback | Ô nhập liệu (text box) hiển thị hiệu ứng viền/nổi bật trực quan (focus state) khi nhấp chuột vào để người dùng nhận biết rõ ràng đang thao tác/nhập liệu. | Norman: Feedback | N/A | |
| IA-04-14 | Feedback | Các nút secondary actions phải được vô hiệu hóa (disabled + đổi con trỏ) khi không có gì để thực hiện, hoặc phải hiển thị phản hồi rõ ràng (toast/thông báo) nếu vẫn cho phép bấm mà không có tác dụng gì | Norman: Feedback + Signifiers | Pass | |

## Task 2: User Testing & Usability Report

## Task 3: Cross-Browser / Cross-Platform

### Compatibility Matrix

| Thiết bị (Device) | Hệ điều hành (OS) | Trình duyệt (Browser) | Kết quả (Pass/Fail) & Ghi chú lỗi | Screenshot File |
|---|---|---|---|---|
| Desktop (MacBook) | macOS 14 | Safari | Pass |  |
| Tablet (iPad) | iOS 17 | Chrome | Fail (Bảng bị tràn viền) |  |
| Phone (Galaxy S23) | Android 14 | Edge | Pass |  |