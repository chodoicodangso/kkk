# (Bài Tập Tổng Hợp) Kiến Trúc Hệ Điều Hành & Tư Duy Quản Lý File

## Phần 1 — Kiến trúc Hệ điều hành

1. **Chức năng quản lý tài nguyên và đa nhiệm:**
   - Việc cùng lúc chạy Word, Chrome, VS Code và phần mềm nộp bài thể hiện chức năng **Quản lý tài nguyên phần cứng (Resource Management)** và khả năng **Đa nhiệm (Multitasking)** của hệ điều hành (HDH).
   - Các phần mềm này chạy được cùng lúc mà không bị xung đột (conflict) là nhờ cơ chế **chia sẻ và cấp phát tài nguyên thông minh** của HDH. HDH phân chia thời gian CPU (CPU Scheduling), quản lý không gian bộ nhớ RAM độc lập cho từng tiến trình (Memory Management), và điều phối thiết bị ngoại vi, đảm bảo mỗi ứng dụng hoạt động trong một vùng nhớ riêng biệt, không xâm phạm lẫn nhau.

2. **Vai trò của Shell và Kernel:**
   - Khi double-click vào file báo cáo để mở, hành động đó trước hết được xử lý qua lớp **Shell** (giao diện người dùng / giao diện dòng lệnh hoặc đồ họa). Shell tiếp nhận thao tác click chuột của bạn, dịch nó thành lệnh hệ thống rồi chuyển xuống tầng cốt lõi bên dưới.
   - **Vai trò của Kernel (Nhân hệ điều hành):** Là trung tâm điều khiển tối cao, trực tiếp quản lý phần cứng (CPU, RAM, ổ cứng) và xử lý các yêu cầu cấp thấp từ Shell (như định vị sector trên ổ đĩa, nạp dữ liệu file lên RAM).
   - **Vì sao người dùng thường không tương tác trực tiếp với Kernel:** Vì Kernel hoạt động ở mức phần cứng với mã nguồn và cơ chế vận hành cực kỳ phức tạp, không an toàn và khó sử dụng đối với người dùng phổ thông. Nếu thao tác nhầm trực tiếp vào Kernel, hệ thống có thể bị treo hoặc sập toàn bộ (kernel panic / crash).

---

## Phần 2 — Cây thư mục & Ổ đĩa

1. **Xác định thành phần cây thư mục:**
   - **Root Directory (Thư mục gốc):** `D:\`
   - **Parent Directory (Thư mục cha trực tiếp của file `anh 1.jpg`):** `Hinh anh`
   - **Vai trò của file `anh 1.jpg`:** Là **"lá" (leaf)** trong mô hình cây thư mục vì nó nằm ở tận cùng, không chứa thêm thư mục con nào bên trong nữa.

2. **Nguy cơ khi lưu trữ dự án ở Desktop hoặc Downloads (Ổ C):**
   - **Lý do 1 (Rủi ro mất dữ liệu khi hệ điều hành lỗi):** Ổ `C:\` là nơi chứa hệ điều hành Windows. Khi máy tính gặp sự cố phải cài lại Win hoặc xung đột hệ thống, các thư mục cá nhân như Desktop hay Downloads thường bị xóa trắng hoặc mất dữ liệu.
   - **Lý do 2 (Dễ bị tràn bộ nhớ hệ thống):** Thư mục User Profile trên ổ `C:\` thường bị giới hạn dung lượng hoặc phân bổ không rộng rãi bằng các ổ dữ liệu riêng biệt. Lưu file nặng ở đây làm giảm hiệu năng hệ thống.
   - **Đề xuất nơi lưu đúng:** Lưu toàn bộ thư mục dự án trên ổ đĩa dữ liệu riêng biệt, ví dụ ổ `D:\` theo mô hình các trụ cột rõ ràng.

---

## Phần 3 — Đường dẫn Path

1. **Absolute Path (Đường dẫn tuyệt đối) của file `anh 1.jpg`:**
   ```text
   D:\Nam1\HocKy1\MonHoc\CongNgheThongTin\BaiTapLon\Session02\BaoCaoCuoiKy\Chuong1\Hinh anh\anh 1.jpg