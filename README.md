# 📚 BỘ TÀI LIỆU ÔN TẬP QUIZLET IOT102 TOÀN DIỆN (350 CÂU HỎI)

Thư mục này chứa đầy đủ toàn bộ ngân hàng câu hỏi môn **IOT102** được trích xuất từ slide thuyết trình, có đối soát đáp án, bổ sung giải thích chuyên sâu và phân loại thành các tệp sẵn sàng để học.

---

## 📂 Danh Sách Các Tệp Trong Thư Mục

1. **`Ung_Dung_On_Tap_Flashcard.html`** ⭐ *(Khuyên dùng)*:
   - Ứng dụng web học tập tương tác trực tiếp cao cấp, **chỉ cần nhấp đúp chuột để mở trên trình duyệt (Chrome, Edge)**.
   - **Chế độ Luyện Thi Trắc Nghiệm Tương Tác (Practice Quiz)**:
     - Cho phép **bấm chọn đáp án A/B/C/D trực tiếp**.
     - Phản hồi đúng/sai tức thì: Đúng chuyển xanh (`✔`), sai chuyển đỏ (`✘`) kèm hiển thị đáp án đúng.
     - Hiệu ứng âm thanh Offline (Web Audio API) sống động.
     - Tự động hiển thị giải thích chi tiết, nguồn slide và cảnh báo nếu có lệch đáp án.
     - Bảng đếm điểm, tỉ lệ chính xác (%), chuỗi trả lời đúng (Streak) và mục "Ôn lại câu làm sai".
   - **5 Phông Nền Động Tuyệt Đẹp (Dynamic Canvas)**:
     - 🌐 *Mạng Lưới Vi Mạch IoT (IoT Cyber Mesh)* tương tác theo chuột.
     - ⚡ *Mưa Ma Trận Cyberpunk (Neon Matrix Rain)*.
     - 🌌 *Cực Quang Vũ Trụ & Sao (Deep Aurora)*.
     - ✨ *Đom Đóm Ánh Sáng (Tech Bokeh)*.
     - ⬛ *Kính Tối Giản (Minimal Dark Glass)*.
   - **Chế độ Flashcard lật thẻ 350 câu** & **Chế độ Danh sách đầy đủ tra cứu nhanh**.
   - Hỗ trợ tách biệt khối mã nguồn Arduino C++ (`<pre><code>`) và khắc phục 100% tình trạng tràn chữ hoặc chèn đáp án dài.
   - Có nút **"Copy Nhanh Quizlet Import"** để sao chép dữ liệu chỉ bằng 1 cú nhấp chuột.

2. **`IoT102_Quizlet_Study_Guide.md`**:
   - Tài liệu học tập toàn diện dạng Markdown.
   - Trình bày toàn bộ 350 câu hỏi, các phương án A/B/C/D, đáp án trong slide ghi chú, đáp án chính xác và lời giải thích chi tiết.
   - Có bảng cảnh báo tổng hợp các câu có đáp án lệch / gây tranh cãi ngay ở đầu trang.

3. **`quizlet_all_350_questions.txt`**:
   - File nạp toàn bộ 350 câu hỏi vào Quizlet (định dạng TSV: Thuật ngữ và Định nghĩa phân cách bằng phím Tab).

4. **Thư mục `quizlet_import_theo_tung_bai/`**:
   - Chia nhỏ thành từng học phần riêng để dễ học trên Quizlet (mỗi học phần từ 15 đến 130 thẻ):
     - `00_Cac_Cau_Co_Dap_An_Lech_Can_Luu_Y_12cau.txt`: 12 câu đặc biệt cần lưu ý/lệch đáp án.
     - `01_Phan_1_Dang_Bai_Tap_74cau.txt`: 74 câu bài tập tính toán mạch điện, ADC, điện áp, PWM, mã màu...
     - `02_Phan_2_Answer_Ngan_133cau.txt`: 133 câu lý thuyết ngắn, linh kiện cảm biến, giao thức.
     - `03_Phan_3_Answer_Dai_92cau.txt`: 92 câu lý thuyết dài, ứng dụng IoT, bảo mật, mạng Mesh.
     - `04_Phan_4_Ly_Thuyet_Bo_Sung_34cau.txt`: 34 câu ôn tập mở rộng, keypad, SoftwareSerial.
     - `05_Phan_5_Cau_Hoi_NOT_15cau.txt`: 15 câu dạng chọn đáp án SAI (NOT).
     - `06_Phan_6_True_False_2cau.txt`: 2 câu dạng Đúng/Sai.

5. **`iot102_complete_dataset.json`**:
   - Dữ liệu dạng JSON chứa toàn bộ 350 câu hỏi chuẩn hóa sạch, có tách trường `code` riêng cho lập trình viên hoặc các công cụ phân tích tự động.

---

## 🚀 Hướng Dẫn Nạp Vào Quizlet Trong 30 Giây

1. Truy cập [Quizlet.com](https://quizlet.com) và đăng nhập.
2. Nhấn nút **Tạo học phần mới (Create set)**.
3. Chọn tính năng **Nhập (Import)** (hoặc biểu tượng tài liệu bên dưới tiêu đề học phần).
4. Mở tệp `.txt` tương ứng (ví dụ `quizlet_all_350_questions.txt` hoặc tệp trong thư mục `quizlet_import_theo_tung_bai/`), chọn tất cả (`Ctrl + A`) và sao chép (`Ctrl + C`).
5. Dán (`Ctrl + V`) vào ô nhập của Quizlet.
   - Đảm bảo thiết lập: Giữa thuật ngữ và định nghĩa là **Tab**, giữa các thẻ là **Dòng mới (Newline)**.
6. Nhấn nút **Nhập (Import)** > Nhấn **Tạo (Create)** để hoàn tất!
