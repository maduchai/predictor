============================================================
  HAI×BO PREDICTOR · README (HƯỚNG DẪN SỬ DỤNG)
============================================================

1. GIỚI THIỆU
------------------------------------------------------------
Đây là hệ thống Tool dự đoán Tài Xỉu đa nền tảng (Sunwin, Hitclub, B52, MD5).
Giao diện 7 màu nhấp nháy, có nhạc nền (bật/tắt bằng nút góc trên phải), 
tích hợp thuật toán AI quét ảnh bàn cầu siêu tốc.
Bộ tool gồm 2 file HTML độc lập chạy trực tiếp trên mọi trình duyệt:
  - index.html : Dành cho người dùng (Đăng ký, Đăng nhập, Nạp xu, Dự đoán).
  - admin.html : Dành cho quản trị viên (Quản lý User, Duyệt nạp, Đổi pass).


2. CÁCH SỬ DỤNG (CHẠY LOCAL)
------------------------------------------------------------
B1: Tạo 1 thư mục trên máy tính (vd: /haibo-tool).
B2: Lưu cả 2 file "index.html" và "admin.html" vào thư mục đó.
B3: Mở file "index.html" bằng trình duyệt (Chrome/Cốc Cốc/Edge).
    -> Bấm "Đăng Ký" để tạo tài khoản -> Đăng nhập để vào Tool.
B4: Mở file "admin.html" bằng trình duyệt để vào trang quản trị.
    -> Mật khẩu mặc định: admin123 (Có thể đổi bằng nút "Đổi Pass").
B5: Nạp tiền ở bên "index.html" -> Qua "admin.html" bấm Duyệt 
    -> Quay lại index F5 để nhận Xu.

*LƯU Ý QUAN TRỌNG: Data (User, Nạp tiền) được lưu bằng LocalStorage. 
Nghĩa là mày mở 2 file này trên CÙNG 1 MÁY, CÙNG 1 TRÌNH DUYỆT 
thì mới thấy dữ liệu của nhau.


3. TÍNH NĂNG NỔI BẬT
------------------------------------------------------------
[+] AI Quét Ảnh (5 Xu): Chụp ảnh bàn cầu, up lên tool. Thuật toán 
    Canvas API sẽ đọc các điểm ảnh Đỏ (Tài) / Xanh (Xỉu), trả thẳng 
    ra kết quả dự đoán kèm độ tự tin.
[+] Tính Xu: Phân tích cầu tốn 2 Xu. Quét ảnh tốn 5 Xu.
[+] Thuật toán riêng biệt:
    - Sunwin: Bắt cầu bệt & nhịp 1-1.
    - Hitclub: Bám cầu (đứt thì nghỉ).
    - B52: Bẻ cầu liên tục.
    - MD5: Băm thời gian thực (Hash).
[+] Nạp tiền: Nạp thẻ cào (Viettel, Vina, Mobi) bắt buộc nhập 
    Serial/PIN dài từ 10 - 15 số. Nạp chuyển khoản qua LPBank.
[+] Admin: Duyệt nạp cộng xu, xem địa chỉ IP của user, đổi pass.


4. CÁCH ĐƯA LÊN WEB (GITHUB PAGES)
------------------------------------------------------------
B1: Tạo Repo mới trên GitHub, để chế độ Public.
B2: Upload 2 file index.html và admin.html lên Repo.
B3: Vào Settings -> Pages -> Chọn branch "main" -> Save.
B4: Đợi 1-2 phút, lấy link dạng: ten-mien.github.io/repo/
B5: Link không đuôi là trang user. Thêm /admin.html là trang admin.
*Cảnh báo: Vì là web tĩnh (LocalStorage), nếu mày đưa link cho 
thằng khác, nó mở bằng máy nó sẽ đéo thấy data bên mày đâu. 
Muốn share data toàn cầu phải dùng Backend (Node.js/Python).


5. LIÊN HỆ
------------------------------------------------------------
discord server: https://discord.gg/wgy5mpDKJq
made by @odil9 on discord
============================================================
