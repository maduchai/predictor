============================================================
  HAI×BO PREDICTOR · HƯỚNG DẪN SỬ DỤNG (README)
============================================================

1. GIỚI THIỆU
------------------------------------------------------------
Đây là hệ thống dự đoán Tài Xỉu đa nền tảng (Sunwin, Hitclub, B52, MD5).
- Giao diện 7 màu nhấp nháy, có nhạc nền.
- Thuật toán riêng biệt cho từng game.
- Tự động quét ảnh bàn cầu bằng AI (Canvas Pixel).
- Hệ thống nạp thẻ, chuyển khoản, quản lý user qua trang Admin.

Gồm 2 file HTML độc lập chạy trực tiếp trên trình duyệt:
  - index.html : Dành cho User (Đăng ký, Đăng nhập, Dự đoán, Nạp xu).
  - admin.html : Dành cho Admin (Quản lý user, Duyệt nạp, Cộng/Trừ xu).


2. CÁCH SỬ DỤNG CƠ BẢN
------------------------------------------------------------
B1: Tạo 1 thư mục (vd: /haibo-tool).
B2: Bỏ 3 file "index.html", "admin.html", "README.txt" vào.
B3: Mở "index.html" -> Bấm Đăng Ký -> Đăng Nhập để vào Tool.
B4: Mở "admin.html" -> Đăng nhập bằng mật khẩu: admin123
B5: Vào tab "Quản Lý Tài Khoản" ở admin để Cộng (+)/Trừ (-) xu cho user.
    (Nếu user nạp thẻ/chuyển khoản, đơn sẽ hiện ở tab "Duyệt Nạp Tiền").


3. TÍNH NĂNG DỰ ĐOÁN VÀ TỶ LỆ
------------------------------------------------------------
[+] Thuật toán mỗi game một khác:
    - Sunwin: Chuyên bắt cầu bệt & nhịp 1-1.
    - Hitclub: Bám cầu theo xu hướng, cầu dài mới bẻ.
    - B52: Chuyên bẻ cầu liên tục (đánh ngược phiên trước).
    - MD5: Băm thời gian thực (Hash) để random.

[+] Tốn Xu:
    - Phân tích thủ công: 2 Xu / lần.
    - Phân tích bằng Ảnh (AI Scan): 5 Xu / lần.

[+] Tỷ lệ nạp:
    - 10.000 VNĐ  = 20 Xu.
    - 100.000 VNĐ = 220 Xu.
    - 400.000 VNĐ = 1000 Xu.


4. HƯỚNG DẪN NẠP TIỀN
------------------------------------------------------------
* Nạp Thẻ Cào:
  - Chọn nhà mạng (Viettel, Vina, Mobi).
  - Nhập Serial và Mã thẻ (Bắt buộc từ 10 đến 15 số).
  - Bấm Gửi -> Chờ Admin duyệt bên admin.html.

* Nạp Chuyển Khoản:
  - Ngân hàng: LPBank
  - Số TK: 0868866580
  - Chủ TK: MA VAN HUNG
  - Nội dung CK: (Hệ thống tự động tạo mã riêng cho từng user, VD: HAIBO1234).
  - Chuyển khoản đúng nội dung -> Bấm "Tôi Đã Chuyển Khoản" -> Chờ Admin duyệt.


5. LƯU Ý QUAN TRỌNG (ĐỌC KỸ)
------------------------------------------------------------
- Data (User, Đơn nạp) lưu bằng LocalStorage của trình duyệt.
- Xài chung 1 máy, cùng 1 trình duyệt mới thấy data của nhau.
- Xóa cache/lịch sử trình duyệt => MẤT HẾT USER VÀ ĐƠN NẠP.
- Nếu đưa link web lên GitHub Pages cho bạn bè, nó mở bằng máy nó
  sẽ đéo thấy data bên máy mày đâu. Muốn dùng chung toàn cầu phải
  làm Backend (Node.js / Python / Firebase).


6. LIÊN HỆ
------------------------------------------------------------
discord server: https://discord.gg/wgy5mpDKJq
made by @odil9 on discord
============================================================
