============================================================
  AI PREDICTOR PREMIUM · README
============================================================

1. GIỚI THIỆU
------------------------------------------------------------
Hệ thống dự đoán Tài Xỉu đa nền tảng (Sunwin, Hitclub, B52, MD5).
Gồm 2 file HTML độc lập chạy trực tiếp trên trình duyệt:
  - index.html : Dành cho người dùng (Đăng ký, Đăng nhập, Nạp xu, Dự đoán).
  - admin.html : Dành cho quản trị viên (Duyệt nạp, Quản lý user).

LƯU Ý CỰC QUAN TRỌNG:
  Đây là tool phân tích pattern và quét ảnh (Canvas Pixel) dựa trên 
  dữ liệu mày tự bỏ vào. Nó KHÔNG kết nối tới server nhà cái, KHÔNG 
  có tool nào đoán được xúc xắc thật 100%. Cờ bạc thì nhà cái luôn 
  có lợi thế, chơi vui thôi, đừng all-in.


2. TÍNH NĂNG NỔI BẬT
------------------------------------------------------------
[+] Phân tích cầu: Bắt cầu bệt, cầu 1-1, tính tỉ lệ % Tài/Xỉu.
[+] AI Quét ảnh (5 Xu): Chụp ảnh bàn cầu, thuật toán Canvas API 
    sẽ quét các điểm ảnh Đỏ (Tài) / Xanh (Xỉu) để tự động trích 
    xuất chuỗi kết quả vào lịch sử.
[+] Tính xu: Dùng tool dự đoán tốn 2 xu. Quét ảnh tốn 5 xu.
[+] Nạp tiền: Hỗ trợ nạp thẻ cào (Vina, Viettel, Mobi) và 
    chuyển khoản ngân hàng (LPBank - Ma Van Hung).
[+] Admin: Duyệt nạp tiền, cộng xu tự động cho user, quản lý/xóa user.


3. CÁCH SỬ DỤNG (LOCAL)
------------------------------------------------------------
B1: Tạo 1 thư mục (vd: /predictor).
B2: Bỏ 2 file "index.html" và "admin.html" vào.
B3: Mở "index.html" bằng trình duyệt để đăng ký tài khoản.
B4: Mở "admin.html" bằng trình duyệt, nhập pass: admin123
B5: Nạp tiền ở index -> qua admin duyệt -> quay lại index F5 để có xu.
Lưu ý: Data lưu bằng LocalStorage. Xài chung 1 máy, cùng 1 
trình duyệt mới thấy data của nhau.


4. CÁCH ĐƯA LÊN WEB (GITHUB PAGES)
------------------------------------------------------------
B1: Tạo Repo mới trên GitHub, để chế độ Public.
B2: Upload 2 file index.html và admin.html lên Repo.
B3: Vào Settings -> Pages -> Chọn branch "main" -> Save.
B4: Đợi 1-2 phút, lấy link (vd: ten-mien.github.io/repo).
B5: Link không có đuôi là trang user, thêm /admin.html là trang admin.
*Cảnh báo: LocalStorage lưu trên từng máy. Up lên GitHub thì 
mày đăng ký bên máy mày, thằng khác mở link đéo thấy đâu. 
Muốn share data toàn cầu phải dùng Backend (Node.js).


5. LIÊN HỆ
------------------------------------------------------------
discord server: https://discord.gg/wgy5mpDKJq
made by @odil9 on discord
============================================================
