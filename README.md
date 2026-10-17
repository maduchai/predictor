============================================================
  LARP TÀI XỈU TOOL · README
============================================================

1. GIỚI THIỆU
------------------------------------------------------------
Tool gồm 2 phần chính chạy trên trình duyệt (HTML/JS):
  - GATE         : Màn hình chặn, phải nhập key mới vào được.
  - PREDICTOR    : Dự đoán Tài/Xỉu dựa trên lịch sử tự nhập.
  - ADMIN        : Tạo key theo giờ / ngày / tháng / năm.

LƯU Ý CỰC QUAN TRỌNG:
  Đây là tool phân tích PATTERN dựa trên data mày tự bỏ vào.
  Nó KHÔNG kết nối tới server Sunwin / Hitclub / B52 hay bất kỳ
  nhà cái nào. Đéo có tool nào đoán được xúc xắc thật 100%.
  Cờ bạc thì nhà cái luôn có lợi thế, chơi vui thôi, đừng all-in.


2. CÁCH DÙNG FILE ALL-IN-ONE (KHUYÊN DÙNG)
------------------------------------------------------------
Mở file: "larp-all-in-one.html" (cái file tao gửi gần nhất).
  1. Nhập key -> bấm Mở Khóa.
  2. Vào trang Dự Đoán -> nhập tổng 3 xúc xắc -> bấm Dự Đoán.
  3. Muốn tạo key thì bấm nút "Admin tạo key" ngay màn hình gate.
  4. Trong app có tab Admin để quản lý key (copy, thu hồi, xóa).


3. CÁCH TẠO KEY ADMIN
------------------------------------------------------------
B1: Vào màn Admin.
B2: Chọn đơn vị thời gian (Giờ / Ngày / Tháng / Năm).
B3: Nhập số lượng thời gian (vd: 1 ngày, 3 tháng).
B4: Nhập số key muốn tạo.
B5: Bấm "Tạo Key".
B6: Copy key đưa cho user. Key có dạng:
    LARP-YYYYMMDDHHMM-XXXX-XXXXXXXX


4. CẢNH BÁO ĐỎ (ĐỌC KỸ)
------------------------------------------------------------
- Key và lịch sử lưu ở localStorage của TRÌNH DUYỆT.
- Xóa cache / dữ liệu trình duyệt => MẤT HẾT KEY + LỊCH SỬ.
- Muốn dùng nhiều máy: key phải được tạo trên máy đó, hoặc phải
  đồng bộ localStorage (phức tạp). Bản này để xài 1 máy cho gọn.
- MASTER_SECRET trong code phải GIỐNG NHAU giữa file tạo key và
  file kiểm tra key. Mặc định tao để chung 1 cái, đừng sửa lẻ.
- Build thật (bán/dùng chung nhiều người) thì phải đẩy MASTER_SECRET
  lên server. Để trong client là bị dịch ngược lấy sạch key.


5. FILE ĐI KÈM
------------------------------------------------------------
- larp-all-in-one.html : Bản gộp Gate + Predictor + Admin.
- larp-predictor.html  : Bản chỉ dự đoán (không có gate).
- larp-admin.html      : Bản chỉ tạo key.
- README.txt           : File này.


6. LIÊN HỆ
------------------------------------------------------------
discord server: https://discord.gg/wgy5mpDKJq
made by @odil9 on discord

============================================================
