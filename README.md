# main_testops
Kho 1: Thu thập ý tưởng, yêu cầu cho yc chung của dự án
# 📌 DISCUSSION: Phân tích & Thu thập yêu cầu  
## Dự án: Hệ thống Thư viện Điện tử HNUE

---

## 1. Thông tin chung dự án

**Tên dự án:**  
Phân tích và quản lý yêu cầu cho dự án phát triển hệ thống Thư viện điện tử  
Trường Đại học Sư phạm Hà Nội (HNUE)

**Mục tiêu chính:**  
Xây dựng hệ thống thư viện điện tử tích hợp AI nhằm:
- Giảm tải cho thủ thư
- Nâng cao hiệu quả quản lý tài nguyên
- Tăng khả năng tiếp cận học liệu cho sinh viên & giảng viên
- Đẩy mạnh chuyển đổi số trong giáo dục

---

## 2. Mô tả bài toán (Problem Statement)

Hiện tại, thư viện HNUE:
- Quản lý mượn – trả sách chủ yếu thủ công
- Quá tải vào giờ cao điểm
- Khó thống kê, báo cáo và mở rộng thư viện số
- Chưa hỗ trợ truy cập học liệu mọi lúc, mọi nơi

➡️ **Vấn đề cốt lõi:**  
Hệ thống hiện tại **thiếu tự động hóa, thiếu minh bạch và khó mở rộng quy mô**.

---

## 3. Stakeholders (Các bên liên quan)

| Nhóm | Vai trò | Nhu cầu chính |
|----|--------|--------------|
| Sinh viên | Người sử dụng chính | Mượn sách nhanh, tra cứu dễ, truy cập online |
| Giảng viên | Người dùng học thuật | Tài liệu chuyên ngành, thống kê học liệu |
| Thủ thư | Quản lý hệ thống | Giảm thao tác thủ công, quản lý hiệu quả |
| Ban quản lý | Ra quyết định | Báo cáo, thống kê, đánh giá nhu cầu |
| Nhóm IT | Phát triển & bảo trì | Yêu cầu rõ ràng, khả thi, dễ mở rộng |

---

## 4. Discussion: Thu thập yêu cầu chức năng (Functional Requirements)

### 4.1 Quản lý mượn – trả sách
- Hệ thống cho phép mượn – trả sách **tự động**
- Đồng bộ dữ liệu **theo thời gian thực**
- Theo dõi trạng thái sách: còn / đang mượn / quá hạn

👉 **Câu hỏi thảo luận:**
- Có cần giới hạn số sách mượn tối đa/sinh viên không?
- Quy trình mượn có cần xác thực bằng thẻ sinh viên không?

---

### 4.2 Thư viện số (Digital Library)
- Hỗ trợ ebook, PDF, luận văn, học liệu số
- Truy cập mọi lúc, mọi nơi
- Phân quyền truy cập theo đối tượng (SV / GV)

👉 **Câu hỏi thảo luận:**
- Tài liệu số có cho phép tải về hay chỉ đọc online?
- Có giới hạn số lượt truy cập đồng thời không?

---

### 4.3 Tra cứu & tìm kiếm tài liệu
- Tìm kiếm theo:
  - Tên sách
  - Tác giả
  - Bộ môn
  - Từ khóa
- Kết quả trả về nhanh, chính xác

👉 **Câu hỏi thảo luận:**
- Có cần tìm kiếm nâng cao (lọc theo năm, loại tài liệu)?
- Có hỗ trợ gợi ý từ khóa không?

---

### 4.4 Mượn sách bằng QR / Barcode
- Sinh viên quét mã QR hoặc barcode bằng điện thoại
- Tích hợp với hệ thống mượn – trả

👉 **Câu hỏi thảo luận:**
- Có cần kiosk tự phục vụ trong thư viện không?
- Có yêu cầu xác nhận thủ thư trong một số trường hợp đặc biệt?

---

### 4.5 Quản lý trễ hạn & vi phạm
- Tự động tính phí trễ hạn
- Gửi thông báo nhắc hạn qua:
  - Email
  - Hệ thống nội bộ
- Lưu lịch sử vi phạm người dùng

👉 **Câu hỏi thảo luận:**
- Mức phạt được cấu hình linh hoạt hay cố định?
- Có khóa quyền mượn khi vi phạm nhiều lần không?

---

### 4.6 Thống kê & báo cáo
- Thống kê:
  - Lượt mượn theo thời gian
  - Sách được mượn nhiều nhất
  - Nhu cầu học liệu theo ngành
- Xuất báo cáo phục vụ quản lý

👉 **Câu hỏi thảo luận:**
- Báo cáo cần xuất ra định dạng gì (PDF, Excel)?
- Chu kỳ báo cáo: ngày / tháng / học kỳ?

---

### 4.7 AI hỗ trợ quản lý
- Gợi ý sách theo chuyên ngành
- Phân tích nhu cầu mượn
- Dự báo số lượng sách cần bổ sung

👉 **Câu hỏi thảo luận:**
- AI dựa trên lịch sử mượn hay hồ sơ học tập?
- Có cần dashboard riêng cho AI insights không?

---

## 5. Yêu cầu phi chức năng (Non-functional Requirements)

- Hiệu năng: hệ thống phản hồi nhanh (< 3s)
- Bảo mật: phân quyền, bảo vệ dữ liệu người dùng
- Khả năng mở rộng: hỗ trợ số lượng lớn người dùng
- Khả dụng: hoạt động ổn định 24/7
- Giao diện: dễ dùng cho sinh viên & thủ thư

---

## 6. Kết luận & bước tiếp theo

- Tổng hợp yêu cầu từ các bên liên quan
- Xác định **requirement ưu tiên (High / Medium / Low)**
- Chuyển sang giai đoạn:
  - Đặc tả yêu cầu (SRS)
  - Thiết kế hệ thống

📌 **Mọi ý kiến đóng góp xin comment trong Discussion để nhóm tổng hợp.**
