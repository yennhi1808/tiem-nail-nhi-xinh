# Tiệm Nail Nhi Xinh — Website Giới Thiệu & Đặt Lịch Dịch Vụ

## Sản phẩm này là gì?
Website tĩnh giới thiệu không gian, bảng giá, các gói chăm sóc móng – hand spa và hỗ trợ khách hàng gửi yêu cầu đặt lịch hẹn cho **Tiệm Nail Nhi Xinh** (địa chỉ: Thôn Tứ Kì, xã Vĩnh Tường, tỉnh Phú Thọ), thực hiện bởi sinh viên **Nguyễn Yến Nhi (MSSV: 2071020148)** cho học phần FIT4014[cite: 16].

## Demo
- **URL GitHub Pages:** https://yennhi1808.github.io/tiem-nail-nhi-xinh/
- **Repository GitHub:** https://github.com/yennhi1808/tiem-nail-nhi-xinh[cite: 16]

## Tính năng
- Bấm **Giới thiệu** trên thanh điều hướng để xem thông tin về chủ tiệm Nguyễn Yến Nhi và 3 cam kết dịch vụ của quán (sơn gel chính hãng, tiệt trùng riêng biệt, bảo hành 7 ngày).
- Bấm **Dịch vụ** để xem 3 thẻ gói làm móng nổi bật (*Sơn Gel Thạch & Trơn Bóng*, *Thiết Kế Nail Art & Mắt Mèo*, *Chà Gót & Spa Dưỡng Tay*) kèm thời lượng và mức giá tham khảo.
- Bấm **Bảng giá** để tra cứu chi phí niêm yết chi tiết của 5 gói dịch vụ tại quán[cite: 11, 16].
- Bấm **Đặt lịch ngay** để xem địa chỉ quán, giờ mở cửa (09:00 – 21:00) và điền biểu mẫu đặt lịch hẹn có kiểm tra ràng buộc HTML5 (họ tên, số điện thoại 10–11 số, email, dịch vụ, ghi chú) rồi chuyển sang trang xác nhận `ket-qua.html`[cite: 11, 16].

## Cách mở
1. Mở đường dẫn ở mục **Demo** (`https://yennhi1808.github.io/tiem-nail-nhi-xinh/`) bằng trình duyệt web[cite: 11, 16].
2. Bấm lần lượt các mục **Giới thiệu**, **Dịch vụ**, **Bảng giá** trên thanh menu để cuộn tới từng phần nội dung[cite: 11, 16].
3. Bấm nút **Đặt lịch ngay** trên menu (hoặc nút **Đặt lịch làm móng** ở đầu trang), điền thông tin thử nghiệm và bấm **Gửi thông tin đặt lịch** để kiểm tra chuyển trang sang `ket-qua.html`[cite: 11, 16].
4. Nếu chạy trên máy cá nhân: tải mã nguồn về máy, giải nén và mở trực tiếp tệp `index.html` bằng trình duyệt (hoặc chạy qua Live Server trong VS Code)[cite: 11].

## Cấu trúc thư mục
```text
tiem-nail-nhi-xinh/
├── index.html              # Trang chủ giới thiệu, dịch vụ, bảng giá và biểu mẫu đặt lịch
├── ket-qua.html            # Trang xác nhận sau khi gửi biểu mẫu hợp lệ
├── README.md               # Tài liệu giới thiệu và hướng dẫn mở sản phẩm
├── CHANGELOG.md            # Nhật ký thay đổi qua các phiên bản (V7, V8)
├── css/
│   └── style.css           # Định dạng giao diện, bố cục Flexbox/Grid và Responsive
├── assets/
│   └── images/
│       ├── nhi-xinh.jpg    # Ảnh chân dung chủ tiệm Nguyễn Yến Nhi
│       ├── gel.jpg         # Ảnh minh họa dịch vụ sơn gel
│       ├── design.jpg      # Ảnh minh họa dịch vụ thiết kế nail art
│       └── spa.jpg         # Ảnh minh họa dịch vụ spa tay chân
└── docs/
    ├── AI_LOG.md           # Nhật ký khai báo sử dụng AI
    ├── evidence-index.md   # Bảng đối chiếu tiêu chí và minh chứng kiểm thử
    └── evidence/           # Thư mục lưu ảnh chụp minh chứng kiểm tra