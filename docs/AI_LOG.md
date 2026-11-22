# Nhật ký sử dụng AI có trách nhiệm (AI_LOG) — Tiệm Nail Nhi Xinh

- **Sinh viên thực hiện:** Nguyễn Yến Nhi
- **Mã sinh viên:** 2071020148
- **Học phần:** FIT4014 — Thiết kế Web và Triển khai Hệ thống phần mềm
- **Công cụ AI hỗ trợ:** Gemini, GitHub Copilot

---

## 1. Bối cảnh và nhận định trước khi hỏi AI

- **Mục tiêu:** Xây dựng website tĩnh giới thiệu dịch vụ, bảng giá và biểu mẫu đặt lịch hẹn cho **Tiệm Nail Nhi Xinh** (Thôn Tứ Kì, xã Vĩnh Tường, tỉnh Phú Thọ), đảm bảo hiển thị tốt từ màn hình điện thoại hẹp (`320px`) tới màn hình máy tính (`1440px`) và triển khai công khai qua GitHub Pages.
- **Nhận định ban đầu:** Website tĩnh chỉ dùng HTML5 và CSS3 nên biểu mẫu đặt lịch cần sử dụng các thuộc tính kiểm tra hợp lệ có sẵn của trình duyệt (`required`, `minlength`, `maxlength`, `pattern`, `type="email"`) kết hợp phương thức `GET` chuyển sang trang `ket-qua.html` để mô phỏng quy trình gửi dữ liệu. Về mặt thẩm mỹ, trang web cần bảng màu hồng trầm dịu mắt thay vì các mẫu portfolio công nghệ thông thường.

---

## 2. Quá trình trao đổi, quyết định và kiểm chứng gợi ý từ AI

| Ngày | Nội dung trao đổi / Prompt | Gợi ý từ AI | Quyết định của sinh viên (Giữ / Sửa / Bỏ) | Kết quả kiểm chứng thực tế |
|---|---|---|---|---|
| 22/11/2026 | Hỏi cách tổ chức cấu trúc HTML5 ngữ nghĩa và bố cục CSS Mobile-first cho website tiệm nail có giới thiệu, dịch vụ, bảng giá và form đặt lịch. | AI đề xuất cấu trúc `header`, `nav`, `main`, `section`, `article`, `figure`, `table`, `footer` cùng lưới CSS Grid và 2 điểm gãy `@media (min-width: 640px)` và `960px`. | **Giữ** bộ khung HTML5 ngữ nghĩa và 2 mốc breakpoint. **Sửa** nội dung giới thiệu, địa chỉ quán tại Vĩnh Tường – Phú Thọ và bổ sung dải 3 cam kết dịch vụ cho sát thực tế. | Mở bằng Chrome DevTools kiểm tra cây DOM thấy đúng 1 thẻ `<h1>`, các thẻ `<label for="...">` khớp `id` ô nhập liệu, không bị tràn ngang ở `320px`. |
| 22/11/2026 | Yêu cầu điều chỉnh màu sắc sang tone hồng trầm thanh lịch và đổi khung ảnh chủ tiệm thành hình tròn. | AI gợi ý bộ biến màu `--brand-rose: #9d4e66`, `--bg-page: #fdf8f7`, `--ink-main: #2d2327` và quy tắc `border-radius: 50%` cho `.owner-avatar img`. | **Chấp nhận** bảng màu hồng trầm và khung tròn. **Sửa** tăng `padding-block` của `.hero` lên `4rem 4.5rem` trên màn hình lớn để mép trên ảnh tròn không chạm vào thanh header cố định. | Quan sát ở độ rộng `1440px` thấy ảnh chân dung `nhi-xinh.jpg` tròn cân đối, có khoảng cách thoáng với thanh điều hướng phía trên. |
| 22/11/2026 | Kiểm tra lỗi không hiển thị ảnh khi mở trang và chuẩn bị triển khai lên GitHub Pages. | AI chỉ ra nguyên nhân do tên tệp ảnh chưa khớp với đường dẫn trong `src` và nhắc chuẩn hóa tên tệp chữ thường không dấu. | **Chấp nhận** và trực tiếp đổi tên 4 ảnh trong `assets/images/` thành `nhi-xinh.jpg`, `gel.jpg`, `design.jpg`, `spa.jpg`, đồng thời cập nhật lại đường dẫn tương đối trong `index.html`. | Tải lại trang trên trình duyệt và mở tab Network (`F12`), cả 4 tệp ảnh đều trả về mã trạng thái `200 OK`, không còn lỗi `404`. |
| 22/11/2026 | Nhờ hỗ trợ rà soát bố cục bộ tài liệu bàn giao (`README.md`, `CHANGELOG.md`, `evidence-index.md`) theo chuẩn học phần FIT4014. | AI gợi ý khung mục cho 4 tệp tài liệu bàn giao và lưu ý ghi rõ giới hạn form tĩnh chưa có máy chủ lưu dữ liệu. | **Sửa** lại toàn bộ nội dung từ bản nháp để khớp đúng tên repository `yennhi1808/tiem-nail-nhi-xinh`, đường dẫn GitHub Pages và kết quả chạy thử thực tế trên máy. | Đối chiếu toàn bộ liên kết nội bộ trong tài liệu (`docs/evidence-index.md`, `docs/AI_LOG.md`) đều hoạt động chính xác. |

---

## 3. Kết quả kiểm chứng trước – sau

| Hạng mục | Trước khi chỉnh sửa | Sau khi chỉnh sửa & kiểm chứng |
|---|---|---|
| **Khung ảnh chủ tiệm & khoảng cách** | Ảnh dùng khung bo vòm và đỉnh khung chạm sát viền dưới thanh menu trên màn hình rộng. | Chuyển sang khung tròn (`border-radius: 50%`, `aspect-ratio: 1 / 1`), tăng khoảng đệm vùng `.hero`, hiển thị cân đối ở cả `320px` và `1440px`. |
| **Đường dẫn tài nguyên ảnh** | Tên tệp ảnh chưa thống nhất gây lỗi không tải được hình minh họa. | Toàn bộ 4 ảnh đặt trong `assets/images/` với tên chữ thường không dấu (`nhi-xinh.jpg`, `gel.jpg`, `design.jpg`, `spa.jpg`), tải đầy đủ trên GitHub Pages. |
| **Biểu mẫu đặt lịch hẹn** | Mới có giao diện nhập liệu cơ bản. | Bổ sung đầy đủ ràng buộc HTML5 (`required`, `minlength`, `maxlength`, `pattern="[0-9]{10,11}"`), viền báo lỗi `:user-invalid` và trang xác nhận `ket-qua.html`. |

---

## 4. Cam kết trách nhiệm cá nhân

- Tôi xác nhận đã tự đọc hiểu toàn bộ mã nguồn HTML5, CSS3 trong dự án `tiem-nail-nhi-xinh`, trực tiếp chạy kiểm thử giao diện, bàn phím, biểu mẫu và triển khai lên GitHub Pages.
- Mọi hình ảnh, thông tin cá nhân và ảnh chụp minh chứng trong thư mục `docs/evidence/` đều là dữ liệu thật của bài làm, không chứa mật khẩu, token hay thông tin nhạy cảm.