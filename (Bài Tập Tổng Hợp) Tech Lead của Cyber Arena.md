# (Bài Tập Tổng Hợp) Tech Lead của Cyber Arena

## 1. Mục tiêu
Sau bài tổng hợp này, có thể vận dụng và hình dung dễ hiểu hơn về các kiến thức đã học:
- Các lĩnh vực CNTT và vai trò nghề nghiệp
- Mô hình DIKW (Data – Information – Knowledge – Wisdom)
- Đơn vị lưu trữ, phân biệt Mbps và MB/s
- Mô hình IPO (Input – Process – Output) và vai trò CPU / RAM / Storage

## 2. Bối cảnh
Bạn và nhóm bạn mở **Cyber Arena**, một trung tâm Gaming & Esports nhỏ. Trung tâm cho khách thuê máy chơi game, đồng thời là nơi đội tuyển **Liên Minh Huyền Thoại** của trường tập luyện. Bạn là người duy nhất học CNTT nên được giao vai trò **Tech Lead** đầu tiên với 3 nhiệm vụ:
1. **Tuyển người phụ trách kỹ thuật.**
2. **Thiết kế hệ thống quay và xem lại các trận đấu.**
3. **Chọn nâng cấp máy tính.**

## 3. Dữ liệu / Tài nguyên cho sẵn
- Mỗi trận đấu quay video, tạo ra file dung lượng khoảng **500 MB**.
- Đội tuyển thi đấu tổng cộng khoảng **20 trận** trong **1 tháng**.
- Trung tâm dùng mạng cáp quang **100 Mbps** để livestream lên YouTube.
- Máy chơi game hiện có **16 GB RAM** và ổ cứng **SSD 512 GB**.
- Ngân sách chỉ đủ tuyển **1 nhân sự kỹ thuật** và nâng cấp **1 linh kiện**.

## 4. Ràng buộc
- Dùng mô hình **IPO** làm xương sống cho hệ thống ghi hình — xem lại trận đấu.
- 1 Byte = 8 bit
- 1 KB = 1024 Byte; 1 MB = 1024 KB; 1 GB = 1024 MB; 1 TB = 1024 GB
- Mbps = Megabit trên giây; MB/s = Megabyte trên giây
- Công thức: **MB/s = Mbps ÷ 8** ; **Thời gian (s) = Dung lượng (MB) ÷ Tốc độ (MB/s)**

## 5. Yêu cầu

### Phần 1 – Lĩnh vực CNTT và đơn vị lưu trữ
1. Ngân sách chỉ đủ tuyển 1 người. Bạn chọn ứng viên nào? Nêu lựa chọn và giải thích trong 2–3 câu, dựa trên nhu cầu thực tế của **Cyber Arena**.
   - *Ứng viên A:* giỏi lập trình, có thể viết phần mềm đặt lịch thuê máy (lĩnh vực *Kỹ thuật phần mềm*).
   - *Ứng viên B:* giỏi lắp ráp, sửa máy tính và cài đặt mạng (lĩnh vực *Mạng máy tính / Quản trị hệ thống*).
2. Sắp xếp các đơn vị sau theo thứ tự **tăng dần**: **GB**, **Byte**, **TB**, **KB**, **MB**

### Phần 2 – Mô hình IPO và lĩnh vực CNTT
1. **Hệ thống quay lại** và **xem lại trận đấu** hoạt động theo **mô hình IPO**, kèm một nơi lưu trữ. Điền vào bảng, mỗi ô 1 ý ngắn:

| Thành phần | Trong hệ thống quay/xem lại trận đấu |
| :--- | :--- |
| **Input** | ? |
| **Process** | ? |
| **Output** | ? |
| **Storage** | ? |

2. Hoạt động của **Cyber Arena** (livestream, quay video, xem lại phân tích) gắn với lĩnh vực CNTT nào đã được học? (Chọn 1-2 lĩnh vực và mỗi lĩnh vực giải thích 1 câu).

### Phần 3 – Tính toán dung lượng và tốc độ mạng
1. **Tính dung lượng lưu trữ:**
   - 20 trận × 500 MB = bao nhiêu MB?
   - Đổi kết quả sang GB.
   - SSD 512 GB có chứa đủ video của 1 tháng không? Sau 1 tháng đầu tiên vận hành còn trống bao nhiêu GB? (Bỏ qua dung lượng hệ điều hành và game.)
2. **Tính tốc độ mạng:**
   - Mạng 100 Mbps tương đương tối đa bao nhiêu MB/s?
   - Với tốc độ đó, tải lên (upload) 1 đoạn video 200 MB mất tối thiểu bao nhiêu giây?
   - Vì sao thực tế thường lâu hơn con số tính được? Nêu 1 lý do.

### Phần 4 – Phần cứng và mô hình DIKW
1. Máy bị giật khi vừa **chơi game** vừa **quay video livestream**. Bạn sẽ nâng cấp **RAM** hay **CPU** để giải quyết vấn đề này? Chọn 1 và giải thích 2–3 câu dựa trên vai trò của từng thành phần.
2. Áp mô hình **DIKW** vào 1 tình huống: "Huấn luyện viên xem video thấy tuyển thủ hay chết ở phút 15-20, phát hiện do thiếu tầm nhìn bản đồ, nên yêu cầu mua thêm mắt (Ward) cho trận sau." Đâu là Data, Information, Knowledge, Wisdom trong câu trên?

| Nội dung trong tình huống | Vì sao thuộc tầng này? (1 câu) |
| :--- | :--- |
| **Data** | ? |
| **Information** | ? |
| **Knowledge** | ? |
| **Wisdom** | ? |