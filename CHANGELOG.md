# Nhật ký thay đổi (CHANGELOG) — Tiệm Nail Nhi Xinh

## v2.0 — 22/11/2026 (Bản bàn giao hoàn chỉnh A3)
**Thay đổi:**
- Tinh chỉnh giao diện sang bảng màu hồng trầm – kem ấm – than tím cùng cặp phông chữ `Mali` và `Quicksand`; chuyển khung ảnh chủ tiệm Nguyễn Yến Nhi sang dạng bo tròn (`border-radius: 50%`) và điều chỉnh khoảng cách thoáng với thanh điều hướng.
- Chuẩn hóa tên 4 tệp ảnh trong `assets/images/` sang chữ thường không dấu (`nhi-xinh.jpg`, `gel.jpg`, `design.jpg`, `spa.jpg`) và đồng bộ đường dẫn tương đối để hiển thị ổn định trên GitHub Pages.
- Cập nhật địa chỉ thực tế của quán tại Thôn Tứ Kì, xã Vĩnh Tường, tỉnh Phú Thọ.
- Hoàn thiện bộ tài liệu bàn giao gồm `README.md`, `CHANGELOG.md`, `docs/AI_LOG.md`, `docs/evidence-index.md` và bổ sung ảnh chụp kiểm thử trong `docs/evidence/`.

**Chưa kiểm tra:**
- Hiển thị trực tiếp trên thiết bị iPhone thật (mới kiểm thử qua chế độ giả lập thiết bị di động trên Chrome DevTools).

---

## v1.0 — 22/11/2026 (Khởi tạo mã nguồn & triển khai GitHub Pages)
**Thay đổi:**
- Dựng cấu trúc website tĩnh HTML5 ngữ nghĩa (`index.html`, `ket-qua.html`) gồm `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<figure>`, `<table>` và `<footer>`.
- Viết bảng định kiểu `css/style.css` theo hướng Mobile-first với Flexbox/Grid, 2 điểm gãy Responsive (`640px`, `960px`) và biểu mẫu đặt lịch có ràng buộc HTML5 (`required`, `minlength`, `maxlength`, `pattern`, `type="email"`).
- Đẩy mã nguồn lần đầu lên repository `yennhi1808/tiem-nail-nhi-xinh` và kích hoạt triển khai qua GitHub Pages tại `https://yennhi1808.github.io/tiem-nail-nhi-xinh/`.

**Chưa kiểm tra:**
- Chưa tối ưu khoảng cách khung ảnh đại diện trên màn hình rộng và chưa hoàn thiện bộ tài liệu bàn giao.