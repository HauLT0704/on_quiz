# BỘ ÔN TẬP QUIZLET & NGÂN HÀNG CÂU HỎI IOT102 ĐẦY ĐỦ NHẤT (350 CÂU)

> **Tài liệu trích xuất từ file:** `D:\Downloads\GoogleSlides_Export_2026-10-04.pptx` (364 slides)
> **Tổng số câu hỏi trắc nghiệm:** 350 câu (chia làm 6 phần)
> **Bao gồm:** Đầy đủ câu hỏi, lựa chọn A/B/C/D, đáp án trong slide ghi chú, đáp án chuẩn xác minh, giải thích chi tiết tại sao chọn, và bảng cảnh báo các câu có đáp án lệch/tranh cãi.

## 1. Cấu Trúc Các Phần (Bài Học)

| Phần | Tên Bài / Nhóm Nội Dung | Số Lượng Câu | Phạm Vi Slide |
| :--- | :--- | :--- | :--- |
| **Phần 1** | Dạng Bài Tập (Calculation & Circuit Problems) | 74 câu | Slide 10 - 83 |
| **Phần 2** | Answer Ngắn (Short Concept Questions) | 133 câu | Slide 85 - 217 |
| **Phần 3** | Answer Dài (Long Concept & Application Questions) | 92 câu | Slide 219 - 310 |
| **Phần 4** | Lý Thuyết & Ứng Dụng Bổ Sung | 34 câu | Slide 312 - 345 |
| **Phần 5** | Dạng Câu Hỏi NOT (Chọn đáp án SAI) | 15 câu | Slide 347 - 361 |
| **Phần 6** | Dạng Đúng / Sai (True / False) | 2 câu | Slide 363 - 364 |
| **Tổng cộng** | **Tất cả các bài** | **350 câu** | **Slide 10 - 364** |

## 2. BẢNG TỔNG HỢP CÁC CÂU CÓ ĐÁP ÁN LỆCH / TRANH CÃI / THIẾU NOTE

| Slide | Câu hỏi tóm tắt | Note gốc | Đáp án chuẩn | Phân tích chi tiết & Cảnh báo |
| :--- | :--- | :---: | :---: | :--- |
| **Slide 30** | What is the resolution of analog readings on the A... | `C Arduino chuyển đổi tất cả các điện áp tương tự (0V đến 5V hoặc 3.3V) được nhận làm đầu vào thành một dải điện áp từ 0 đến 1023. Điều này được thực hiện bằng cách ánh xạ các mức điện áp. Trên Arduino Uno, mức điện áp tối đa là 5V và bộ chuyển đổi ADC tích hợp có độ phân giải 10 bit, có nghĩa là nó có thể chia tín hiệu tương tự nhận được thành 2¹⁰ mức.` | **C** | ⚠️ LƯU Ý ĐÁP ÁN: File gốc chọn C (5V/1024) dựa trên 2^10 = 1024 mức rời rạc (bước lượng tử q = Vref/2^n). Tuy nhiên, trên slide có in kèm công thức Resolution = Vref/(2^n - 1) = 5V/1023 (Đáp án A). Trong đề thi nếu hỏi theo công thức trên slide là A, nếu hỏi theo số mức lượng tử lý thuyết ADC là C. |
| **Slide 52** | Which function to retrieve text sent from the comp... | `AA` | **A** | ⚠️ LƯU Ý: Ghi chú trong file gốc ghi nhầm "AA" (lặp chữ). Đáp án chuẩn là A: Serial.readStringUntil('\n'). |
| **Slide 56** | How many errors are present in the code given belo... | `C chỗ này có 2 lỗi lớn nếu tính theo dòng là cái dòng int pin1=12 nó là chân digital , nhưng ở dưới lại viết là analogRead tức là đọc tín hiệu analog từ chân digital nên nó sẽ sai , với cái cái dòng vàng cái chỗ pinmode phải sửa thành pinMode là 1 lỗi nữa , ngoài ra đoạn sau nó quy định chân pin1 là input nma để mỗi là IN nên n sai phải là INPUT , tuy nhiên cái lỗi pin1=12 nó gây tranh cãi vì bản thân nó không phải là lỗi compile nó là lỗi logic . nếu tính khắt khe thì là 3 lỗi còn nếu chỉ quy ước code chạy đúng thì nó chỉ có 2 lỗi thôi nhưng thường thì với môn này ngta hay tính 3 lỗi còn nếu chỉ quy ước code chạy đúng thì nó chỉ có 2 lỗi thôi nhưng thường thì với môn này ngta hay tính 3 lỗi vì nếu n đọc giá trị liên tục mà nó auto là 1 giá trị rời rạc thì n sai về mặt logic` | **C** | ⚠️ LƯU Ý ĐÁP ÁN TRANH CÃI: Note chọn C (3 lỗi). Nếu tính lỗi biên dịch (compile error) thì chỉ có 2 lỗi: "pinmode" (phải viết hoa M -> pinMode) và "IN" (phải là INPUT). Lỗi thứ 3 là lỗi logic: "analogRead(pin1)" đọc analog trên chân digital 12 (chân 12 không có bộ ADC, chỉ chân A0-A5 mới đọc được analogRead). Môn IOT102 thường tính 3 lỗi. |
| **Slide 114** | What happens if pinMode is not set for a pin befor... | `*(Trống)*` | **B** | ⚠️ CÂU THIẾU ĐÁP ÁN TRONG FILE GỐC: Slide 114 không có ghi chú trong file PPTX. Đáp án chuẩn xác là B: The pin stays in input mode. |
| **Slide 137** | Which communication protocol does the MAX30102 use... | `*(Trống)*` | **B** | ⚠️ CÂU THIẾU ĐÁP ÁN TRONG FILE GỐC: Slide 137 không có ghi chú trong file PPTX. Đáp án chuẩn xác là B: Inter-Integrated Circuit (I2C). |
| **Slide 145** | Which factors must be considered when aligning mul... | `ABC` | **A, B, C** | ⚠️ CÂU HỎI CHỌN NHIỀU ĐÁP ÁN (Select all that apply): Slide ghi chú chọn ABC. Cần chọn cả 3 phương án A, B và C. |
| **Slide 149** | Which actuator types operate using pressurized flu... | `AB` | **A, B** | ⚠️ CÂU HỎI CHỌN NHIỀU ĐÁP ÁN (Select all that apply): Slide ghi chú chọn AB. Cần chọn cả 2 phương án A và B. |
| **Slide 155** | Which of the following is used for comments in Ard... | `D D phải là both // comment and /* comment */ mới đúng` | **D** | ⚠️ LƯU Ý LỖI IN TRÊN SLIDE: Slide in nhầm phương án D thành "both // comment and/comment*/" (thiếu dấu sao). Note giải thích chuẩn: Phải là cả hai cú pháp // và /* comment */. |
| **Slide 159** | Which of the following is not an example of an ope... | `D. not examlple -> Automatic eletric iron` | **D** | ⚠️ CÂU HỎI PHỦ ĐỊNH (NOT open-loop): Note giải thích đáp án là D (Automatic electric iron). |
| **Slide 166** | Which button in the ESP8266 is used to load the co... | `A` | **A** | ⚠️ LƯU Ý THUẬT NGỮ: Câu hỏi ghi "Which button..." nhưng các đáp án lại là tên chân (GND, TX, A1, A0). Note chọn A (GND). |
| **Slide 203** | To send sensor data to the Serial Monitor, you use... | `AB` | **A, B (hoặc B)** | ⚠️ LƯU Ý: Note trong slide ghi nhận cả "AB". Thông thường để đọc được dữ liệu dạng text trên màn hình Serial Monitor người ta dùng B (Serial.print/println), còn Serial.write gửi dữ liệu byte thô. |
| **Slide 349** | Which Arduino UNO pin is NOT typically used for ex... | `C` | **C** | ⚠️ LƯU Ý LỖI IN: Slide gốc in thiếu phương án D thành ký tự "e.". Đáp án đúng là C: Pin 5 không phải chân ngắt ngoài. |

---

## Phần 1: Dạng Bài Tập (Calculation & Circuit Problems)

### Câu 10 (Slide 10)

**Câu hỏi:** What is the default baud rate for communication in the HC-05 Bluetooth module?

**Các lựa chọn:**
- **A.** 9600
- **B.** 115200
- **C.** 38400
- **D.** 19200

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (9600)

**💡 Giải thích chi tiết:** Module Bluetooth HC-05 có tốc độ truyền nhận dữ liệu (baud rate) mặc định ở chế độ truyền thông thông thường (Data Mode) là 9600 bps. (Lưu ý: ở chế độ cấu hình lệnh AT, baud rate mặc định là 38400 bps).

---

### Câu 11 (Slide 11)

**Câu hỏi:** What is the maximum DC current per 1/0 pin on the Arduino Uno? A 20 mA

**Các lựa chọn:**
- **A.** 20 mA
- **B.** 40 mA
- **C.** 50 mA
- **D.** 100 mA

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (40 mA)

**💡 Giải thích chi tiết:** Theo datasheet vi điều khiển ATmega328P trên Arduino Uno, dòng điện một chiều tối đa tuyệt đối (Absolute Maximum DC Current) cho mỗi chân I/O là 40 mA. Dòng điện khuyến nghị làm việc liên tục an toàn là 20 mA.

---

### Câu 12 (Slide 12)

**Câu hỏi:** What is the maximum value a single number can have in an IPv4 address? A 255

**Các lựa chọn:**
- **A.** 255
- **B.** 128
- **C.** 1024
- **D.** 512

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (255)

**💡 Giải thích chi tiết:** Địa chỉ IPv4 gồm 4 octet (mỗi octet 8 bit). Giá trị lớn nhất của 8 bit nhị phân (11111111_2) tương ứng với số thập phân là 2^8 - 1 = 255. Do đó mỗi số trong địa chỉ IPv4 không thể vượt quá 255.

---

### Câu 13 (Slide 13)

**Câu hỏi:** What is the maximum input voltage limit for an Arduino Uno?

**Các lựa chọn:**
- **A.** 6-20 V
- **B.** 5-15 V
- **C.** 7-17 v
- **D.** 10-20 V

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (6-20 V)

**💡 Giải thích chi tiết:** Bo mạch Arduino Uno Rev3 có giới hạn điện áp đầu vào tuyệt đối (Input Voltage Limit) cấp qua chân Vin hoặc cổng nguồn DC là 6V đến 20V. Dưới 6V nguồn 5V không ổn định; trên 20V IC ổn áp có nguy cơ bị cháy do quá nhiệt.

---

### Câu 14 (Slide 14)

**Câu hỏi:** What is the output of 'pin1' if 'pin2' is sent '1011' where 1 is 5V and 0 is 0V?

**Các lựa chọn:**
- **A.** 1110
- **B.** 0100
- **C.** 0001
- **D.** 1011

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (0100)

**💡 Giải thích chi tiết:** Theo code: nếu digitalRead(pin2) == 1 (HIGH) thì digitalWrite(pin1, LOW - 0); nếu digitalRead(pin2) == 0 (LOW) thì digitalWrite(pin1, HIGH - 1). Đầu vào '1011' sẽ đảo ngược thành '0100' (Bit 1->0, Bit 2->1, Bit 3->0, Bit 4->0).

---

### Câu 15 (Slide 15)

**Câu hỏi:** What is the objective of the code given below if it is executed on the Arduino Uno?

**Các lựa chọn:**
- **A.** Clear EEPROM
- **B.** Fill EEPROM with 1's
- **C.** Export EEPROM data
- **D.** Fill EEPROM with 0's

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (Fill EEPROM with 1's)

**💡 Giải thích chi tiết:** Vòng lặp for chạy từ 0 đến EEPROM.length() và thực hiện lệnh EEPROM.write(i, 1). Lệnh này ghi giá trị byte 1 vào từng ô nhớ của bộ nhớ EEPROM, do đó mục tiêu là ghi số 1 vào toàn bộ EEPROM (Fill EEPROM with 1's).

---

### Câu 16 (Slide 16)

**Câu hỏi:** What is the time period of the output signal of the program given below?

**Các lựa chọn:**
- **A.** 20 Microseconds
- **B.** 100 Milliseconds
- **C.** 10 Milliseconds
- **D.** 20 Milliseconds

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (20 Milliseconds)

**💡 Giải thích chi tiết:** Chương trình bật HIGH trong delay(10) (10ms) và tắt LOW trong delay(10) (10ms). Chu kỳ (Time period) T = Thigh + Tlow = 10ms + 10ms = 20 Milliseconds.

---

### Câu 17 (Slide 17)

**Câu hỏi:** What is the purpose of the following Arduino code?

**Các lựa chọn:**
- **A.** Send a signal to pin 40 on the Arduino board
- **B.** Send an octal number of 40 through the Serial pins
- **C.** Send a byte with value 40 through the Serial pins
- **D.** Send a hexadecimal number of 40 through the Serial pins

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Send a byte with value 40 through the Serial pins)

**💡 Giải thích chi tiết:** Hàm Serial.write(val) gửi trực tiếp một byte nhị phân thô (binary byte) có giá trị 40 (mã ASCII của ký tự '(') qua chân Serial TX tới máy tính/thiết bị nhận.

---

### Câu 18 (Slide 18)

**Câu hỏi:** What is the output of the program given below if a voltage of 5V is supplied to the pin corresponding to the A0 pin on an Arduino UNO?

**Các lựa chọn:**
- **A.** 0
- **B.** 5
- **C.** 1023
- **D.** 512

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (5)

**💡 Giải thích chi tiết:** Bộ chuyển đổi ADC 10-bit của Arduino Uno chuyển đổi dải điện áp 0V - 5V thành giá trị số nguyên từ 0 đến 1023. Khi cấp điện áp cực đại 5V vào chân analog A0, analogRead(A0) sẽ đọc và trả về giá trị số cực đại là 1023.

---

### Câu 19 (Slide 19)

**Câu hỏi:** What is the operating voltage of the Arduino Uno/ATmega328Q

**Các lựa chọn:**
- **A.** 3.3V
- **B.** 6-20 V
- **C.** 5V
- **D.** 7-12 V

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (5V)

**💡 Giải thích chi tiết:** Vi điều khiển ATmega328P trên bo mạch Arduino Uno hoạt động ở điện áp chuẩn là 5V (cung cấp qua cổng USB hoặc qua IC ổn áp 5V tích hợp).

---

### Câu 20 (Slide 20)

**Câu hỏi:** What is the input voltage limit of Arduino Uno Rev3?

**Các lựa chọn:**
- **A.** 7-12 v
- **B.** 3.3~5V
- **C.** 6-20 v
- **D.** 1.5~9 V

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (6-20 v)

**💡 Giải thích chi tiết:** Giới hạn điện áp đầu vào (Input Voltage Limit) cấp qua jack cắm nguồn DC hoặc chân Vin của Arduino Uno Rev3 là 6V - 20V.

---

### Câu 21 (Slide 21)

**Câu hỏi:** What is the voltage at which the ESP8266 chip works?

**Các lựa chọn:**
- **A.** 3.3V
- **B.** 05V
- **C.** 12V
- **D.** 24V

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (3.3V)

**💡 Giải thích chi tiết:** Chip Wi-Fi SoC ESP8266 hoạt động ở mức điện áp danh định là 3.3V. Cấp nguồn 5V trực tiếp có thể gây hỏng chip.

---

### Câu 22 (Slide 22)

**Câu hỏi:** What is the operating voltage of Atmega328?

**Các lựa chọn:**
- **A.** 1.9V to 5V
- **B.** 1.8V to 5.5V
- **C.** 1.1V to5V
- **D.** 1.2V to 9V

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (1.8V to 5.5V)

**💡 Giải thích chi tiết:** Theo thông số kỹ thuật của nhà sản xuất Atmel/Microchip, vi điều khiển ATmega328P có dải điện áp làm việc rộng từ 1.8V đến 5.5V.

---

### Câu 23 (Slide 23)

**Câu hỏi:** What is the clock speed of the ATmega328 microcontroller used in the Arduino Uno?

**Các lựa chọn:**
- **A.** 12 MHz.
- **B.** 8 MHz.
- **C.** 24 MHz.
- **D.** 16 MHz.

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (16 MHz.)

**💡 Giải thích chi tiết:** Tần số xung nhịp dao động (Clock speed) của vi điều khiển ATmega328P trên bo mạch Arduino Uno là 16 MHz (sử dụng thạch anh 16 MHz gắn sẵn).

---

### Câu 24 (Slide 24)

**Câu hỏi:** What is the operating voltage of the Arduino Uno/ATmega328?

**Các lựa chọn:**
- **A.** 3.3V
- **B.** 6-20 V
- **C.** 5V
- **D.** 7-12V

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (5V)

**💡 Giải thích chi tiết:** Điện áp hoạt động chuẩn (Operating Voltage) của bo mạch Arduino Uno và chip ATmega328P là 5V.

---

### Câu 25 (Slide 25)

**Câu hỏi:** What is the recommended input voltage for an Arduino Uno?

**Các lựa chọn:**
- **A.** 5-10 V
- **B.** 7-12 V
- **C.** 9-15 v
- **D.** 11-16 V

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (7-12 V)

**💡 Giải thích chi tiết:** Dải điện áp đầu vào khuyến nghị (Recommended Input Voltage) cho Arduino Uno là 7V đến 12V để IC ổn áp tuyến tính hoạt động mát mẻ và cấp đủ dòng 5V ổn định.

---

### Câu 26 (Slide 26)

**Câu hỏi:** What is the clock speed for the microcontroller of Arduino Uno R3?

**Các lựa chọn:**
- **A.** 5 MHz
- **B.** 8 MHz
- **C.** IO MHz
- **D.** 16 MHz

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (16 MHz)

**💡 Giải thích chi tiết:** Tần số xung nhịp (Clock speed) chuẩn của bo mạch Arduino Uno R3 là 16 MHz.

---

### Câu 27 (Slide 27)

**Câu hỏi:** What is the size of the EEPROM of the Arduino Uno R3Q

**Các lựa chọn:**
- **A.** 1 KB
- **B.** 2KB
- **C.** 4KB
- **D.** 8 KB

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (1 KB)

**💡 Giải thích chi tiết:** Vi điều khiển ATmega328P trên Arduino Uno R3 có dung lượng bộ nhớ bất biến EEPROM tích hợp là 1 KB (1024 bytes).

---

### Câu 28 (Slide 28)

**Câu hỏi:** What is the size of the SRAM of the Arduino Uno R3Q

**Các lựa chọn:**
- **A.** 1 KB
- **B.** 2KB
- **C.** 4KB
- **D.** 8KB

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (2KB)

**💡 Giải thích chi tiết:** Dung lượng bộ nhớ RAM tĩnh (SRAM) của Arduino Uno R3 là 2 KB (2048 bytes), dùng để lưu trữ các biến tạm thời khi chạy chương trình.

---

### Câu 29 (Slide 29)

**Câu hỏi:** What is the size of the flash memory of the microcontroller of Arduino Uno Rev3?

**Các lựa chọn:**
- **A.** 32 KB
- **B.** 40 KB
- **C.** 64 KB
- **D.** 128 KB

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (32 KB)

**💡 Giải thích chi tiết:** Dung lượng bộ nhớ Flash (bộ nhớ lưu mã chương trình) của vi điều khiển ATmega328P trên Arduino Uno Rev3 là 32 KB (trong đó 0.5 KB dành cho bootloader).

---

### Câu 30 (Slide 30)

**Câu hỏi:** What is the resolution of analog readings on the Arduino Uno?

**Các lựa chọn:**
- **A.** 5\//1023
- **B.** 3.3V/1024
- **C.** 5V/1024
- **D.** 3.3V/1023 Resolution :

- **Đáp án trong ghi chú:** `C Arduino chuyển đổi tất cả các điện áp tương tự (0V đến 5V hoặc 3.3V) được nhận làm đầu vào thành một dải điện áp từ 0 đến 1023. Điều này được thực hiện bằng cách ánh xạ các mức điện áp. Trên Arduino Uno, mức điện áp tối đa là 5V và bộ chuyển đổi ADC tích hợp có độ phân giải 10 bit, có nghĩa là nó có thể chia tín hiệu tương tự nhận được thành 2¹⁰ mức.`
- **Đáp án chính xác:** **C** (5V/1024)

> ⚠️ LƯU Ý ĐÁP ÁN: File gốc chọn C (5V/1024) dựa trên 2^10 = 1024 mức rời rạc (bước lượng tử q = Vref/2^n). Tuy nhiên, trên slide có in kèm công thức Resolution = Vref/(2^n - 1) = 5V/1023 (Đáp án A). Trong đề thi nếu hỏi theo công thức trên slide là A, nếu hỏi theo số mức lượng tử lý thuyết ADC là C.

**💡 Giải thích chi tiết:** ⚠️ LƯU Ý ĐÁP ÁN: File gốc chọn C (5V/1024). Với ADC 10-bit, dải giá trị chia thành 2^10 = 1024 mức rời rạc, bước lượng tử q = 5V / 1024 ≈ 4.88 mV. Tuy nhiên hình trên slide in công thức Resolution = Vref / (2^n - 1) = 5V / 1023 (Đáp án A). Cần lưu ý tùy theo đề bài yêu cầu theo công thức hay số mức rời rạc.

---

### Câu 31 (Slide 31)

**Câu hỏi:** What is the purpose of the following Arduino code?

**Các lựa chọn:**
- **A.** Send a signal to pin 40 on the Arduino board
- **B.** Send an octal number of 40 through the Serial pins
- **C.** Send a byte with value 40 through the Serial pins
- **D.** Send a hexadecimal number of 40 through the Serial pins

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Send a byte with value 40 through the Serial pins)

**💡 Giải thích chi tiết:** Hàm Serial.write(40) thực hiện gửi một byte có giá trị 40 qua cổng nối tiếp Serial (UART).

---

### Câu 32 (Slide 32)

**Câu hỏi:** What is the frequency band of Bluetooth technology?

**Các lựa chọn:**
- **A.** 2.4 to 2.78 GHz
- **B.** 2.4 to 2.48 GHz
- **C.** 2.4 to 2.68 GHz
- **D.** 2.4 to 3.18 GHz

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (2.4 to 2.48 GHz)

**💡 Giải thích chi tiết:** Công nghệ Bluetooth hoạt động trong dải tần vô tuyến công nghiệp, khoa học và y tế (ISM band) ở dải tần số 2.4 GHz đến 2.4835 GHz (khoảng 2.4 - 2.48 GHz).

---

### Câu 33 (Slide 33)

**Câu hỏi:** What is the correct syntax to make a digital pin (say D7) as an output pin?

**Các lựa chọn:**
- **A.** pinMode(7, output)
- **B.** pinMode(7, Output)
- **C.** pinMode(7, OUTPUT)
- **D.** pinmode(7, OUTPUT)

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (pinMode(7, OUTPUT))

**💡 Giải thích chi tiết:** Cú pháp chuẩn để cấu hình một chân số làm đầu ra trong Arduino C là pinMode(7, OUTPUT) với từ khóa OUTPUT viết hoa toàn bộ và tên hàm là pinMode.

---

### Câu 34 (Slide 34)

**Câu hỏi:** What is the correct syntax to output a string like: "I like IoT' in C program?

**Các lựa chọn:**
- **A.** System.out.println("l like IOT");
- **B.** Console_writeLine("I like IoT');
- **C.** System.output("l like IoT");
- **D.** printf("lI like loT");

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (printf("lI like loT");)

**💡 Giải thích chi tiết:** Trong ngôn ngữ lập trình C chuẩn, hàm xuất chuỗi ký tự ra màn hình console là printf("..."). Các hàm khác thuộc về Java (System.out.println) hoặc C# (Console.WriteLine).

---

### Câu 35 (Slide 35)

**Câu hỏi:** What are the two pins of Arduino Uno for 12C protocol?

**Các lựa chọn:**
- **A.** A1, A2
- **B.** DI, D2
- **C.** A4,A5
- **D.** D4, D5

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (A4,A5)

**💡 Giải thích chi tiết:** Trên bo mạch Arduino Uno, giao thức I2C sử dụng 2 chân analog A4 (SDA - Serial Data) và A5 (SCL - Serial Clock).

---

### Câu 36 (Slide 36)

**Câu hỏi:** What will be the output of the following Arduino code?

**Các lựa chọn:**
- **A.** 0xAB
- **B.** 0xa
- **C.** 10
- **D.** Error

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (Error)

**💡 Giải thích chi tiết:** Macro tiền xử lý #define X 10 định nghĩa X là một hằng số. Trong hàm setup(), câu lệnh gán X = 0 cố tình gán lại giá trị cho hằng số sẽ gây lỗi biên dịch (Compilation Error).

---

### Câu 37 (Slide 37)

**Câu hỏi:** What will be the output of the following Arduino code?

**Các lựa chọn:**
- **A.** 10
- **B.** 0
- **C.** Error
- **D.** 0x0

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (0x0)

**💡 Giải thích chi tiết:** Tương tự, câu lệnh gán X = 0 cho một hằng số được định nghĩa bởi macro #define sẽ bị trình biên dịch báo lỗi (Error).

---

### Câu 38 (Slide 38)

**Câu hỏi:** What pins of Arduino Uno are the external interrupt pins?

**Các lựa chọn:**
- **A.** 2,3
- **B.** 3, 4
- **C.** 5,6
- **D.** 7,8

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (2,3)

**💡 Giải thích chi tiết:** Arduino Uno R3 hỗ trợ 2 chân ngắt ngoài phần cứng chuyên dụng là Digital Pin 2 (ứng với Interrupt 0) và Digital Pin 3 (ứng với Interrupt 1).

---

### Câu 39 (Slide 39)

**Câu hỏi:** What resistance value does a resistor with brown, black, and red bands indicate?

**Các lựa chọn:**
- **A.** 1kQ
- **B.** 10 kQ
- **C.** 100 Q Giå tri dien tro (Giå tri dåi thü nhåt x 10 + Giå tri dåi tho hai) x He Sö nhån Åp dung cåc giå tri måu b.n dä cung cäp: DSi thü nhät (Nau - Brown): Giå tri 1 • Dåi thü hai (Den - Black): Giå tri O Dåi thü ba - Red): Hé nhän 100 Thay cåc giå tri våo cong thüc: Giå tri dien tro (1 x 10 + O) x 100 10 x 100 1000 Q
- **D.** 1 Q Gia tri dien tro = (Gia tri dai thu nhat x 10 + Gia tri dai thu hai) x He so nhan Ap dung cac gia tri mau ban da cung cap: ·Dai thu nhat (Nau -Brown): Gia tri 1 Dai thu hai (Den -Black): Gia tri 0 ·Dai thu ba(Do-Red):Hé s6nhan 100 Thay cac gia tri vao cong thuc: Gia tri dien tro = (1 x 10 + 0) x 100 = 10 x 100 = 1000 Ω

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (1kQ)

**💡 Giải thích chi tiết:** Mã màu điện trở: Vạch 1: Nâu (Brown) = 1; Vạch 2: Đen (Black) = 0; Vạch 3: Đỏ (Red) = hệ số nhân 10^2 = 100. Giá trị R = 10 * 100 = 1000 Ω = 1 kΩ.

---

### Câu 40 (Slide 40)

**Câu hỏi:** What happens to the LED's blink rate in the given code when the potentiometer is turned all the way to provide the maximum voltage to the analog pin?

**Các lựa chọn:**
- **A.** The LED blinks faster.
- **B.** The LED blinks slower.
- **C.** The LED stops blinking.
- **D.** The LED blinks at a constant rate regardless of the potentiometer's position.

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (The LED blinks slower.)

**💡 Giải thích chi tiết:** Khi xoay chiết áp đến vị trí điện áp cực đại (5V), hàm analogRead(sensorPin) trả về giá trị lớn nhất (1023). Do đó thời gian delay(sensorValue) tăng lên mức tối đa (~1023ms), làm LED chớp tắt chậm hơn (blinks slower).

---

### Câu 41 (Slide 41)

**Câu hỏi:** What does the analogRead() function return when the potentiometer is turned all the way to connect with the +5 volts?

**Các lựa chọn:**
- **A.** 0
- **B.** Between 1 and 1022
- **C.** 1023
- **D.** 5

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (1023)

**💡 Giải thích chi tiết:** Khi chiết áp được xoay hết cỡ về nguồn +5V, điện áp đưa vào chân analog đạt mức cực đại 5V, do đó bộ ADC 10-bit trả về giá trị số cực đại là 1023.

---

### Câu 42 (Slide 42)

**Câu hỏi:** What type of microcontroller does the Arduino use?

**Các lựa chọn:**
- **A.** 32-bit microcontroller
- **B.** 8-bit microcontroller
- **C.** 16-bit microcontroller
- **D.** 64-bit microcontroller

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (8-bit microcontroller)

**💡 Giải thích chi tiết:** Vi điều khiển ATmega328P sử dụng trên Arduino Uno là dòng vi điều khiển kiến trúc 8-bit RISC.

---

### Câu 43 (Slide 43)

**Câu hỏi:** Which digit does the color violet denote on the first color band of a resistor?

**Các lựa chọn:**
- **A.** 2
- **B.** 5
- **C.** 4
- **D.** 7

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (7)

**💡 Giải thích chi tiết:** Trong bảng mã màu điện trở, vạch màu tím (Violet) đại diện cho chữ số 7 (Đen 0, Nâu 1, Đỏ 2, Cam 3, Vàng 4, Lục 5, Lam 6, Tím 7, Xám 8, Trắng 9).

---

### Câu 44 (Slide 44)

**Câu hỏi:** Which communication range has a distance of about 1 Ocm?

**Các lựa chọn:**
- **A.** NFC
- **B.** RF
- **C.** Wifi
- **D.** Bluetooth

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (NFC)

**💡 Giải thích chi tiết:** Giao tiếp trường gần NFC (Near Field Communication) hoạt động ở khoảng cách rất ngắn, thông thường dưới 10 cm.

---

### Câu 45 (Slide 45)

**Câu hỏi:** Which component is referred to as the 'brain' of the Arduino?

**Các lựa chọn:**
- **A.** ATMega328
- **B.** 16 MHz crystal
- **C.** FTDI USB-to-Serial chip
- **D.** Power regulator

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (ATMega328)

**💡 Giải thích chi tiết:** Vi điều khiển ATmega328P được ví như bộ não (brain) của Arduino Uno, thực thi toàn bộ tập lệnh chương trình.

---

### Câu 46 (Slide 46)

**Câu hỏi:** Which category of actuators includes mechanisms that utilize air pressure to control or move objects?

**Các lựa chọn:**
- **A.** Electrical
- **B.** Mechanical
- **C.** Hydraulic
- **D.** Pneumatic

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (Pneumatic)

**💡 Giải thích chi tiết:** Cơ cấu chấp hành khí nén (Pneumatic actuators) sử dụng áp suất khí nén (air pressure) để tạo ra lực và chuyển động cơ học.

---

### Câu 47 (Slide 47)

**Câu hỏi:** What type of interface is typically used by a fingerprint sensor?

**Các lựa chọn:**
- **A.** UART interface
- **B.** CoAP interface
- **C.** SPI interface
- **D.** I2C interface

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (UART interface)

**💡 Giải thích chi tiết:** Hầu hết các module cảm biến vân tay quang học (như AS608) giao tiếp với vi điều khiển thông qua giao thức nối tiếp bất đồng bộ UART (chân TX/RX).

---

### Câu 48 (Slide 48)

**Câu hỏi:** Which component on tinkercad.com allows displaying the results of the simulation program?

**Các lựa chọn:**
- **A.** Components
- **B.** Send to
- **C.** Start simulation
- **D.** Serial monitor

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (Serial monitor)

**💡 Giải thích chi tiết:** Trên trang Tinkercad Circuits, cửa sổ Serial Monitor cho phép người dùng quan sát dữ liệu in ra từ chương trình mô phỏng vi điều khiển.

---

### Câu 49 (Slide 49)

**Câu hỏi:** Which board is commonly used for IoT projects?

**Các lựa chọn:**
- **A.** Raspberry Pi
- **B.** Arduino UNO
- **C.** BeagleBone Black
- **D.** All of the above

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (All of the above)

**💡 Giải thích chi tiết:** Cả Raspberry Pi, Arduino UNO và BeagleBone Black đều là những bo mạch phát triển phần cứng rất phổ biến trong các ứng dụng và dự án IoT.

---

### Câu 50 (Slide 50)

**Câu hỏi:** Which Arduino model is most commonly used by beginners due to its simplicity and affordability?

**Các lựa chọn:**
- **A.** Due
- **B.** Uno
- **C.** Esplora
- **D.** LilyPad

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (Uno)

**💡 Giải thích chi tiết:** Arduino Uno là phiên bản phổ biến nhất cho người mới bắt đầu nhờ giá thành rẻ, cộng đồng hỗ trợ lớn và nhiều tài liệu hướng dẫn.

---

### Câu 51 (Slide 51)

**Câu hỏi:** Which software is used to upload the Arduino Sketches to the board?

**Các lựa chọn:**
- **A.** Avrgcc
- **B.** g++
- **C.** cpython for windows
- **D.** Avrdude

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (Avrdude)

**💡 Giải thích chi tiết:** avrdude (AVR Downloader/UploaDEr) là phần mềm tiện ích nạp mã nhị phân (.hex) vào bộ nhớ Flash của vi điều khiển AVR trên bo mạch Arduino.

---

### Câu 52 (Slide 52)

**Câu hỏi:** Which function to retrieve text sent from the computer?

**Các lựa chọn:**
- **A.** Serial.readStringUntil('\n')
- **B.** ReadStringUntil('\n')
- **C.** Serial.readingStringUntil("\in')

- **Đáp án trong ghi chú:** `AA`
- **Đáp án chính xác:** **A** (Serial.readStringUntil('\n'))

> ⚠️ LƯU Ý: Ghi chú trong file gốc ghi nhầm "AA" (lặp chữ). Đáp án chuẩn là A: Serial.readStringUntil('\n').

**💡 Giải thích chi tiết:** ⚠️ LƯU Ý: Ghi chú ghi 'AA' do lỗi gõ phím. Đáp án đúng là A: Serial.readStringUntil('\n') dùng để đọc chuỗi ký tự nhận từ máy tính cho đến khi gặp ký tự xuống dòng.

---

### Câu 53 (Slide 53)

**Câu hỏi:** Why is the delay(1000); function used in the Arduino sketch for blinking an LED?

**Các lựa chọn:**
- **A.** To increase the voltage supplied to the LED.
- **B.** To turn the LED off
- **C.** To keep the LED on or off for a visible amount of time.
- **D.** To set the LED_BUILTIN pin as an input.

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (To keep the LED on or off for a visible amount of time.)

**💡 Giải thích chi tiết:** Lệnh delay(1000) được sử dụng để giữ trạng thái LED bật hoặc tắt trong khoảng thời gian 1 giây để mắt người có thể kịp quan sát thấy sự thay đổi.

---

### Câu 54 (Slide 54)

**Câu hỏi:** How many bits are in an IPv6 address? 802

**Các lựa chọn:**
- **A.** 8
- **B.** 32
- **C.** 64
- **D.** 128

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (128)

**💡 Giải thích chi tiết:** Địa chỉ IPv6 có chiều dài 128 bit, được thiết kế để thay thế địa chỉ 32 bit của IPv4 nhằm giải quyết tình trạng cạn kiệt địa chỉ IP.

---

### Câu 55 (Slide 55)

**Câu hỏi:** How many parts of a complete IoT system?

**Các lựa chọn:**
- **A.** 3
- **B.** 4
- **C.** 5
- **D.** 6

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (4)

**💡 Giải thích chi tiết:** Một hệ thống IoT hoàn chỉnh gồm 4 thành phần chính: 1) Sensors/Devices, 2) Connectivity, 3) Data Processing, 4) User Interface.

---

### Câu 56 (Slide 56)

**Câu hỏi:** How many errors are present in the code given below?

**Các lựa chọn:**
- **A.** 1
- **B.** 2
- **C.** 3
- **D.** 4

- **Đáp án trong ghi chú:** `C chỗ này có 2 lỗi lớn nếu tính theo dòng là cái dòng int pin1=12 nó là chân digital , nhưng ở dưới lại viết là analogRead tức là đọc tín hiệu analog từ chân digital nên nó sẽ sai , với cái cái dòng vàng cái chỗ pinmode phải sửa thành pinMode là 1 lỗi nữa , ngoài ra đoạn sau nó quy định chân pin1 là input nma để mỗi là IN nên n sai phải là INPUT , tuy nhiên cái lỗi pin1=12 nó gây tranh cãi vì bản thân nó không phải là lỗi compile nó là lỗi logic . nếu tính khắt khe thì là 3 lỗi còn nếu chỉ quy ước code chạy đúng thì nó chỉ có 2 lỗi thôi nhưng thường thì với môn này ngta hay tính 3 lỗi còn nếu chỉ quy ước code chạy đúng thì nó chỉ có 2 lỗi thôi nhưng thường thì với môn này ngta hay tính 3 lỗi vì nếu n đọc giá trị liên tục mà nó auto là 1 giá trị rời rạc thì n sai về mặt logic`
- **Đáp án chính xác:** **C** (3)

> ⚠️ LƯU Ý ĐÁP ÁN TRANH CÃI: Note chọn C (3 lỗi). Nếu tính lỗi biên dịch (compile error) thì chỉ có 2 lỗi: "pinmode" (phải viết hoa M -> pinMode) và "IN" (phải là INPUT). Lỗi thứ 3 là lỗi logic: "analogRead(pin1)" đọc analog trên chân digital 12 (chân 12 không có bộ ADC, chỉ chân A0-A5 mới đọc được analogRead). Môn IOT102 thường tính 3 lỗi.

**💡 Giải thích chi tiết:** ⚠️ TRANH CÃI ĐÁP ÁN: Note chọn C (3 lỗi). Đoạn mã có 3 lỗi: 1) pinmode viết thường (phải là pinMode); 2) Tham số IN sai (phải là INPUT); 3) chân pin1=12 là digital nhưng lại gọi analogRead(pin1) - lỗi logic đọc analog trên chân không có ADC.

---

### Câu 57 (Slide 57)

**Câu hỏi:** How much space of flash memory does the default bootloader of Arduino Uno take?

**Các lựa chọn:**
- **A.** 06 KB
- **B.** 1 KB
- **C.** 16 KB
- **D.** 32 KB • Flash memory: 32 KB, of which 0.5 KB used by the bootloader

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (06 KB)

**💡 Giải thích chi tiết:** Trình nạp khởi động Optiboot mặc định của Arduino Uno chỉ chiếm dung lượng 0.5 KB (512 bytes) bộ nhớ Flash.

---

### Câu 58 (Slide 58)

**Câu hỏi:** How many pins on Arduino Uno R3 support the pulse width modulation (PWM)? PWM pins in Arduino: Arduino Uno R3 has 6 PWM pins that are 3, 5, 6, 9, 10, and 11. These pins are marked with the negation sign ' ". These pins can generate a pulse as per the given inputs. Arduino supports an 8-bit wide pulse that can have 256 possible levels ( O to 255 ). https://www.geeksforgeeks.org/analog-write-and-working-of-pwm-in-arduino/

**Các lựa chọn:**
- **A.** 7
- **B.** 5
- **C.** 9
- **D.** 6 PWM pins in Arduino: Arduino Uno R3 has 6 PWM pins that are 3, 5, 6, 9, 10, and 11. These pins are marked with the negation sign " ~“. These pins can generate a pulse as per thegiveninputs.Arduinosupportsan8-bitwidepulse thatcanhave 256possiblelevels(0to255). https://www.qeeksforgeeks.org/analog-write-and-working-of-pwm-in-arduino/

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (6 PWM pins in Arduino: Arduino Uno R3 has 6 PWM pins that are 3, 5, 6, 9, 10, and 11. These pins are marked with the negation sign " ~“. These pins can generate a pulse as per thegiveninputs.Arduinosupportsan8-bitwidepulse thatcanhave 256possiblelevels(0to255). https://www.qeeksforgeeks.org/analog-write-and-working-of-pwm-in-arduino/)

**💡 Giải thích chi tiết:** Bo mạch Arduino Uno R3 có 6 chân hỗ trợ xuất xung điều chế độ rộng PWM: chân 3, 5, 6, 9, 10 và 11 (được ký hiệu dấu ~ trên bo mạch).

---

### Câu 59 (Slide 59)

**Câu hỏi:** How many bits does the TCS34725 use for its ADC resolution? A IO-bit with oversampling

**Các lựa chọn:**
- **A.** 10-bit with oversampling
- **B.** 16-bit
- **C.** 12-bit with gain stages
- **D.** 14-bit in fast mode -OR 1' e Hoang H0ång Buön source

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (16-bit)

**💡 Giải thích chi tiết:** Cảm biến màu sắc kỹ thuật số TCS34725 tích hợp bộ chuyển đổi ADC 16-bit độ phân giải cao cho từng kênh màu R, G, B và Clear.

---

### Câu 60 (Slide 60)

**Câu hỏi:** How many bits are in an IPv4 address?

**Các lựa chọn:**
- **A.** 4
- **B.** 16
- **C.** 32
- **D.** 64

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (32)

**💡 Giải thích chi tiết:** Địa chỉ IPv4 có độ dài chuẩn là 32 bit, chia thành 4 octet (mỗi octet 8 bit).

---

### Câu 61 (Slide 61)

**Câu hỏi:** How many groups are an IPv6 represented?

**Các lựa chọn:**
- **A.** 4
- **B.** 8
- **C.** 12
- **D.** 16

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (8)

**💡 Giải thích chi tiết:** Địa chỉ IPv6 được biểu diễn thành 8 nhóm số thập lục phân (hexadecimal), mỗi nhóm gồm 16 bit phân tách bằng dấu hai chấm (:).

---

### Câu 62 (Slide 62)

**Câu hỏi:** How many bits are there in a nibble? One nibble equals four bits. In computing, the term "nibble" (occasionally, the term nybble is used to spell bytes) can also be defined as a 4-bit aggregate known as half an Octet.

**Các lựa chọn:**
- **A.** 2
- **B.** 3
- **C.** 4
- **D.** 5 5 One nibble equals four bits. In computing, the term “nibble" (occasionally, the term nybble is used to spell bytes) can also be defined as a 4-bit aggregate known as half an Octet.

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (4)

**💡 Giải thích chi tiết:** Một Nibble (hoặc nybble) tương đương với đúng 4 bit (nửa byte).

---

### Câu 63 (Slide 63)

**Câu hỏi:** How many pins are there in a 7-segment LED display?

**Các lựa chọn:**
- **A.** 5
- **B.** 7
- **C.** 9
- **D.** 10 total: 10 f com a b 10 9 8 7 6 12 345 com c DP

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (10 total: 10 f com a b 10 9 8 7 6 12 345 com c DP)

**💡 Giải thích chi tiết:** Module LED 7 đoạn đơn chuẩn có tổng cộng 10 chân kết nối: 8 chân điều khiển các đoạn LED (a-g và chấm DP) cùng với 2 chân cấp nguồn chung (Common Anode hoặc Cathode).

---

### Câu 64 (Slide 64)

**Câu hỏi:** How many parts of a complete IoT system? Each application and example of IoT highlights four different integrations of -OR elements: Sensors/devices, Connectivity, Data Processing, and User Interface. 25 thg 7, 2022

**Các lựa chọn:**
- **A.** 3
- **B.** 4
- **C.** 5
- **D.** 6 Each application and example of loT highlights four different integrations of FOR elements:Sensors/devices, Connectivity,Data Processing,and UserInterface.25 thg7,2022

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (4)

**💡 Giải thích chi tiết:** Hệ thống IoT được cấu thành từ 4 thành phần cơ bản: Cảm biến/thiết bị, Kết nối, Xử lý dữ liệu và Giao diện người dùng.

---

### Câu 65 (Slide 65)

**Câu hỏi:** How many bits are in an IPv4 address?

**Các lựa chọn:**
- **A.** 4
- **B.** 16
- **C.** 32
- **D.** 64

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (32)

**💡 Giải thích chi tiết:** Địa chỉ IPv4 có tổng cộng 32 bit.

---

### Câu 66 (Slide 66)

**Câu hỏi:** How many pins are there in a servo motor?

**Các lựa chọn:**
- **A.** 2
- **B.** 3
- **C.** 4
- **D.** 5

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (3)

**💡 Giải thích chi tiết:** Động cơ servo tiêu chuẩn (như SG90) có 3 chân kết nối: VCC (nguồn 5V), GND (đất) và Signal (chân nhận tín hiệu PWM).

---

### Câu 67 (Slide 67)

**Câu hỏi:** A part of an Arduino sketch is as follows. How long is the built-in LED on?

**Các lựa chọn:**
- **A.** 1 second
- **B.** 2 seconds
- **C.** 1000 seconds
- **D.** Infinite

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (1000 seconds)

**💡 Giải thích chi tiết:** Đoạn code: digitalWrite(13, HIGH); delay(1000); bật LED trong 1000 mili giây, tức là LED sáng trong đúng 1 giây.

---

### Câu 68 (Slide 68)

**Câu hỏi:** A part of an Arduino sketch is as follows. What is the frequency of the waveform at digital pin D11?

**Các lựa chọn:**
- **A.** 2 Hz
- **B.** 5 Hz
- **C.** 200 Hz
- **D.** 500 Hz

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (2 Hz)

**💡 Giải thích chi tiết:** Chu kỳ sóng: T = 300 ms + 200 ms = 500 ms = 0.5 s. Tần số f = 1 / T = 1 / 0.5 = 2 Hz.

---

### Câu 69 (Slide 69)

**Câu hỏi:** If the following are the parameters of ADC, Vref = 5V, and a 10-bit AID output code is OxlAB, what is the ADC input voltage?

**Các lựa chọn:**
- **A.** 1.685V
- **B.** 2.085V
- **C.** 1.885V
- **D.** 2.285V

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (2.085V)

**💡 Giải thích chi tiết:** Đổi 0x1AB sang thập phân: 427. Điện áp Vin = (427 / 1023) * 5V ≈ 2.085V.

---

### Câu 70 (Slide 70)

**Câu hỏi:** If a resistor has bands of yellow, violet, and orange, what would be its resistance value?

**Các lựa chọn:**
- **A.** 43 kilo Ohms
- **B.** 470 Ohms
- **C.** 47 kilo Ohms
- **D.** 4.7 kilo Ohms

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (47 kilo Ohms)

**💡 Giải thích chi tiết:** Mã màu điện trở: Vàng (4), Tím (7), Cam (10^3 = 1k). Giá trị = 47 * 10^3 Ω = 47 kΩ (47 kilo Ohms).

---

### Câu 71 (Slide 71)

**Câu hỏi:** If the following are the parameters of ADC, Vref = 5V, and a IO-bit AID output code is OxlAB, what is the ADC input voltage?

**Các lựa chọn:**
- **A.** 1 685V
- **B.** 2085V
- **C.** 1 885V
- **D.** 2.285V

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (2085V)

**💡 Giải thích chi tiết:** Tương tự câu 69: Giá trị Vin = (427 / 1023) * 5V ≈ 2.085V.

---

### Câu 72 (Slide 72)

**Câu hỏi:** In code: pinMode(2, INPUT PULLUP); When the button is not pressed, and the internal pull-up resistor is enabled on digital pin 2, what is the voltage level on this pin?

**Các lựa chọn:**
- **A.** O volts
- **B.** 5 volts
- **C.** 3B volts
- **D.** It depends on the button's position

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (5 volts)

**💡 Giải thích chi tiết:** Khi cấu hình pinMode(2, INPUT_PULLUP), điện trở kéo lên nội bộ kết nối chân 2 với nguồn 5V. Khi nút bấm chưa được nhấn (hở mạch), điện áp trên chân 2 ở mức HIGH (5 volts).

---

### Câu 73 (Slide 73)

**Câu hỏi:** If a resistor has bands of yellow, violet, and orange, what would be its resistance value?

**Các lựa chọn:**
- **A.** 43 kilo Ohms
- **B.** 470 Ohms
- **C.** 47 kilo Ohms
- **D.** 4.7 kilo Ohms

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (47 kilo Ohms)

**💡 Giải thích chi tiết:** Điện trở màu Vàng (4), Tím (7), Cam (hệ số 10^3) có giá trị là 47 kilo Ohms.

---

### Câu 74 (Slide 74)

**Câu hỏi:** In circuit design, choose the correct usage for the LED component with Arduino board

**Các lựa chọn:**
- **A.** Anode of the LED component will indirectly connected by a resistor to 5V pin in Arduino board and cathode of the LED component is connected to the AO pin in the Arduino board.
- **B.** Anode of the LED component will indirectly connected by a resistor to 5V pin in Arduino board and the cathode of the LED component is connected to the 3V pin in the Arduino board.
- **C.** Anode of the LED component will indirectly connected by a resistor to 5V pin in Arduino board and cathode of the LED component is connected to the 5V pin in the Arduino board.
- **D.** Anode of the LED component will indirectly connected by a resistor to a 5V pin in Arduino board and cathode of the LED component is connected to the TX pin in the Arduino board.

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (Anode of the LED component will indirectly connected by a resistor to 5V pin in Arduino board and cathode of the LED component is connected to the AO pin in the Arduino board.)

**💡 Giải thích chi tiết:** Mạch LED chuẩn: Cực dương (Anode) nối qua điện trở hạn dòng tới nguồn 5V hoặc chân I/O, cực âm (Cathode) nối với đất (GND) hoặc chân điều khiển.

---

### Câu 75 (Slide 75)

**Câu hỏi:** The first three color bands of a 4-band resistor are brown, green, and yellow. What is its value?

**Các lựa chọn:**
- **A.** 364 Ohm
- **B.** 150k Ohm
- **C.** 65 Ohm
- **D.** 2800 Ohm

- **Đáp án trong ghi chú:** `đen nâu đỏ cam vàng lụm lam tím xám trắng => B`
- **Đáp án chính xác:** **B** (150k Ohm)

**💡 Giải thích chi tiết:** Vạch màu Nâu (1), Lục (5), Vàng (hệ số 10^4). Giá trị = 15 * 10^4 Ω = 150 kΩ.
[Ghi chú gốc từ slide]: đen nâu đỏ cam vàng lụm lam tím xám trắng => B

---

### Câu 76 (Slide 76)

**Câu hỏi:** The digital pin D2 of Arduino Uno generates a square wave, making an LED on for 1 second and off for 4 seconds. If the LED's anode is connected to 5 V and the LED's cathode is connected to pin D2, what is the duty cycle of this square wave?

**Các lựa chọn:**
- **A.** 20%
- **B.** 25%
- **C.** 80%
- **D.** 90%

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (80%)

**💡 Giải thích chi tiết:** LED nối Anode vào 5V, Cathode vào D2. Khi LED sáng (1s), D2 ở mức LOW. Khi LED tắt (4s), D2 ở mức HIGH. Chu kỳ T = 1s + 4s = 5s. Độ rộng xung HIGH chiếm 4s / 5s = 80% (Duty cycle = 80%).

---

### Câu 77 (Slide 77)

**Câu hỏi:** To declare a variable that stores the value read from analog pin AO, what data type is this variable?

**Các lựa chọn:**
- **A.** String
- **B.** Single
- **C.** Double
- **D.** Int

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (Int)

**💡 Giải thích chi tiết:** Hàm analogRead() trả về giá trị số nguyên từ 0 đến 1023, do đó biến lưu trữ giá trị đọc được phải có kiểu số nguyên int.

---

### Câu 78 (Slide 78)

**Câu hỏi:** P, V, and I denote the power, voltage, and current, respectively. Which formula is correct?

**Các lựa chọn:**
- **A.** P=VA2xR
- **B.** P=V^2/R
- **C.** P -Vx IA2
- **D.** P = V/lA2 P: VA2/R = IA2.R

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (P=V^2/R)

**💡 Giải thích chi tiết:** Theo định luật Ohm và công thức công suất: P = V * I = V^2 / R = I^2 * R. Công thức đúng là P = V^2 / R.

---

### Câu 79 (Slide 79)

**Câu hỏi:** For a voltage dividercircuit with R1=10kOhm and R2=15kOhm.IfVin=12V andVout is the voltagebetweentwoendsofR1,whatisthevalueofVout?

**Các lựa chọn:**
- **A.** 4.8 V
- **B.** 4V
- **C.** 8V
- **D.** 72 v 10kO x 12V out — 10kQ + 15kO out = For a voltage divider circuit with RI = 10k Ohm and R2 = 15k Ohm. If Vin = 12V and Vout is the • RI = 10kQ • R2=15kO • Vin=12V RI RI + R2

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (4.8 V)

**💡 Giải thích chi tiết:** Cầu phân áp: Vout (trên R1) = Vin * R1 / (R1 + R2) = 12V * 10k / (10k + 15k) = 12V * (10 / 25) = 4.8V.

---

### Câu 80 (Slide 80)

**Câu hỏi:** Given the nominal voltage of an AAA battery is 1.5 V, what is the nominal voltage of 5 AAA batteries connected in parallel? ASV

**Các lựa chọn:**
- **A.** 6V
- **B.** 7.5V
- **C.** 9V
- **D.** 1.5V

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (1.5V)

**💡 Giải thích chi tiết:** Khi mắc 5 viên pin 1.5V song song với nhau, hiệu điện thế tổng của bộ nguồn không thay đổi và vẫn bằng hiệu điện thế của một viên pin là 1.5V (chỉ dung lượng dòng Ah tăng gấp 5).

---

### Câu 81 (Slide 81)

**Câu hỏi:** Given an array as follows [4, 1, 2, 9, 81. How is the array like after the first round of Bubble sort?

**Các lựa chọn:**
- **A.** 4, 1, 2, 9, 8
- **B.** 1, 2, 4, 8, 9
- **C.** 1,4, 2, 8, 9
- **D.** 1, 4, 2, 9, 8

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (1, 2, 4, 8, 9)

**💡 Giải thích chi tiết:** Thuật toán Bubble sort trên mảng [4, 1, 2, 9, 8]: Lần 1: hoán đổi (4,1)->[1,4,2,9,8]; hoán đổi (4,2)->[1,2,4,9,8]; so sánh (4,9) giữ nguyên; hoán đổi (9,8)->[1,2,4,8,9]. Kết quả sau vòng đầu là 1, 2, 4, 8, 9.

---

### Câu 82 (Slide 82)

**Câu hỏi:** On the Arduino Uno, how many analog input pins are available, and how many of the digital input/output pins can be used as PWM outputs?

**Các lựa chọn:**
- **A.** Analog Inputs: 6, PWM Outputs: 6
- **B.** Analog Inputs. 14, PWM Outputs. 14
- **C.** Analog Inputs. 6, PWM Outputs: 14
- **D.** Analog Inputs: 14, PWM Outputs_ 6

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (Analog Inputs: 6, PWM Outputs: 6)

**💡 Giải thích chi tiết:** Bo mạch Arduino Uno có 6 chân đầu vào analog (A0 đến A5) và 6 chân đầu ra điều chế xung PWM (chân 3, 5, 6, 9, 10, 11).

---

### Câu 83 (Slide 83)

**Câu hỏi:** You are reading data from a DS18B20 temperature sensor (using 1 -Wire communication) on Arduino. After reading, the temperature value you get is rawTemp = OXOI 91. How do you convert this value to degrees Celsius?

**Các lựa chọn:**
- **A.** float tempC = (float)rawTemp / 16.0;
- **B.** float tempC = (fioat)rawTemp * 0.625;
- **C.** float tempC = (float)rawTemp / 256.0;
- **D.** float tempC = (rawTemp >> 4);

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (float tempC = (float)rawTemp / 16.0;)

**💡 Giải thích chi tiết:** Cảm biến nhiệt độ DS18B20 có độ phân giải 12-bit với bước nhảy 0.0625°C (tương đương 1/16). Để đổi từ giá trị thô rawTemp sang độ Celsius: tempC = (float)rawTemp / 16.0.

---

## Phần 2: Câu hỏi Answer Ngắn (Short Concept Questions)

### Câu 85 (Slide 85)

**Câu hỏi:** What is a common mistake to check if an Arduino program doesn't compile?

**Các lựa chọn:**
- **A.** Incorrect USB cable
- **B.** Missing semicolon
- **C.** Wrong breadboard size
- **D.** Faulty LED

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (Missing semicolon)

**💡 Giải thích chi tiết:** Lỗi phổ biến nhất khiến chương trình Arduino không thể biên dịch thành công là quên dấu chấm phẩy (Missing semicolon ;) ở cuối câu lệnh.

---

### Câu 86 (Slide 86)

**Câu hỏi:** What is the MAX7219 module commonly used for? A Audio output

**Các lựa chọn:**
- **A.** Audio output
- **B.** LED matrix display control
- **C.** Temperature measurement
- **D.** Power supply regulation e Hoang H0ång Buön Source

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (LED matrix display control)

**💡 Giải thích chi tiết:** IC MAX7219 là vi mạch điều khiển hiển thị LED chuyên dụng (LED matrix display control / 7-segment display driver) qua giao tiếp nối tiếp 3 dây.

---

### Câu 87 (Slide 87)

**Câu hỏi:** What is the default 12C clock speed on the Arduino Uno? A 100 kHz

**Các lựa chọn:**
- **A.** 100 kHz
- **B.** 400 kHz
- **C.** 16 MHz
- **D.** IO kHz

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (100 kHz)

**💡 Giải thích chi tiết:** Tốc độ xung nhịp chuẩn mặc định của giao thức I2C trên Arduino Uno là 100 kHz (Standard mode).

---

### Câu 88 (Slide 88)

**Câu hỏi:** What is one of the primary concerns with the growing number of connected devices? A The number of available IP addresses

**Các lựa chọn:**
- **A.** The number of available IP addresses
- **B.** The security and privacy of data
- **C.** The aesthetic design of devices
- **D.** The speed of the intermet connection

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (The security and privacy of data)

**💡 Giải thích chi tiết:** Mối lo ngại lớn nhất khi số lượng thiết bị kết nối IoT bùng nổ là an toàn thông tin và quyền riêng tư dữ liệu (The security and privacy of data).

---

### Câu 89 (Slide 89)

**Câu hỏi:** What is the process of identifying a trusted device in IoT network?

**Các lựa chọn:**
- **A.** Auditing
- **B.** Authorization
- **C.** Authentication
- **D.** Accounting

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Authentication)

**💡 Giải thích chi tiết:** Quá trình xác nhận danh tính của một thiết bị hoặc người dùng tin cậy trong mạng IoT được gọi là Xác thực (Authentication).

---

### Câu 90 (Slide 90)

**Câu hỏi:** What is the purpose of the delay function in the sensor reading loop?

**Các lựa chọn:**
- **A.** To set the sensor range
- **B.** To avoid serial monitor overload
- **C.** To control the brightness of LED
- **D.** To initialize the pins

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (To avoid serial monitor overload)

**💡 Giải thích chi tiết:** Trong vòng lặp đọc cảm biến, hàm delay() giúp hạn chế tần suất gửi dữ liệu, tránh làm quá tải bộ đệm cổng nối tiếp (To avoid serial monitor overload).

---

### Câu 91 (Slide 91)

**Câu hỏi:** What is one of the primary components that need to be secured in an IoT system? A The software of the user's mobile phone

**Các lựa chọn:**
- **A.** The software of the user's mobilephone
- **B.** The devices, network, programs, and data
- **C.** The cloud storage location
- **D.** The intemet service provider

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (The devices, network, programs, and data)

**💡 Giải thích chi tiết:** Để bảo vệ toàn diện hệ thống IoT, cần bảo mật đồng thời cả 4 thành phần: thiết bị phần cứng, đường truyền mạng, phần mềm chương trình và dữ liệu người dùng.

---

### Câu 92 (Slide 92)

**Câu hỏi:** What is the role of a network router in an IoT system?

**Các lựa chọn:**
- **A.** Processing data locally
- **B.** Converting AC to DC
- **C.** Directing data between devices
- **D.** Controlling actuator movements

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Directing data between devices)

**💡 Giải thích chi tiết:** Vai trò của thiết bị định tuyến (Router) trong mạng IoT là điều hướng và chuyển tiếp các gói tin dữ liệu giữa các thiết bị với nhau và ra ngoài Internet.

---

### Câu 93 (Slide 93)

**Câu hỏi:** What is Arduino? A Programming language

**Các lựa chọn:**
- **A.** Programminglanguage
- **B.** Open-source electronics platform
- **C.** Image editing software
- **D.** Text editor
- **E.** None of the others

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (Open-source electronics platform)

**💡 Giải thích chi tiết:** Arduino là một nền tảng điện tử mã nguồn mở (Open-source electronics platform) bao gồm cả phần cứng có thể lập trình và phần mềm (IDE).

---

### Câu 94 (Slide 94)

**Câu hỏi:** What is the role of the ATMega168/328 in an Arduino circuit?

**Các lựa chọn:**
- **A.** Run the program.
- **B.** To regulate the power supply.
- **C.** To provide Wi-Fi connectivity.
- **D.** To filter analog signals.

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (Run the program.)

**💡 Giải thích chi tiết:** Vi điều khiển ATmega168/328 đóng vai trò là chip xử lý trung tâm, có nhiệm vụ lưu trữ và thực thi chương trình của người dùng.

---

### Câu 95 (Slide 95)

**Câu hỏi:** What is the type of USB port on Arduino Uno R3?

**Các lựa chọn:**
- **A.** Type A
- **B.** Type B
- **C.** Type C
- **D.** Micro USB

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (Type B)

**💡 Giải thích chi tiết:** Bo mạch Arduino Uno R3 sử dụng cổng nạp USB Type-B tiêu chuẩn (loại cổng vuông thường dùng trên máy in).

---

### Câu 96 (Slide 96)

**Câu hỏi:** What is the default bootloader of Arduino Uno?

**Các lựa chọn:**
- **A.** Barebox
- **B.** Optiboot
- **C.** U-Boot
- **D.** Lilo

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (Optiboot)

**💡 Giải thích chi tiết:** Trình nạp khởi động mặc định trên Arduino Uno là Optiboot.

---

### Câu 97 (Slide 97)

**Câu hỏi:** What is the term for the extension of the existing Internet structure to billions of connected devices?

**Các lựa chọn:**
- **A.** Digitization
- **B.** M2M
- **C.** IoT
- **D.** 82B

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (IoT)

**💡 Giải thích chi tiết:** Mạng lưới kết nối internet mở rộng tới hàng tỷ đồ vật vật lý được gọi là Internet of Things (IoT).

---

### Câu 98 (Slide 98)

**Câu hỏi:** What is the unit of inductance?

**Các lựa chọn:**
- **A.** Farad
- **B.** Henry
- **C.** Ohm
- **D.** Voltage

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (Henry)

**💡 Giải thích chi tiết:** Đơn vị đo độ tự cảm của cuộn cảm trong hệ SI là Henry (H).

---

### Câu 99 (Slide 99)

**Câu hỏi:** What is the default bootloader of Arduino Uno?

**Các lựa chọn:**
- **A.** Barebox
- **B.** Optiboot
- **C.** U-Boot
- **D.** Lilo

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (Optiboot)

**💡 Giải thích chi tiết:** Trình nạp khởi động mặc định trên Arduino Uno là Optiboot.

---

### Câu 100 (Slide 100)

**Câu hỏi:** What is the other name of hardware address?

**Các lựa chọn:**
- **A.** MAC address
- **B.** IP address
- **C.** Postal address
- **D.** Gateway address

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (MAC address)

**💡 Giải thích chi tiết:** Địa chỉ phần cứng gắn liền với card mạng (NIC) được gọi là địa chỉ MAC (Media Access Control address).

---

### Câu 101 (Slide 101)

**Câu hỏi:** What is DHTII?

**Các lựa chọn:**
- **A.** Proximity sensor
- **B.** Touch sensor
- **C.** Pressure sensor
- **D.** Temperature and humidity sensor
- **E.** None of the others

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (Temperature and humidity sensor)

**💡 Giải thích chi tiết:** DHT11 là module cảm biến kỹ thuật số dùng để đo đồng thời cả nhiệt độ và độ ẩm không khí.

---

### Câu 102 (Slide 102)

**Câu hỏi:** What is the default bootloader of the Arduino UNO?

**Các lựa chọn:**
- **A.** AIR-boot
- **B.** GAG
- **C.** Optiboot bootloader
- **D.** Bare box

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Optiboot bootloader)

**💡 Giải thích chi tiết:** Bootloader mặc định nạp sẵn trên chip ATmega328P của Arduino UNO là Optiboot bootloader.

---

### Câu 103 (Slide 103)

**Câu hỏi:** What is the use of the ESP8266 WiFi Module?

**Các lựa chọn:**
- **A.** Network Provider
- **B.** Switches circuits
- **C.** Evaluates air pressure
- **D.** Monitors Motion

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (Network Provider)

**💡 Giải thích chi tiết:** Module Wi-Fi SoC ESP8266 cho phép vi điều khiển kết nối vào mạng Wi-Fi và truyền nhận dữ liệu qua giao thức TCP/IP.

---

### Câu 104 (Slide 104)

**Câu hỏi:** What is the term for the extension of the existing Internet structure to billions of connected devices?

**Các lựa chọn:**
- **A.** Digitization
- **B.** M2M
- **C.** IoT
- **D.** 82B

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (IoT)

**💡 Giải thích chi tiết:** Khái niệm mở rộng cấu trúc Internet tới hàng tỷ thiết bị kết nối được định nghĩa là Internet of Things (IoT).

---

### Câu 105 (Slide 105)

**Câu hỏi:** What does NFC stand for? A Near Fast Connection

**Các lựa chọn:**
- **A.** NearFast Connection
- **B.** Near Field Connection
- **C.** Near Fast Communication
- **D.** Near Field Communication

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (Near Field Communication)

**💡 Giải thích chi tiết:** NFC là viết tắt của cụm từ Near Field Communication (Giao tiếp trường gần).

---

### Câu 106 (Slide 106)

**Câu hỏi:** What does a fog extend cloud to?

**Các lựa chọn:**
- **A.** Application to process logic
- **B.** Storage of processed data
- **C.** Things that process and act on data
- **D.** Hardware for executing boot loading

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Things that process and act on data)

**💡 Giải thích chi tiết:** Điện toán sương mù (Fog computing) mở rộng tài nguyên đám mây xuống biên mạng - nơi các 'vật' (Things) trực tiếp thu thập, xử lý và phản ứng với dữ liệu.

---

### Câu 107 (Slide 107)

**Câu hỏi:** What additional consideration is necessary to make an IoT project successful compared to existing solutions?

**Các lựa chọn:**
- **A.** Focus on expensive materials
- **B.** Implement the latest IoT protocols
- **C.** Be better than current solutions
- **D.** Use cutting-edge programming languages

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Be better than current solutions)

**💡 Giải thích chi tiết:** Để một dự án IoT thành công so với các giải pháp truyền thống, nó phải mang lại giá trị vượt trội, hiệu quả hơn và giải quyết bài toán tốt hơn giải pháp hiện tại.

---

### Câu 108 (Slide 108)

**Câu hỏi:** What pin mode is used for the button in the Arduino setup code?

**Các lựa chọn:**
- **A.** OUTPUT
- **B.** INPUT
- **C.** ANALOG
- **D.** PWM

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (INPUT)

**💡 Giải thích chi tiết:** Đối với nút nhấn đơn giản, chân kết nối trên Arduino cần được thiết lập ở chế độ INPUT hoặc INPUT_PULLUP để đọc trạng thái đóng/ngắt mạch.

---

### Câu 109 (Slide 109)

**Câu hỏi:** What type of loop is used to repeatedly check a sensor?

**Các lựa chọn:**
- **A.** FOR loop
- **B.** LOOPO function
- **C.** setup() function
- **D.** check() function

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (LOOPO function)

**💡 Giải thích chi tiết:** Trong cấu trúc chương trình Arduino, hàm loop() là vòng lặp vô tận được hệ thống tự động gọi lặp đi lặp lại liên tục để kiểm tra trạng thái cảm biến.

---

### Câu 110 (Slide 110)

**Câu hỏi:** What color represents the digit 6 in the resistor color band?

**Các lựa chọn:**
- **A.** blue
- **B.** orange
- **C.** white
- **D.** black

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (blue)

**💡 Giải thích chi tiết:** Mã màu điện trở: Màu xanh lam (Blue) đại diện cho chữ số 6.

---

### Câu 111 (Slide 111)

**Câu hỏi:** What kind of control system in which the output quantity has no effect upon the input quantity?

**Các lựa chọn:**
- **A.** Open loop
- **B.** Closed loop
- **C.** Variable
- **D.** Non-variable

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (Open loop)

**💡 Giải thích chi tiết:** Hệ thống điều khiển vòng hở (Open loop) là hệ thống mà tín hiệu đầu ra không có bất kỳ phản hồi nào ảnh hưởng ngược lại đến tín hiệu điều khiển ở đầu vào.

---

### Câu 112 (Slide 112)

**Câu hỏi:** What does the statement delay(IOOO); do in Arduino C?

**Các lựa chọn:**
- **A.** Repeat the program 1000 times
- **B.** Pause the program for 1000 microseconds
- **C.** Pause the program for 1 second
- **D.** Send data after 1 second

- **Đáp án trong ghi chú:** `C Trong Arduino, hàm delay(x) làm chương trình tạm dừng trong x mili giây (milliseconds) . ● delay(1000) = 1000 ms = 1 giây . ● Trong thời gian này, chương trình sẽ không thực hiện các lệnh tiếp theo.`
- **Đáp án chính xác:** **C** (Pause the program for 1 second)

**💡 Giải thích chi tiết:** Lệnh delay(1000) tạm dừng chương trình trong đúng 1000 mili giây (tức 1 giây).
[Ghi chú gốc từ slide]: C Trong Arduino, hàm delay(x) làm chương trình tạm dừng trong x mili giây (milliseconds) . ● delay(1000) = 1000 ms = 1 giây . ● Trong thời gian này, chương trình sẽ không thực hiện các lệnh tiếp theo.

---

### Câu 113 (Slide 113)

**Câu hỏi:** What role do gas monitoring systems play in IoT-enabled mining operations?

**Các lựa chọn:**
- **A.** They reduce the number of gas emissions
- **B.** They detect harmful gases
- **C.** They automate mining drills
- **D.** They track the amount of fuel used

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (They detect harmful gases)

**💡 Giải thích chi tiết:** Trong ngành khai thác mỏ, hệ thống giám sát khí ga IoT có vai trò tối quan trọng là phát hiện kịp thời các khí độc hại và khí dễ cháy nổ (They detect harmful gases) để bảo vệ tính mạng công nhân.

---

### Câu 114 (Slide 114)

**Câu hỏi:** What happens if pinMode is not set for a pin before digitalWrite?

**Các lựa chọn:**
- **A.** It works as expected
- **B.** The pin stays in input mode
- **C.** The sketch won't compile
- **D.** It creates random output

- **Đáp án trong ghi chú:** ``
- **Đáp án chính xác:** **B** (The pin stays in input mode)

> ⚠️ CÂU THIẾU ĐÁP ÁN TRONG FILE GỐC: Slide 114 không có ghi chú trong file PPTX. Đáp án chuẩn xác là B: The pin stays in input mode.

**💡 Giải thích chi tiết:** ⚠️ CÂU THIẾU NOTE GỐC: Đáp án là B. Khi khởi động, các chân I/O trên vi điều khiển AVR mặc định ở chế độ INPUT. Nếu gọi digitalWrite() mà chưa cấu hình pinMode(OUTPUT), chân đó vẫn ở chế độ INPUT.

---

### Câu 115 (Slide 115)

**Câu hỏi:** What type of communication does the RX and TX pins on the Arduino Uno facilitate?

**Các lựa chọn:**
- **A.** Power transfer
- **B.** Wireless communication
- **C.** Serial communication
- **D.** Analog signal processing

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Serial communication)

**💡 Giải thích chi tiết:** Hai chân RX (chân 0) và TX (chân 1) trên Arduino Uno hỗ trợ giao tiếp nối tiếp UART (Serial communication) để truyền nhận dữ liệu với máy tính hoặc vi điều khiển khác.

---

### Câu 116 (Slide 116)

**Câu hỏi:** What technique is used to create an analog-like behavior from a digital output?

**Các lựa chọn:**
- **A.** Serial communication
- **B.** Pulse Width Modulation (PWM)
- **C.** Digital-to-Analog Conversion (DAC)
- **D.** Analog-to-Digital Conversion (ADC)

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (Pulse Width Modulation (PWM))

**💡 Giải thích chi tiết:** Chuyển đổi tín hiệu analog sang dạng số rời rạc được gọi là quá trình ADC (Analog-to-Digital Conversion).

---

### Câu 117 (Slide 117)

**Câu hỏi:** What type of signal does the analogWrite() function output? A Pulse Code Modulated Signal

**Các lựa chọn:**
- **A.** Pulse Code Modulated Signal
- **B.** Frequency Modulated Signal
- **C.** Pulse Width Modulated Signal
- **D.** Pulse Amplitude Modulated Signal

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Pulse Width Modulated Signal)

**💡 Giải thích chi tiết:** Trong ngôn ngữ Arduino C/C++, kiểu dữ liệu số nguyên int trên Arduino Uno chiếm 16 bit (2 bytes) và có dải giá trị từ -32,768 đến 32,767.

---

### Câu 118 (Slide 118)

**Câu hỏi:** What type of device could allow a vehicle to place a show a warning on the dashboard, which might also notify the car's manufacturer?

**Các lựa chọn:**
- **A.** Digital network
- **B.** Smart phone
- **C.** Sensor
- **D.** Bluetooth

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Sensor)

**💡 Giải thích chi tiết:** Giao thức I2C chỉ cần đúng 2 đường dây tín hiệu: SDA (Serial Data) và SCL (Serial Clock).

---

### Câu 119 (Slide 119)

**Câu hỏi:** What type of actuator is typically used to control the movement of a conveyor belt?

**Các lựa chọn:**
- **A.** Electrical
- **B.** Hydraulic
- **C.** Mechanical
- **D.** Pneumatic

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (Electrical)

**💡 Giải thích chi tiết:** Hàm digitalRead(pin) đọc mức logic trên chân số và trả về HIGH (1) hoặc LOW (0).

---

### Câu 120 (Slide 120)

**Câu hỏi:** What feature of IPv6 makes it particularly suitable for IoT? A It provides many more IP addresses.

**Các lựa chọn:**
- **A.** It provides many moreIP addresses.
- **B.** It has better encryption.
- **C.** It uses less power.
- **D.** It is easier to remember.

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (It provides many moreIP addresses.)

**💡 Giải thích chi tiết:** Cảm biến LDR (quang điện trở) thay đổi giá trị điện trở tùy thuộc vào cường độ ánh sáng chiếu vào bề mặt cảm biến.

---

### Câu 121 (Slide 121)

**Câu hỏi:** What programming language is primarily used by the Arduino IDE in IoT software development for writing code? A Python

**Các lựa chọn:**
- **A.** Python
- **B.** Java
- **C.** C/C++
- **D.** JavaScript

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (C/C++)

**💡 Giải thích chi tiết:** Cổng USB trên Arduino Uno vừa dùng để nạp code (chuyển đổi USB-Serial), vừa cấp nguồn 5V cho bo mạch và hỗ trợ giao tiếp Serial Monitor.

---

### Câu 122 (Slide 122)

**Câu hỏi:** What programming language is used for a sketch in Arduino IDE?

**Các lựa chọn:**
- **A.** Python
- **B.** Java
- **C.** C/C++
- **D.** Assembly

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (C/C++)

**💡 Giải thích chi tiết:** Đơn vị đo điện dung của tụ điện trong hệ đo lường quốc tế SI là Farad (F).

---

### Câu 123 (Slide 123)

**Câu hỏi:** What component needs to connect to an interrupt pin to use the external interrupt on Arduino?

**Các lựa chọn:**
- **A.** LED
- **B.** Resistor
- **C.** Button
- **D.** Capacitor

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Button)

**💡 Giải thích chi tiết:** Chuẩn giao tiếp SPI (Serial Peripheral Interface) là giao tiếp nối tiếp đồng bộ 4 dây: MISO, MOSI, SCK, SS.

---

### Câu 124 (Slide 124)

**Câu hỏi:** What type of sensor is the LM35?

**Các lựa chọn:**
- **A.** Pressure sensor
- **B.** Humidity sensor
- **C.** Temperature sensor
- **D.** Touch sensor

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Temperature sensor)

**💡 Giải thích chi tiết:** Một hệ thống IoT gồm 4 thành phần thiết yếu: Cảm biến, Kết nối mạng, Xử lý dữ liệu và Giao diện người dùng.

---

### Câu 125 (Slide 125)

**Câu hỏi:** What type of sensor detects motion or presence using infrared light?

**Các lựa chọn:**
- **A.** Hall effect sensor
- **B.** Photoresistor
- **C.** Infrared sensor
- **D.** Force sensitive resistor

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Infrared sensor)

**💡 Giải thích chi tiết:** Điện áp danh định cấp từ cổng USB tiêu chuẩn của máy tính là 5V DC.

---

### Câu 126 (Slide 126)

**Câu hỏi:** What material is used as the sensing element in the MQ135?

**Các lựa chọn:**
- **A.** Tin dioxide (Sn02)
- **B.** Zinc oxide (ZnO)
- **C.** Silicon carbide (SiC)
- **D.** Titanium dioxide (TIO:)

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (Tin dioxide (Sn02))

**💡 Giải thích chi tiết:** Chất bán dẫn phổ biến nhất được sử dụng để chế tạo các linh kiện điện tử vi mạch là Silic (Silicon).

---

### Câu 127 (Slide 127)

**Câu hỏi:** What feature helps the MAX30102 reduce power consumption? A Duty-cycle modulation mode

**Các lựa chọn:**
- **A.** Duty-cycle modulation mode
- **B.** Shutdown mode
- **C.** Adaptive sampling rate
- **D.** Standby with FIFO buffering

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (Shutdown mode)

**💡 Giải thích chi tiết:** Địa chỉ MAC là địa chỉ vật lý duy nhất của phần cứng mạng, có độ dài cố định 48 bit (6 octet).

---

### Câu 128 (Slide 128)

**Câu hỏi:** What value range is used with the analogWrite() function for PWM control?

**Các lựa chọn:**
- **A.** Oto 1023
- **B.** ot05
- **C.** O to 255
- **D.** -255 to 255

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (O to 255)

**💡 Giải thích chi tiết:** Điện trở kéo lên (Pull-up resistor) giữ cho chân tín hiệu ở mức logic cao xác định (HIGH) khi nút bấm chưa được nhấn, tránh hiện tượng chân bị thả nổi (floating).

---

### Câu 129 (Slide 129)

**Câu hỏi:** What type of network does the Wi-Fi shield allow the Arduino to connect to?

**Các lựa chọn:**
- **A.** A Bluetooth network
- **B.** A wired Ethernet network
- **C.** A Wi-Fi network
- **D.** A ZigBee mesh network e HOång HOång Buön souræ

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (A Wi-Fi network)

**💡 Giải thích chi tiết:** Hàm millis() trả về số mili giây kể từ lúc bo mạch Arduino bắt đầu chạy chương trình hiện tại mà không làm chặn (non-blocking) luồng thực thi.

---

### Câu 130 (Slide 130)

**Câu hỏi:** What type of light does the TCS34725 measure in addition to RGB?

**Các lựa chọn:**
- **A.** Infrared filtered channel
- **B.** Clear light
- **C.** Narrowband blue light
- **D.** Polarized light

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (Clear light)

**💡 Giải thích chi tiết:** Cảm biến DHT11 truyền dữ liệu nhiệt độ và độ ẩm qua một dây tín hiệu số duy nhất (Single-wire two-way digital bus).

---

### Câu 131 (Slide 131)

**Câu hỏi:** What symbol is used to indicate a comment in C?

**Các lựa chọn:**
- **A.** //
- **B.** #
- **C.** <>
- **D.** &

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (//)

**💡 Giải thích chi tiết:** Ký hiệu hai dấu gạch chéo // được sử dụng để bắt đầu một dòng chú thích (single-line comment) trong ngôn ngữ C/C++.

---

### Câu 132 (Slide 132)

**Câu hỏi:** Which of the following is an example of an IoT device? A Smart thermostat

**Các lựa chọn:**
- **A.** Smart thermostat
- **B.** Traditional desktop computer
- **C.** Mechanical typewriter
- **D.** Standard light bulb

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (Smart thermostat)

**💡 Giải thích chi tiết:** Hàm analogWrite(pin, val) xuất tín hiệu điều chế độ rộng xung (PWM) với giá trị chu kỳ nhiệm vụ từ 0 (0% duty cycle) đến 255 (100% duty cycle).

---

### Câu 133 (Slide 133)

**Câu hỏi:** Which of the following is an example of an authentication method used in IoT devices?

**Các lựa chọn:**
- **A.** Biometric data
- **B.** Data encryption
- **C.** Data backup
- **D.** Device size reduction

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (Biometric data)

**💡 Giải thích chi tiết:** Định luật Ohm thiết lập mối quan hệ cơ bản trong mạch điện một chiều: V = I * R (Hiệu điện thế bằng Cường độ dòng điện nhân Điện trở).

---

### Câu 134 (Slide 134)

**Câu hỏi:** Which of the following devices is considered an input device in an IoT system?

**Các lựa chọn:**
- **A.** Microcontroller
- **B.** Temperature sensor
- **C.** LCD screen
- **D.** Servo motor

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (Temperature sensor)

**💡 Giải thích chi tiết:** Tần số xung nhịp dao động chuẩn của Arduino Uno là 16 MHz.

---

### Câu 135 (Slide 135)

**Câu hỏi:** Which data type is used to store integer values in C?

**Các lựa chọn:**
- **A.** float
- **B.** char
- **C.** int
- **D.** double

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (int)

**💡 Giải thích chi tiết:** IC chuyển đổi giao tiếp USB-sang-Serial trên Arduino Uno R3 chính hãng là ATmega16U2 (hoặc CH340 trên các bản clone).

---

### Câu 136 (Slide 136)

**Câu hỏi:** Which command is used to read the state of a digital input pin? A digitalRead()

**Các lựa chọn:**
- **A.** digitalRead()
- **B.** analogRead()
- **C.** pinRead()
- **D.** getPinState()

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (digitalRead())

**💡 Giải thích chi tiết:** Bộ vi điều khiển chính xử lý mọi tác vụ trên bo mạch Arduino Uno là chip ATmega328P.

---

### Câu 137 (Slide 137)

**Câu hỏi:** Which communication protocol does the MAX30102 use?

**Các lựa chọn:**
- **A.** SPI with open-drain outputs
- **B.** Inter-lntegrated Circuit
- **C.** UART with parity bit
- **D.** SWD debug interface

- **Đáp án trong ghi chú:** ``
- **Đáp án chính xác:** **B** (Inter-lntegrated Circuit)

> ⚠️ CÂU THIẾU ĐÁP ÁN TRONG FILE GỐC: Slide 137 không có ghi chú trong file PPTX. Đáp án chuẩn xác là B: Inter-Integrated Circuit (I2C).

**💡 Giải thích chi tiết:** ⚠️ CÂU THIẾU NOTE GỐC: Đáp án là B. Module cảm biến đo nhịp tim & nồng độ oxy trong máu MAX30102 sử dụng giao thức truyền thông I2C (Inter-Integrated Circuit).

---

### Câu 138 (Slide 138)

**Câu hỏi:** Which Arduino function is specifically used to link a servo object to a designated control pin on the board?

**Các lựa chọn:**
- **A.** myservo.connect()
- **B.** myservo.attach()
- **C.** myservo.link()
- **D.** myservo-bind()

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (myservo.attach())

**💡 Giải thích chi tiết:** Khi đấu nối LED vào mạch, luôn cần mắc nối tiếp một điện trở hạn dòng (current-limiting resistor) để tránh dòng điện vượt quá mức tối đa làm cháy LED.

---

### Câu 139 (Slide 139)

**Câu hỏi:** Which function is used to create a PWM signal to dim an LED?

**Các lựa chọn:**
- **A.** analogWrite(pin, value);
- **B.** digitalWrite(pin, value);
- **C.** pwmSend(pin, value);
- **D.** fade(pin, value);

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (analogWrite(pin, value);)

**💡 Giải thích chi tiết:** Trong mô hình kiến trúc IoT nhiều tầng, tầng cảm nhận (Perception Layer) chịu trách nhiệm thu thập các thông số vật lý từ môi trường qua các cảm biến.

---

### Câu 140 (Slide 140)

**Câu hỏi:** Which layer of IoT architecture involves sensors and devices that collect data? A Perception layer

**Các lựa chọn:**
- **A.** Perception layer
- **B.** Network layer
- **C.** Application layer
- **D.** Data layer

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (Perception layer)

**💡 Giải thích chi tiết:** Tầng cảm nhận (Perception layer) bao gồm các cảm biến và thiết bị đầu cuối trực tiếp tiếp xúc và đo đạc dữ liệu từ thế giới thực.

---

### Câu 141 (Slide 141)

**Câu hỏi:** Which Arduino command is used to generate a pulse width modulated signal?

**Các lựa chọn:**
- **A.** analogWrite()
- **B.** tone()
- **C.** digitalRead()
- **D.** digitalWrite()

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (analogWrite())

**💡 Giải thích chi tiết:** Hàm analogWrite() trong Arduino được sử dụng để tạo ra tín hiệu điều chế độ rộng xung PWM trên các chân hỗ trợ.

---

### Câu 142 (Slide 142)

**Câu hỏi:** Which board is the Arduino's first development board to use one microcontroller with built-in USB?

**Các lựa chọn:**
- **A.** Lily Pad
- **B.** Uno
- **C.** RedBoard
- **D.** Leonardo

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (Leonardo)

**💡 Giải thích chi tiết:** Arduino Leonardo là bo mạch đầu tiên tích hợp vi điều khiển ATmega32u4 có sẵn khối phần cứng USB bên trong chip, cho phép giả lập bàn phím/chuột mà không cần IC chuyển đổi USB ngoài.

---

### Câu 143 (Slide 143)

**Câu hỏi:** Which microcontroller does Arduino Uno use?

**Các lựa chọn:**
- **A.** ATmega328P
- **B.** ESP32
- **C.** STM32
- **D.** Raspberry Pi

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (ATmega328P)

**💡 Giải thích chi tiết:** Bo mạch Arduino Uno sử dụng vi điều khiển chính là chip ATmega328P của hãng Atmel/Microchip.

---

### Câu 144 (Slide 144)

**Câu hỏi:** Which command is used to read a signal from an analog temperature sensor?

**Các lựa chọn:**
- **A.** digitalRead(AO);
- **B.** analogRead(A0);
- **C.** readSensor();
- **D.** input(A0);

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (analogRead(A0);)

**💡 Giải thích chi tiết:** Để đọc giá trị điện áp từ cảm biến nhiệt độ analog (như LM35), ta sử dụng hàm analogRead(A0).

---

### Câu 145 (Slide 145)

**Câu hỏi:** Which factors must be considered when aligning multiple IoT devices in a network to work together efficiently? (Select all that apply)

**Các lựa chọn:**
- **A.** Interoperability
- **B.** Communication latency
- **C.** Power source compatibility
- **D.** Device color coding

- **Đáp án trong ghi chú:** `ABC`
- **Đáp án chính xác:** **A, B, C** (A. Interoperability; B. Communication latency; C. Power source compatibility)

> ⚠️ CÂU HỎI CHỌN NHIỀU ĐÁP ÁN (Select all that apply): Slide ghi chú chọn ABC. Cần chọn cả 3 phương án A, B và C.

**💡 Giải thích chi tiết:** ⚠️ CHỌN NHIỀU ĐÁP ÁN: Khi kết nối nhiều thiết bị IoT, cần xem xét Khả năng tương tác (A), Độ trễ truyền thông (B), và Tính tương thích nguồn điện (C). Mã màu vỏ (D) không ảnh hưởng kỹ thuật.

---

### Câu 146 (Slide 146)

**Câu hỏi:** Which medium is best suited for long-distance, high-speed communication?

**Các lựa chọn:**
- **A.** Copper cables
- **B.** Fibre optic cables
- **C.** Wireless transmission
- **D.** Plastic wires

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (Fibre optic cables)

**💡 Giải thích chi tiết:** Cáp quang (Fibre optic cables) là môi trường truyền dẫn tốt nhất cho cự ly dài và tốc độ cao nhờ sử dụng ánh sáng truyền trong sợi thủy tinh, không bị suy hao hay nhiễu điện từ.

---

### Câu 147 (Slide 147)

**Câu hỏi:** Which of the following is an example of an output device?

**Các lựa chọn:**
- **A.** Temperature sensor
- **B.** LED
- **C.** Microphone
- **D.** Touchscreen

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (LED)

**💡 Giải thích chi tiết:** LED (Light Emitting Diode) là một cơ cấu đầu ra (Output device / Actuator) chuyển đổi năng lượng điện thành ánh sáng. Cảm biến nhiệt, microphone, màn hình cảm ứng là thiết bị đầu vào.

---

### Câu 148 (Slide 148)

**Câu hỏi:** Which port is commonly used to connect input/output modules to Arduino?

**Các lựa chọn:**
- **A.** GPIO
- **B.** USB
- **C.** HDMI
- **D.** Ethernet

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (GPIO)

**💡 Giải thích chi tiết:** Các chân GPIO (General-Purpose Input/Output) là các cổng đa dụng được dùng phổ biến nhất để kết nối module ngoại vi vào/ra với Arduino.

---

### Câu 149 (Slide 149)

**Câu hỏi:** Which actuator types operate using pressurized fluids or gases? (Select all that apply)

**Các lựa chọn:**
- **A.** Pneumatic
- **B.** Hydraulic
- **C.** Electrical
- **D.** Mechanical spring

- **Đáp án trong ghi chú:** `AB`
- **Đáp án chính xác:** **A, B** (A. Pneumatic; B. Hydraulic)

> ⚠️ CÂU HỎI CHỌN NHIỀU ĐÁP ÁN (Select all that apply): Slide ghi chú chọn AB. Cần chọn cả 2 phương án A và B.

**💡 Giải thích chi tiết:** ⚠️ CHỌN NHIỀU ĐÁP ÁN: Cơ cấu chấp hành bằng áp suất chất lưu gồm: Khí nén (A. Pneumatic - dùng khí áp suất) và Thủy lực (B. Hydraulic - dùng chất lỏng áp suất).

---

### Câu 150 (Slide 150)

**Câu hỏi:** Which board is commonly used for IoT projects? A Raspberry Pi

**Các lựa chọn:**
- **A.** RaspberryPi
- **B.** Arduino UNO
- **C.** BeagleBone Black
- **D.** All of the above

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (All of the above)

**💡 Giải thích chi tiết:** Cả Raspberry Pi, Arduino UNO và BeagleBone Black đều là các nền tảng phần cứng phát triển IoT thông dụng.

---

### Câu 151 (Slide 151)

**Câu hỏi:** Which category of actuators includes mechanisms that utilize air pressure to control or move objects?

**Các lựa chọn:**
- **A.** Electrical
- **B.** Mechanical
- **C.** Hydraulic
- **D.** Pneumatic

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (Pneumatic)

**💡 Giải thích chi tiết:** Cơ cấu chấp hành khí nén (Pneumatic) sử dụng áp suất khí (air pressure) để tạo lực đẩy và chuyển động.

---

### Câu 152 (Slide 152)

**Câu hỏi:** Which function in the Arduino is used to initialize the serial communication?

**Các lựa chọn:**
- **A.** Serial.println()
- **B.** Serial.available()
- **C.** Serial.read()
- **D.** Serial.begin()

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (Serial.begin())

**💡 Giải thích chi tiết:** Hàm Serial.begin(baudrate) được dùng để khởi tạo và mở cổng truyền thông nối tiếp UART với tốc độ baud xác định.

---

### Câu 153 (Slide 153)

**Câu hỏi:** Which component on tinkercad.com allows displaying the results of the simulation program?

**Các lựa chọn:**
- **A.** Components
- **B.** Send to
- **C.** Start simulation
- **D.** Serial monitor

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (Serial monitor)

**💡 Giải thích chi tiết:** Trên Tinkercad, cửa sổ Serial Monitor hiển thị dữ liệu văn bản từ hàm Serial.print() trong quá trình mô phỏng.

---

### Câu 154 (Slide 154)

**Câu hỏi:** Which device commonly uses binary states to store information?

**Các lựa chọn:**
- **A.** Resistor
- **B.** Transistor
- **C.** Capacitor
- **D.** Inductor

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (Transistor)

**💡 Giải thích chi tiết:** Transistor (bóng bán dẫn) là linh kiện cốt lõi được sử dụng ở 2 trạng thái đóng/ngắt (nhị phân 0 và 1) để lưu trữ và xử lý thông tin trong mạch kỹ thuật số.

---

### Câu 155 (Slide 155)

**Câu hỏi:** Which of the following is used for comments in Arduino sketch?

**Các lựa chọn:**
- **A.** /*comment*/
- **B.** l/ comment /
- **C.** // comment
- **D.** both // comment and / comment *I

- **Đáp án trong ghi chú:** `D D phải là both // comment and /* comment */ mới đúng`
- **Đáp án chính xác:** **D** (both // comment and / comment *I)

> ⚠️ LƯU Ý LỖI IN TRÊN SLIDE: Slide in nhầm phương án D thành "both // comment and/comment*/" (thiếu dấu sao). Note giải thích chuẩn: Phải là cả hai cú pháp // và /* comment */.

**💡 Giải thích chi tiết:** ⚠️ LƯU Ý LỖI IN: Cú pháp chú thích hợp lệ trong Arduino C gồm cả // (chú thích một dòng) và /* ... */ (chú thích nhiều dòng).

---

### Câu 156 (Slide 156)

**Câu hỏi:** Which of the following IoT network topologies provides the highest reliability?

**Các lựa chọn:**
- **A.** Star topology
- **B.** Mesh topology
- **C.** Bus topology
- **D.** Ring topology

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (Mesh topology)

**💡 Giải thích chi tiết:** Mô hình mạng lưới (Mesh topology) mang lại độ tin cậy cao nhất vì nếu một nút gặp sự cố, các nút còn lại tự động tìm đường định tuyến thay thế.

---

### Câu 157 (Slide 157)

**Câu hỏi:** Which of the following could be an IOT device?

**Các lựa chọn:**
- **A.** A lamp
- **B.** A pen
- **C.** A couch
- **D.** All of the mentioned

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (All of the mentioned)

**💡 Giải thích chi tiết:** Mọi đồ vật trong cuộc sống (đèn, bút, ghế sofa...) đều có thể trở thành thiết bị IoT nếu được gắn thêm cảm biến, bộ xử lý và khả năng kết nối mạng.

---

### Câu 158 (Slide 158)

**Câu hỏi:** Which part of the ATmega328p is responsible for executing instructions?

**Các lựa chọn:**
- **A.** Flash memory
- **B.** ALU
- **C.** EEPROM
- **D.** UART

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (ALU)

**💡 Giải thích chi tiết:** Đơn vị số học và logic ALU (Arithmetic Logic Unit) trong CPU của ATmega328P chịu trách nhiệm thực thi các phép toán và lệnh của chương trình.

---

### Câu 159 (Slide 159)

**Câu hỏi:** Which of the following is not an example of an open loop system?

**Các lựa chọn:**
- **A.** Automatic water faucet
- **B.** Traffic signals
- **C.** Electronic lift
- **D.** Automatic electric iron

- **Đáp án trong ghi chú:** `D. not examlple -> Automatic eletric iron`
- **Đáp án chính xác:** **D** (Automatic electric iron)

> ⚠️ CÂU HỎI PHỦ ĐỊNH (NOT open-loop): Note giải thích đáp án là D (Automatic electric iron).

**💡 Giải thích chi tiết:** ⚠️ CÂU PHỦ ĐỊNH: Bàn ủi điện tự động (Automatic electric iron) có bộ cảm ứng nhiệt thermostat để tự đóng ngắt duy trì nhiệt độ -> là hệ thống điều khiển vòng kín (closed-loop), KHÔNG PHẢI vòng hở.

---

### Câu 160 (Slide 160)

**Câu hỏi:** Which type of network is the connection between a Bluetooth headset and a smartphone?

**Các lựa chọn:**
- **A.** PAN
- **B.** MAN
- **C.** LAN
- **D.** WAN

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (PAN)

**💡 Giải thích chi tiết:** Kết nối giữa tai nghe Bluetooth và điện thoại thông minh thuộc loại mạng cá nhân PAN (Personal Area Network).

---

### Câu 161 (Slide 161)

**Câu hỏi:** Which Arduino function is used to stop an active interrupt?

**Các lựa chọn:**
- **A.** detachlnterrupt()
- **B.** interruptOff()
- **C.** disablelSR()
- **D.** stoplnterrupt()

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (detachlnterrupt())

**💡 Giải thích chi tiết:** Để hủy kích hoạt và dừng một ngắt ngoài đang hoạt động trên Arduino, sử dụng hàm detachInterrupt(pin).

---

### Câu 162 (Slide 162)

**Câu hỏi:** Which issue in the cloud focuses on protecting data from theft or corruption?

**Các lựa chọn:**
- **A.** DATA PRIVATE
- **B.** DATA ACCESS
- **C.** DATA THEFT
- **D.** SECURE NETWORK

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (DATA THEFT)

**💡 Giải thích chi tiết:** Vấn đề bảo mật dữ liệu khỏi bị đánh cắp hoặc xâm phạm trái phép trên nền tảng đám mây tập trung vào Data Theft / Data Protection.

---

### Câu 163 (Slide 163)

**Câu hỏi:** Which industry benefits the most from IoT?

**Các lựa chọn:**
- **A.** Healthcare
- **B.** Traditional farming
- **C.** Printing press
- **D.** Textile industry

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (Healthcare)

**💡 Giải thích chi tiết:** Ngành chăm sóc sức khỏe y tế (Healthcare) là một trong những lĩnh vực hưởng lợi nhiều nhất từ IoT thông qua theo dõi bệnh nhân từ xa, thiết bị đeo thông minh...

---

### Câu 164 (Slide 164)

**Câu hỏi:** Which protocol is most commonly used for small data transmission in IoT devices?

**Các lựa chọn:**
- **A.** HTTP
- **B.** MQTT
- **C.** FTP
- **D.** SMTP

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (MQTT)

**💡 Giải thích chi tiết:** MQTT là giao thức gọn nhẹ tiêu chuẩn được dùng rộng rãi nhất để truyền tải dữ liệu kích thước nhỏ cho các thiết bị IoT.

---

### Câu 165 (Slide 165)

**Câu hỏi:** Which mode parameter triggers the interrupt when the pin goes from Iow to high?

**Các lựa chọn:**
- **A.** LOW
- **B.** CHANGE
- **C.** RISING
- **D.** FALLING

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (RISING)

**💡 Giải thích chi tiết:** Tham số RISING trong hàm attachInterrupt() kích hoạt ngắt khi mức logic trên chân chuyển từ mức thấp lên mức cao (LOW sang HIGH).

---

### Câu 166 (Slide 166)

**Câu hỏi:** Which button in the ESP8266 is used to load the code again?

**Các lựa chọn:**
- **A.** GND
- **B.** TX
- **C.** A1
- **D.** A0

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (GND)

> ⚠️ LƯU Ý THUẬT NGỮ: Câu hỏi ghi "Which button..." nhưng các đáp án lại là tên chân (GND, TX, A1, A0). Note chọn A (GND).

**💡 Giải thích chi tiết:** ⚠️ LƯU Ý: Chân GPIO0 trên ESP8266 cần được kéo xuống mức thấp (nối đất GND) khi khởi động để đưa chip vào chế độ nạp chương trình (Flash Mode).

---

### Câu 167 (Slide 167)

**Câu hỏi:** Which communication range has a distance of about I Ocm?

**Các lựa chọn:**
- **A.** NFC
- **B.** RF
- **C.** Wifi
- **D.** Bluetooth

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (NFC)

**💡 Giải thích chi tiết:** NFC (Near Field Communication) là công nghệ truyền thông không dây tầm ngắn với khoảng cách hoạt động khoảng 10 cm.

---

### Câu 168 (Slide 168)

**Câu hỏi:** Which pins support the serial communication between the Arduino Uno communicate and the computer?

**Các lựa chọn:**
- **A.** UART pins
- **B.** ADC pins
- **C.** 12C pins
- **D.** PWM pins

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (UART pins)

**💡 Giải thích chi tiết:** Các chân UART (chân 0 RX và chân 1 TX) hỗ trợ giao tiếp nối tiếp trực tiếp giữa vi điều khiển Arduino Uno và máy tính.

---

### Câu 169 (Slide 169)

**Câu hỏi:** Which digital pin is used as the LED BUILTIN value on an Arduino UNO board?

**Các lựa chọn:**
- **A.** D10
- **B.** Dll
- **C.** D12
- **D.** D13

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (D13)

**💡 Giải thích chi tiết:** Trên bo mạch Arduino Uno, đèn LED tích hợp sẵn (LED_BUILTIN) được kết nối cố định với chân Digital D13.

---

### Câu 170 (Slide 170)

**Câu hỏi:** Which operation is appropriate when system calls notify the OS that the file is comming and set some of its attributes? Delete

**Các lựa chọn:**
- **A.** Delete
- **B.** Create
- **C.** Read
- **D.** Write

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (Create)

**💡 Giải thích chi tiết:** Lời gọi hệ thống Create được sử dụng khi hệ điều hành cần tạo lập và thiết lập các thuộc tính ban đầu cho một file mới.

---

### Câu 171 (Slide 171)

**Câu hỏi:** Which function in the Arduino is used to initialize the serial communication?

**Các lựa chọn:**
- **A.** Serial.println()
- **B.** Serial.available()
- **C.** Serial.read()
- **D.** Serial.begin()

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (Serial.begin())

**💡 Giải thích chi tiết:** Hàm Serial.begin(baud) được dùng để khởi tạo cổng giao tiếp nối tiếp Serial trên Arduino.

---

### Câu 172 (Slide 172)

**Câu hỏi:** Which function to retrieve text sent from the computer? B- ReadStringUntil('\n')

**Các lựa chọn:**
- **A.** Serial.readStringUntil(\n')
- **B.** ReadStringUntil("in')
- **C.** Serial.readingStringUntil(\n')

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (Serial.readStringUntil(\n'))

**💡 Giải thích chi tiết:** Hàm Serial.readStringUntil('\n') đọc chuỗi ký tự nhận từ máy tính qua cổng Serial cho đến khi gặp ký tự ngắt dòng.

---

### Câu 173 (Slide 173)

**Câu hỏi:** Which function below is used to configure pins as input or output?

**Các lựa chọn:**
- **A.** DigitalWrite()
- **B.** pinMode()
- **C.** DigitalRead()
- **D.** Println()

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (pinMode())

**💡 Giải thích chi tiết:** Hàm pinMode(pin, mode) được dùng để cấu hình chế độ hoạt động cho chân vi điều khiển là INPUT hoặc OUTPUT.

---

### Câu 174 (Slide 174)

**Câu hỏi:** Which protocol is suitable for IoT devices requiring low power and low data rate communication over a few kilometers?

**Các lựa chọn:**
- **A.** Bluetooth
- **B.** Zigbee
- **C.** LoRaWAN
- **D.** WiFi

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (LoRaWAN)

**💡 Giải thích chi tiết:** LoRaWAN là công nghệ mạng diện rộng công suất thấp (LPWAN) lý tưởng cho các thiết bị IoT cần truyền dữ liệu cự ly xa vài kilômét với mức tiêu thụ điện cực nhỏ.

---

### Câu 175 (Slide 175)

**Câu hỏi:** Which sensor is LM35?

**Các lựa chọn:**
- **A.** Pressure sensor
- **B.** Humidity sensor
- **C.** Touch sensor
- **D.** Temperature sensor

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (Temperature sensor)

**💡 Giải thích chi tiết:** LM35 là cảm biến nhiệt độ dạng analog tuyến tính với độ chính xác cao.

---

### Câu 176 (Slide 176)

**Câu hỏi:** Which sensor is SRF05?

**Các lựa chọn:**
- **A.** Water level sensor
- **B.** Ranging sensor
- **C.** Sound intensity sensor
- **D.** Temperature sensor

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (Ranging sensor)

**💡 Giải thích chi tiết:** SRF05 là module cảm biến siêu âm đo khoảng cách (ranging sensor) đến vật cản.

---

### Câu 177 (Slide 177)

**Câu hỏi:** Which software is used to upload the Arduino Sketches to the board? A Avrgcc

**Các lựa chọn:**
- **A.** Avrgcc
- **B.** g++
- **C.** cpython for windows
- **D.** Avrdude

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (Avrdude)

**💡 Giải thích chi tiết:** avrdude là công cụ phần mềm mã nguồn mở được dùng để nạp mã máy chương trình vào vi điều khiển AVR.

---

### Câu 178 (Slide 178)

**Câu hỏi:** Which of the following is not a fundamental component of an IoT system?

**Các lựa chọn:**
- **A.** Sensors
- **B.** Connectivity
- **C.** User interface
- **D.** Voltage regulator

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (Voltage regulator)

**💡 Giải thích chi tiết:** Hệ thống IoT gồm Cảm biến, Kết nối mạng và Giao diện người dùng. Bộ ổn áp (Voltage regulator) chỉ là linh kiện nguồn phần cứng phụ trợ.

---

### Câu 179 (Slide 179)

**Câu hỏi:** Which of the following is an example of an IoT device? A Smart thermostat

**Các lựa chọn:**
- **A.** Smart thermostat
- **B.** Calculator
- **C.** Mechanical typewriter
- **D.** Standard light bulb

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (Smart thermostat)

**💡 Giải thích chi tiết:** Bộ điều nhiệt thông minh (Smart thermostat) có khả năng kết nối Wi-Fi, thu thập dữ liệu và tự động điều chỉnh nhiệt độ từ xa là một thiết bị IoT điển hình.

---

### Câu 180 (Slide 180)

**Câu hỏi:** Which communication medium is most affected by environmental conditions like interference? A Fibre optic cables

**Các lựa chọn:**
- **A.** Fibre optic cables
- **B.** Copper cables
- **C.** Wireless transmission
- **D.** All of the others

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Wireless transmission)

**💡 Giải thích chi tiết:** Môi trường truyền dẫn không dây (Wireless transmission) chịu ảnh hưởng lớn nhất từ các điều kiện môi trường như vật cản, nhiễu điện từ và thời tiết.

---

### Câu 181 (Slide 181)

**Câu hỏi:** Which function is used to enable an interrupt in Arduino UNO? A enablelnterrupt()

**Các lựa chọn:**
- **A.** enablelnterrupt()
- **B.** attachlnterrupt()
- **C.** activatelnterrupt()
- **D.** startlnterrupt()

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (attachlnterrupt())

**💡 Giải thích chi tiết:** Hàm attachInterrupt(digitalPinToInterrupt(pin), ISR, mode) được sử dụng để thiết lập và bật ngắt phần cứng trong Arduino.

---

### Câu 182 (Slide 182)

**Câu hỏi:** When was the actual term "Internet of Things" coined? A _ 1998 B- 1999

**Các lựa chọn:**
- **A.** 1998
- **B.** 1999
- **C.** 2001
- **D.** 2002

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (1999)

**💡 Giải thích chi tiết:** Thuật ngữ 'Internet of Things' được Kevin Ashton chính thức đặt ra và sử dụng lần đầu tiên vào năm 1999.

---

### Câu 183 (Slide 183)

**Câu hỏi:** How many digital 1/0 pins does the Arduino Uno have?

**Các lựa chọn:**
- **A.** 8
- **B.** 10
- **C.** 14
- **D.** 16

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (14)

**💡 Giải thích chi tiết:** Bo mạch Arduino Uno R3 có tổng cộng 14 chân Digital I/O (từ chân D0 đến D13).

---

### Câu 184 (Slide 184)

**Câu hỏi:** How many parts of a complete IoT system?

**Các lựa chọn:**
- **A.** 3
- **B.** 4
- **C.** 5
- **D.** 6

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (4)

**💡 Giải thích chi tiết:** Hệ thống IoT hoàn chỉnh gồm 4 thành phần chính: Thiết bị/cảm biến, Kết nối, Xử lý dữ liệu và Giao diện người dùng.

---

### Câu 185 (Slide 185)

**Câu hỏi:** How many wires are used for communication in the 12C protocol?

**Các lựa chọn:**
- **A.** 2
- **B.** 3
- **C.** 8
- **D.** 5

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (2)

**💡 Giải thích chi tiết:** Giao thức I2C sử dụng đúng 2 đường dây tín hiệu: đường dữ liệu SDA và đường xung nhịp SCL.

---

### Câu 186 (Slide 186)

**Câu hỏi:** Who was coined the term "Internet of Things"?

**Các lựa chọn:**
- **A.** Kevin Ashton
- **B.** John Wright
- **C.** Edward Jameson
- **D.** George Garton

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (Kevin Ashton)

**💡 Giải thích chi tiết:** Kevin Ashton là người đầu tiên đặt ra thuật ngữ 'Internet of Things' (IoT).

---

### Câu 187 (Slide 187)

**Câu hỏi:** A huge number of networked devices to communicate without human intervention. What is this called? A IoT B- M2M

**Các lựa chọn:**
- **A.** loT
- **B.** M2M
- **C.** Thingsboard
- **D.** Particle

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (M2M)

**💡 Giải thích chi tiết:** Giao tiếp giữa một số lượng lớn các thiết bị kết nối mạng mà không cần sự can thiệp của con người được gọi là M2M (Machine-to-Machine communication).

---

### Câu 188 (Slide 188)

**Câu hỏi:** A narrow pipe in a water system is analogous to what concept in an electrical circuit?

**Các lựa chọn:**
- **A.** Resistance
- **B.** Voltage
- **C.** Capacitance
- **D.** Current

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (Resistance)

**💡 Giải thích chi tiết:** Trong mô hình dòng nước tương đương mạch điện: một đường ống nước bị thu hẹp cản trở dòng chảy tương đương với Điện trở (Resistance) cản trở dòng điện.

---

### Câu 189 (Slide 189)

**Câu hỏi:** Among the following protocols commonly used in IoT, which one is considered lightweight?

**Các lựa chọn:**
- **A.** IP (Internet Protocol)
- **B.** HTTP (Hypertext Transfer Protocol)
- **C.** MQTT (Message Queuing Telemetry Transport)
- **D.** Bluetooth

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (MQTT (Message Queuing Telemetry Transport))

**💡 Giải thích chi tiết:** Giao thức MQTT (Message Queuing Telemetry Transport) được thiết kế đặc biệt gọn nhẹ (lightweight) dành riêng cho các thiết bị hạn chế băng thông và năng lượng trong IoT.

---

### Câu 190 (Slide 190)

**Câu hỏi:** Consider the statement: "Each resource is either currently assigned to exactly one process or is available." Which of the following is appropriate for this statement?

**Các lựa chọn:**
- **A.** No-preemption
- **B.** Hold-and-wait
- **C.** Mutual exclusion
- **D.** Circular wait

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Mutual exclusion)

**💡 Giải thích chi tiết:** Khái niệm 'Mỗi tài nguyên tại một thời điểm hoặc được gán cho duy nhất một tiến trình hoặc đang rảnh' mô tả điều kiện Loại trừ lẫn nhau (Mutual exclusion) trong hệ điều hành.

---

### Câu 191 (Slide 191)

**Câu hỏi:** To declare a variable that stores the value read from analog pin AO, what data type is this variable?

**Các lựa chọn:**
- **A.** String
- **B.** Single
- **C.** Double
- **D.** Int

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (Int)

**💡 Giải thích chi tiết:** Hàm analogRead() trên Arduino Uno trả về giá trị số nguyên trong dải từ 0 đến 1023 (độ phân giải 10-bit của bộ ADC). Do đó, biến dùng để lưu trữ giá trị này phải được khai báo với kiểu dữ liệu số nguyên int.

---

### Câu 192 (Slide 192)

**Câu hỏi:** In an IoT system, many devices are connected to the same set of wires. What is this connection mode?

**Các lựa chọn:**
- **A.** Train
- **B.** Bus
- **C.** Multi-point connection
- **D.** Serial connection

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (Bus)

**💡 Giải thích chi tiết:** Mô hình mạng mà nhiều thiết bị cùng gắn chung vào một tuyến dây dẫn truyền thông duy nhất được gọi là cấu trúc liên kết đường trục Bus (Bus topology / Bus connection mode).

---

### Câu 193 (Slide 193)

**Câu hỏi:** In the IoT case study of a dairy farm, what is the primary purpose of the responders attached to the cows?

**Các lựa chọn:**
- **A.** To measure the quantity of milk produced by each cow
- **B.** To monitor the health and movement of the cows.
- **C.** To control the feeding mechanism for the cows.
- **D.** To provide a wireless internet connection to the farm.

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (To monitor the health and movement of the cows.)

**💡 Giải thích chi tiết:** Trong ứng dụng IoT chăn nuôi thông minh (Smart Dairy Farming), các thiết bị cảm biến responder gắn trên cổ hoặc tai bò dùng để theo dõi sức khỏe, hành vi vận động và phát hiện sớm dịch bệnh của đàn bò (To monitor the health and movement of the cows).

---

### Câu 194 (Slide 194)

**Câu hỏi:** In the smart grid architecture of IoT, what is the primary function of the Cloud? A Enhancing security

**Các lựa chọn:**
- **A.** Enhancing security
- **B.** Collecting data
- **C.** Managing data
- **D.** Storing data

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Managing data)

**💡 Giải thích chi tiết:** Trong kiến trúc lưới điện thông minh (Smart Grid), điện toán đám mây (Cloud) đóng vai trò trung tâm trong việc quản lý, tổng hợp và điều phối dữ liệu lớn (Managing data) từ hàng triệu đồng hồ đo điện thông minh.

---

### Câu 195 (Slide 195)

**Câu hỏi:** In a typical three-layer IoT architecture, which layer includes sensors, actuators, and RFID tags?

**Các lựa chọn:**
- **A.** Application Layer
- **B.** Data Link Layer
- **C.** Network Layer
- **D.** Perception Layer

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (Perception Layer)

**💡 Giải thích chi tiết:** Trong mô hình kiến trúc IoT 3 tầng (Perception, Network, Application), Tầng cảm nhận (Perception Layer) là tầng thấp nhất chứa các phần cứng cảm biến (sensors), cơ cấu chấp hành (actuators) và thẻ định danh RFID để thu thập dữ liệu vật lý.

---

### Câu 196 (Slide 196)

**Câu hỏi:** In the Linux OS, which key combination stops the ping command in the terminal? A_ Ctrl+Break_ B- Ctrl+D-

**Các lựa chọn:**
- **A.** Ctrl+Break
- **B.** Ctrl+D
- **C.** Ctrl+C
- **D.** Ctrl+Z

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Ctrl+C)

**💡 Giải thích chi tiết:** Trên hệ điều hành Linux/Unix, tổ hợp phím Ctrl + C gửi tín hiệu SIGINT (Interrupt Signal) tới tiến trình đang chạy ở terminal để ngắt và dừng lệnh ping liên tục.

---

### Câu 197 (Slide 197)

**Câu hỏi:** In circuit design, which component is used to limit the current from the arduino board to the LED? A Capacitor

**Các lựa chọn:**
- **A.** Capacitor
- **B.** Diode
- **C.** Resistor
- **D.** Push button

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Resistor)

**💡 Giải thích chi tiết:** Điện trở (Resistor) được mắc nối tiếp với đèn LED nhằm mục đích giới hạn cường độ dòng điện chạy qua LED, bảo vệ LED không bị quá dòng dẫn đến cháy hỏng.

---

### Câu 198 (Slide 198)

**Câu hỏi:** In the IR remote control, IR stands for what? A_ Indirect Radio

**Các lựa chọn:**
- **A.** IndirectRadio
- **B.** Infrared
- **C.** Inside Remote
- **D.** Instant Reception

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (Infrared)

**💡 Giải thích chi tiết:** Trong điều khiển từ xa IR, từ viết tắt IR là viết tắt của Infrared (tia hồng ngoại) - bức xạ điện từ có bước sóng dài hơn ánh sáng khả kiến được dùng để truyền mã điều khiển không dây.

---

### Câu 199 (Slide 199)

**Câu hỏi:** In C programming for IoT, what does digitalWrite(13, HIGH) mean?

**Các lựa chọn:**
- **A.** Write value 13 to pin HIGH
- **B.** Turn off pin 13
- **C.** Turn on pin 13 (set HIGH level)
- **D.** Initialize variable HIGH with value 13

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Turn on pin 13 (set HIGH level))

**💡 Giải thích chi tiết:** Lệnh digitalWrite(13, HIGH) trong Arduino có nghĩa là xuất mức điện áp cao (5V đối với Arduino Uno) ra chân Digital 13, tức là bật chân 13 lên mức HIGH (Turn on pin 13).

---

### Câu 200 (Slide 200)

**Câu hỏi:** Given the nominal voltage of an AAA battery is 1.5 V, what is the nominal voltage of 5 AAA batteries connected in parallel?

**Các lựa chọn:**
- **A.** 6V
- **B.** 7.5V
- **C.** 9V
- **D.** 16 v

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (16 v)

**💡 Giải thích chi tiết:** Khi mắc các viên pin giống nhau song song, hiệu điện thế của bộ nguồn bằng đúng hiệu điện thế của một viên pin thành phần (1.5V), chỉ có dung lượng dòng điện (Ah) là tăng lên.

---

### Câu 201 (Slide 201)

**Câu hỏi:** Given a hash table with size 100 and the Division hashing method is used, in what location will the key 124 be hashed? 24

**Các lựa chọn:**
- **A.** 24
- **B.** 1
- **C.** 4
- **D.** 12

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (24)

**💡 Giải thích chi tiết:** Theo phương pháp băm phép chia (Division hashing): hash(key) = key % Table_Size = 124 % 100 = 24. Khóa 124 được lưu ở vị trí chỉ mục 24.

---

### Câu 202 (Slide 202)

**Câu hỏi:** Kizspy I Question: 43 (Choose 1 answer) Given a graph in the figure, the depth first traversal from node B is (visit nodes in ABC order):

**Các lựa chọn:**
- **A.** BADCE
- **B.** BAEDC B
- **C.** BCDEA
- **D.** BACDE -ORU c

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (BADCE)

**💡 Giải thích chi tiết:** Duyệt đồ thị theo chiều sâu (DFS) bắt đầu từ đỉnh B theo thứ tự bảng chữ cái ABC: từ B thăm đỉnh kề A đầu tiên, từ A thăm D, từ D thăm C, từ C thăm E -> Thứ tự duyệt là B -> A -> D -> C -> E (BADCE).

---

### Câu 203 (Slide 203)

**Câu hỏi:** To send sensor data to the Serial Monitor, you use: A Serial.write()

**Các lựa chọn:**
- **A.** Serial.write()
- **B.** Serial.print() or Serial.println()
- **C.** Send-toMonitor()
- **D.** console.log()

- **Đáp án trong ghi chú:** `AB`
- **Đáp án chính xác:** **A, B (hoặc B)** (A. Serial.write(); B. Serial.print() or Serial.println())

> ⚠️ LƯU Ý: Note trong slide ghi nhận cả "AB". Thông thường để đọc được dữ liệu dạng text trên màn hình Serial Monitor người ta dùng B (Serial.print/println), còn Serial.write gửi dữ liệu byte thô.

**💡 Giải thích chi tiết:** ⚠️ LƯU Ý: Để gửi dữ liệu lên Serial Monitor đọc được dưới dạng text, ta dùng Serial.print() hoặc Serial.println() (phương án B). Serial.write() gửi dạng byte thô (A). Note chấp nhận cả AB.

---

### Câu 204 (Slide 204)

**Câu hỏi:** What is the maximum input voltage limit for the Arduino Uno?

**Các lựa chọn:**
- **A.** 6-20V
- **B.** 7-15V
- **C.** 9-15V
- **D.** 5-12V

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (6-20V)

**💡 Giải thích chi tiết:** Phương án A ('6-20V') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 205 (Slide 205)

**Câu hỏi:** Which of the following are valid power input methods for an Arduino Uno boardO (Select all that apply)

**Các lựa chọn:**
- **A.** Mn pin
- **B.** Power jack
- **C.** PWM pin
- **D.** USB port

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (Mn pin)

**💡 Giải thích chi tiết:** Bo mạch Arduino Uno có thể được cấp nguồn qua 3 ngõ: 1) Cổng USB (5V); 2) Jack cắm nguồn DC tròn (7-12V); 3) Chân Vin (7-12V qua IC ổn áp tích hợp).

---

### Câu 206 (Slide 206)

**Câu hỏi:** Which of the following is an input device?

**Các lựa chọn:**
- **A.** LED light
- **B.** Light sensor
- **C.** Speaker
- **D.** DC motor

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (Light sensor)

**💡 Giải thích chi tiết:** Cảm biến ánh sáng (Light sensor) là một thiết bị đầu vào (Input device) thu thập thông tin quang học từ môi trường và chuyển thành tín hiệu điện cho vi điều khiển.

---

### Câu 207 (Slide 207)

**Câu hỏi:** What type of voltage is required to operate an LCD 16x2 display?

**Các lựa chọn:**
- **A.** 5V
- **B.** 3.3V
- **C.** 12V
- **D.** 9V

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (5V)

**💡 Giải thích chi tiết:** Module màn hình tinh thể lỏng LCD 16x2 tiêu chuẩn (dựa trên vi điều khiển HD44780) hoạt động với điện áp cung cấp chuẩn là 5V DC.

---

### Câu 208 (Slide 208)

**Câu hỏi:** How do you open the LED blink example sketch in the Arduino IDE? A File > New > Sketch

**Các lựa chọn:**
- **A.** File>New>Sketch
- **B.** File > Examples > I.Basics > Blink
- **C.** Tools > Upload > Blink
- **D.** Sketch > Compile > Examples > Blink

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (File > Examples > I.Basics > Blink)

**💡 Giải thích chi tiết:** Trong phần mềm Arduino IDE, để mở ví dụ mẫu chớp tắt đèn LED, người dùng truy cập theo đường dẫn menu: File > Examples > 01.Basics > Blink.

---

### Câu 209 (Slide 209)

**Câu hỏi:** Which symbol is used to start a comment in Arduino code?

**Các lựa chọn:**
- **A.** #
- **B.** //
- **C.** *
- **D.** <

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (//)

**💡 Giải thích chi tiết:** Trong mã nguồn Arduino C/C++, ký hiệu hai dấu gạch chéo // được dùng để bắt đầu một dòng chú thích đơn (single-line comment).

---

### Câu 210 (Slide 210)

**Câu hỏi:** What is the potential risk of a hacked IoT device being misused?

**Các lựa chọn:**
- **A.** Increased device efficiency
- **B.** Damage to other devices or operations
- **C.** Improved user expenence
- **D.** Reduced maintenance costs

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (Damage to other devices or operations)

**💡 Giải thích chi tiết:** Khi một thiết bị IoT bị tin tặc chiếm quyền điều khiển (hacked), nguy cơ nghiêm trọng nhất là nó bị lợi dụng làm bàn đạp (botnet) để tấn công hoặc gây hư hại cho các thiết bị và hệ thống vận hành khác trong mạng.

---

### Câu 211 (Slide 211)

**Câu hỏi:** How many pins does the LM35 Temperature Sensor Module have?

**Các lựa chọn:**
- **A.** 1
- **B.** 4
- **C.** 3
- **D.** 2

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (3)

**💡 Giải thích chi tiết:** Module cảm biến nhiệt độ LM35 tiêu chuẩn (đóng gói TO-92) có đúng 3 chân: chân 1 cấp nguồn VCC (+5V), chân 2 ngõ ra điện áp VOUT (10mV/°C), chân 3 nối đất GND.

---

### Câu 212 (Slide 212)

**Câu hỏi:** What is the main role of the Cloud in IoT smart grid architecture?

**Các lựa chọn:**
- **A.** Enhancing security
- **B.** Collecting data
- **C.** Managing data
- **D.** Storing data

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Managing data)

**💡 Giải thích chi tiết:** Trong kiến trúc lưới điện thông minh (Smart Grid), điện toán đám mây (Cloud) đóng vai trò trung tâm trong việc quản lý, tổng hợp và điều phối dữ liệu lớn (Managing data) từ hàng triệu đồng hồ đo điện thông minh.

---

### Câu 213 (Slide 213)

**Câu hỏi:** Which sensor in smartphones uses acoustic waves for detection? A Gyroscope

**Các lựa chọn:**
- **A.** Gyroscope
- **B.** Accelerometer
- **C.** Surface acoustic wave sensor
- **D.** Resistive touch sensor

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Surface acoustic wave sensor)

**💡 Giải thích chi tiết:** Cảm biến sóng âm bề mặt (Surface Acoustic Wave - SAW sensor) sử dụng sóng âm truyền lan trên bề mặt chất nền áp điện để phát hiện các biến đổi cơ học, áp suất hoặc tiếp xúc.

---

### Câu 214 (Slide 214)

**Câu hỏi:** What programming language is commonly used for programming IoT devices?

**Các lựa chọn:**
- **A.** C/C++
- **B.** Python
- **C.** Java
- **D.** JavaScript

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (C/C++)

**💡 Giải thích chi tiết:** Ngôn ngữ C/C++ là ngôn ngữ lập trình phổ biến nhất cho phần cứng thiết bị nhúng và IoT nhờ tốc độ thực thi cao, quản lý bộ nhớ trực tiếp và hỗ trợ thư viện phần cứng rộng rãi.

---

### Câu 215 (Slide 215)

**Câu hỏi:** What property is responsible for the flow of electrons, while the difference in electric charge between two points is referred to as voltage, and the ability to conduct electricity is termed resistance?

**Các lựa chọn:**
- **A.** Current
- **B.** Voltage
- **C.** Conductance
- **D.** Resistors

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (Current)

**💡 Giải thích chi tiết:** Dòng dịch chuyển có hướng của các electron mang điện tích trong dây dẫn được định nghĩa là Dòng điện (Electric Current, đo bằng Ampe - A).

---

### Câu 216 (Slide 216)

**Câu hỏi:** Which interface does the AS608 fingerprint sensor use? A CoAP interface

**Các lựa chọn:**
- **A.** CoAPinterface
- **B.** UART interface
- **C.** 12P interface
- **D.** SPI interface

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (UART interface)

**💡 Giải thích chi tiết:** Cảm biến vân tay quang học AS608 giao tiếp với vi điều khiển thông qua giao thức truyền thông nối tiếp bất đồng bộ UART (chân TX/RX).

---

### Câu 217 (Slide 217)

**Câu hỏi:** Which additional device is required to control a DC motor?

**Các lựa chọn:**
- **A.** WiFi module
- **B.** L298N motor driver
- **C.** Temperature sensor
- **D.** OLED display

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (L298N motor driver)

**💡 Giải thích chi tiết:** Phương án B ('L298N motor driver') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

## Phần 3: Câu hỏi Answer Dài (Long Concept & Application Questions)

### Câu 219 (Slide 219)

**Câu hỏi:** What is the purpose of 'Authentication' in a Secure IoT Framework?

**Các lựa chọn:**
- **A.** To establish a trust relationship by validating the identity of an IoT device connecting to the network
- **B.** To control all elements that route and transport endpoint traffic securely over the network.
- **C.** To determine what information an authenticated device can access and share.
- **D.** To provide threat detection and threat mitigation for aggregated information.

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (To establish a trust relationship by validating the identity of an IoT device connecting to the network)

**💡 Giải thích chi tiết:** Xác thực (Authentication) trong bảo mật IoT nhằm xác minh và chứng thực danh tính của thiết bị trước khi cho phép nó kết nối và trao đổi dữ liệu trong mạng.

---

### Câu 220 (Slide 220)

**Câu hỏi:** What is the DISADVANTAGE of segmentation in the memory management? A It can have extemal fragmentation.

**Các lựa chọn:**
- **A.** Itcanhaveextermalfragmentation.
- **B.** The average segment size is larger than the actual page size.
- **C.** It is easier to relocate segments than the entire address space.
- **D.** The segment table is smaller as compared to the page table.

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (Itcanhaveextermalfragmentation.)

**💡 Giải thích chi tiết:** Nhược điểm lớn nhất của kỹ thuật phân đoạn bộ nhớ (Segmentation) trong quản lý bộ nhớ của hệ điều hành là gây ra phân mảnh ngoại vi (External fragmentation).

---

### Câu 221 (Slide 221)

**Câu hỏi:** What is a mesh network in the context of IoT?

**Các lựa chọn:**
- **A.** A network topology where devices are interconnected with each other to relay data
- **B.** A network topology where devices are connected to a central hub
- **C.** A network topology where devices are connected in a linear fashion
- **D.** A network topology where devices are connected to multiple networks simultaneously

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (A network topology where devices are interconnected with each other to relay data)

**💡 Giải thích chi tiết:** Mạng lưới (Mesh network) trong IoT là kiến trúc mạng trong đó các thiết bị được liên kết đan xen với nhau để chuyển tiếp dữ liệu qua lại, giúp mở rộng tầm phủ sóng và tăng độ bền vững.

---

### Câu 222 (Slide 222)

**Câu hỏi:** What is the function of an actuator in an IoT system?

**Các lựa chọn:**
- **A.** To convert physical quantities into electrical signals
- **B.** To convert electrical signals into physical action
- **C.** To process data from sensors
- **D.** To encrypt communication

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (To convert electrical signals into physical action)

**💡 Giải thích chi tiết:** Cơ cấu chấp hành (Actuator) có chức năng chuyển đổi các tín hiệu điều khiển điện tử thành hành động vật lý cơ học (như quay động cơ, đóng rơ-le, phát âm thanh).

---

### Câu 223 (Slide 223)

**Câu hỏi:** What is a key consideration when choosing the hardware for an IoT device with limited power, memory, and computational resources?

**Các lựa chọn:**
- **A.** A high-resolution display for user interaction
- **B.** A high-performance processor for faster computations
- **C.** Energy-eficient components and minimal storage needs
- **D.** Compatibility with multiple third-party applications

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Energy-eficient components and minimal storage needs)

**💡 Giải thích chi tiết:** Khi chọn phần cứng cho thiết bị IoT có nguồn năng lượng và bộ nhớ hạn chế, ưu tiên hàng đầu là các linh kiện tiêu thụ điện cực thấp và nhu cầu lưu trữ tối thiểu.

---

### Câu 224 (Slide 224)

**Câu hỏi:** What is the function of serial communication in Arduino? A Send and receive data to/from external devices.

**Các lựa chọn:**
- **A.** Send andreceivedatato/fromexternaldevices.
- **B.** To provide power to extemal components
- **C.** To generate clock signals for timing operations.
- **D.** To connect the Arduino to Wi-Fi or Bluetooth.

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (Send andreceivedatato/fromexternaldevices.)

**💡 Giải thích chi tiết:** Giao tiếp nối tiếp (Serial communication) trên Arduino có chức năng truyền và nhận các luồng dữ liệu hai chiều với máy tính hoặc các vi điều khiển ngoại vi.

---

### Câu 225 (Slide 225)

**Câu hỏi:** What is PWM (Pulse Width Modulation) primarily used for in Arduino projects?

**Các lựa chọn:**
- **A.** To enhance digital signal strength
- **B.** To achieve analog-like results from digital outputs
- **C.** To increase the digital pin voltage
- **D.** To decrease the processing time for digital outputs

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (To achieve analog-like results from digital outputs)

**💡 Giải thích chi tiết:** Điều chế độ rộng xung (PWM) trên Arduino chủ yếu được sử dụng để mô phỏng tín hiệu tương tự (analog-like) từ các chân xuất tín hiệu số (digital output), ví dụ điều chỉnh độ sáng LED hoặc tốc độ động cơ.

---

### Câu 226 (Slide 226)

**Câu hỏi:** What is a Mock-up?

**Các lựa chọn:**
- **A.** It is a horizontal prototype.
- **B.** It is a particular approach to throwaway prototype
- **C.** It is a throwaway prototype.
- **D.** It is a nonreleasable prototype.

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (It is a horizontal prototype.)

**💡 Giải thích chi tiết:** Mock-up trong thiết kế phần mềm/hệ thống là một dạng nguyên mẫu nằm ngang (Horizontal prototype) mô phỏng giao diện người dùng trực quan mà chưa có logic nghiệp vụ xử lý đầy đủ bên dưới.

---

### Câu 227 (Slide 227)

**Câu hỏi:** What is the primary purpose of the Internet of Things (IOT)? A To connect only computers to the internet

**Các lựa chọn:**
- **A.** Toconnect onlycomputersto the internet
- **B.** To connect everyday physical objects to the internet
- **C.** To increase internet speed
- **D.** To allow humans to communicate directly with each other online

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (To connect everyday physical objects to the internet)

**💡 Giải thích chi tiết:** Mục đích cốt lõi của Internet of Things (IoT) là kết nối các đồ vật vật lý thông thường trong đời sống hàng ngày vào mạng Internet để thu thập và chia sẻ dữ liệu.

---

### Câu 228 (Slide 228)

**Câu hỏi:** What is one of the main impacts of IoT on urban areas?

**Các lựa chọn:**
- **A.** Creating smart cities with smart buildings and transportation.
- **B.** Improving public entertainment services.
- **C.** Reducing air pollution by enhancing public transportation.
- **D.** Enhancing cybersecurity for personal devices.

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (Creating smart cities with smart buildings and transportation.)

**💡 Giải thích chi tiết:** Tác động lớn nhất của IoT lên khu vực đô thị là xây dựng các thành phố thông minh (Smart cities) với các tòa nhà thông minh, hệ thống chiếu sáng và giao thông tự động hóa.

---

### Câu 229 (Slide 229)

**Câu hỏi:** What is each controller in memory-mapped 1/0 used for? A_ Perform any error correction necessary

**Các lựa chọn:**
- **A.** Perform anyerror correctionnecessary
- **B.** Communication with memory
- **C.** Communication with the CPU
- **D.** Perform read and write with 1/0 devices

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (Perform read and write with 1/0 devices)

**💡 Giải thích chi tiết:** Trong cơ chế I/O ánh xạ bộ nhớ (Memory-mapped I/O), mỗi bộ điều khiển thiết bị thực hiện thao tác đọc và ghi trực tiếp với các thiết bị vào/ra thông qua không gian địa chỉ bộ nhớ.

---

### Câu 230 (Slide 230)

**Câu hỏi:** What is MQTT primarily used for?

**Các lựa chọn:**
- **A.** System transfer
- **B.** Create connection
- **C.** User communication
- **D.** Machine to Machine Communication

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (Machine to Machine Communication)

**💡 Giải thích chi tiết:** Giao thức MQTT được thiết kế chuyên biệt và tối ưu nhất cho giao tiếp máy-với-máy (M2M - Machine to Machine Communication) trong các hệ thống IoT.

---

### Câu 231 (Slide 231)

**Câu hỏi:** What is a "Sketch" in Arduino terminology?

**Các lựa chọn:**
- **A.** A sketch is a program written for the board and shields
- **B.** A sketch is a blueprint for designing a circuit
- **C.** A sketch is a diagram of the microcontroller layout
- **D.** A sketch is an input data format for sensors

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (A sketch is a program written for the board and shields)

**💡 Giải thích chi tiết:** Trong thuật ngữ Arduino, một 'Sketch' chính là một chương trình phần mềm viết bằng ngôn ngữ Arduino C/C++ để nạp vào chạy trên bo mạch.

---

### Câu 232 (Slide 232)

**Câu hỏi:** What is electricity?

**Các lựa chọn:**
- **A.** A type of energy used only for lighting.
- **B.** A form of energy that can produce work.
- **C.** A form of energy only used in machines.
- **D.** None of the others

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (A form of energy that can produce work.)

**💡 Giải thích chi tiết:** Điện năng (Electricity) là một dạng năng lượng có khả năng sinh công (A form of energy that can produce work) để vận hành các thiết bị và máy móc.

---

### Câu 233 (Slide 233)

**Câu hỏi:** What is an interrupt in the context of Arduino UNO programming? A A function that stops the Arduino from running

**Các lựa chọn:**
- **A.** Afunction thatstopstheArduinofromrunning
- **B.** A signal that pauses the current process to execute a specific function
- **C.** An error in the code compilation
- **D.** A method to increase the processing speed

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (A signal that pauses the current process to execute a specific function)

**💡 Giải thích chi tiết:** Ngắt (Interrupt) trong lập trình vi điều khiển là một tín hiệu đặc biệt làm tạm dừng tiến trình chương trình đang chạy để nhảy sang thực thi ngay một hàm xử lý ngắt cụ thể (ISR), sau đó quay lại chạy tiếp.

---

### Câu 234 (Slide 234)

**Câu hỏi:** What is the difference between the INPUT and INPUT PULLUP arguments in the pinMode() function?

**Các lựa chọn:**
- **A.** They are both the same
- **B.** INPUT supports only analog voltages while INPUT PULLUP supports only digital voltage readings
- **C.** INPUT takes the default reading as 0 while INPUT_PULLUP takes default reading as 1023
- **D.** INPUT takes the default reading as 1023 while INPUT_PULLUP takes the default reading as 0

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (INPUT takes the default reading as 0 while INPUT_PULLUP takes default reading as 1023)

**💡 Giải thích chi tiết:** Chế độ INPUT đọc giá trị hở mạch thả nổi hoặc 0; trong khi chế độ INPUT_PULLUP kích hoạt điện trở kéo lên 5V bên trong vi điều khiển, làm cho trạng thái mặc định khi nút bấm chưa nhấn đọc về mức cao (HIGH/1023).

---

### Câu 235 (Slide 235)

**Câu hỏi:** What is the main purpose of routing in network communication?

**Các lựa chọn:**
- **A.** To encrypt data
- **B.** To select a path for traffic in a network
- **C.** To store data
- **D.** To create new data paths

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (To select a path for traffic in a network)

**💡 Giải thích chi tiết:** Mục đích chính của định tuyến (Routing) trong truyền thông mạng là tìm kiếm và lựa chọn đường đi tối ưu cho lưu lượng dữ liệu di chuyển trong mạng.

---

### Câu 236 (Slide 236)

**Câu hỏi:** What is the primary purpose of connecting shields to the 1/0 board in an embedded system? A To increase the weight of the 1/0 board.

**Các lựa chọn:**
- **A.** To increase theweightof theI/Oboard.
- **B.** To improve the 1/0 board's aesthetic appearance.
- **C.** To extend the functionality of the 1/0 board.
- **D.** To decrease the power consumption of the 1/0 board.

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (To extend the functionality of the 1/0 board.)

**💡 Giải thích chi tiết:** Arduino Shields là các bo mạch mở rộng cắm chồng lên Arduino nhằm mục đích mở rộng tính năng phần cứng (To extend the functionality of the I/O board) như kết nối Wi-Fi, Ethernet, điều khiển động cơ, hiển thị...

---

### Câu 237 (Slide 237)

**Câu hỏi:** What is the full form of GUI?

**Các lựa chọn:**
- **A.** Graphical User Interaction
- **B.** Graph User Interface
- **C.** Graphical User Interface
- **D.** Graph Using Interface

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Graphical User Interface)

**💡 Giải thích chi tiết:** GUI là viết tắt của Graphical User Interface (Giao diện người dùng đồ họa).

---

### Câu 238 (Slide 238)

**Câu hỏi:** What is the purpose of digital input/output programming in Arduino UNO?

**Các lựa chọn:**
- **A.** To process text data
- **B.** To control LEDs and buttons
- **C.** To enhance graphics processing
- **D.** To increase memory capacity

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (To control LEDs and buttons)

**💡 Giải thích chi tiết:** Phương án B ('To control LEDs and buttons') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 239 (Slide 239)

**Câu hỏi:** What is the purpose of Fritzing in the context of designing circuits?

**Các lựa chọn:**
- **A.** To physically build circuits in the real world.
- **B.** To simulate circuit behavior.
- **C.** To create circuit diagrams and layouts
- **D.** To test electronic components.

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (To create circuit diagrams and layouts)

**💡 Giải thích chi tiết:** Phần mềm Fritzing là công cụ thiết kế nguồn mở phổ biến giúp vẽ sơ đồ lắp ráp linh kiện trên breadboard, sơ đồ nguyên lý mạch điện (schematic) và thiết kế mạch in PCB.

---

### Câu 240 (Slide 240)

**Câu hỏi:** What is the purpose of the TRIG pin on the SRF05 ultrasonic sensor? A_ To receive the echo signal

**Các lựa chọn:**
- **A.** To receive the echosignal
- **B.** To send out ultrasound bursts
- **C.** To supply power to the sensor
- **D.** To process the incoming data

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (To send out ultrasound bursts)

**💡 Giải thích chi tiết:** Trên cảm biến siêu âm SRF05 (hoặc HC-SR04), chân TRIG (Trigger) có nhiệm vụ nhận xung kích hoạt 10µs từ Arduino để phát ra chùm sóng siêu âm 40kHz vào không gian.

---

### Câu 241 (Slide 241)

**Câu hỏi:** What is the primary function of a resistor in a circuit? A To amplify electncal signals

**Các lựa chọn:**
- **A.** To amplify electrical signals
- **B.** To store electrical energy
- **C.** To oppose the flow of electrical current
- **D.** To convert electrical energy into mechanical energy

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (To oppose the flow of electrical current)

**💡 Giải thích chi tiết:** Chức năng cơ bản nhất của điện trở trong mạch điện là cản trở và giới hạn dòng điện (To oppose the flow of electrical current) theo định luật Ohm.

---

### Câu 242 (Slide 242)

**Câu hỏi:** What is the primary function of the Ultrasonic Sensor in IoT applications?

**Các lựa chọn:**
- **A.** Measuring air pressure
- **B.** Detecting humidity levels
- **C.** Enabling image processing
- **D.** Proximity Detection

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (Proximity Detection)

**💡 Giải thích chi tiết:** Cảm biến siêu âm trong IoT chủ yếu dùng để phát hiện vật cản ở cự ly gần (Proximity Detection) và đo khoảng cách chính xác dựa trên thời gian bay của sóng âm (Time of Flight).

---

### Câu 243 (Slide 243)

**Câu hỏi:** What is the role of a gateway in an IoT network, and how does it relate to routing?

**Các lựa chọn:**
- **A.** Gateways are responsible for routing data packets within the local network.
- **B.** Gateways serve as a central control hub for all IoT devices
- **C.** Gateways connect IoT devices to the internet and perform protocol translation between IoT devices and the internet, aiding in data routing
- **D.** Routing is a term specific to IoT, and gateways are not involved in data transmission.

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Gateways connect IoT devices to the internet and perform protocol translation between IoT devices and the internet, aiding in data routing)

**💡 Giải thích chi tiết:** Cổng kết nối IoT Gateway đóng vai trò làm cầu nối giữa mạng cảm biến cục bộ và mạng Internet toàn cầu, thực hiện chuyển đổi giao thức (protocol translation) và hỗ trợ định tuyến dữ liệu.

---

### Câu 244 (Slide 244)

**Câu hỏi:** What is the function of the Domain Name System (DNS) in networking? A_ It routes the data packets to the destination.

**Các lựa chọn:**
- **A.** It routes the datapackets to thedestination.
- **B.** It is a large database of computer names and their internet addresses.
- **C.** It acts as the memory storage for the internet
- **D.** It is the main server for internet traffic.

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (It is a large database of computer names and their internet addresses.)

**💡 Giải thích chi tiết:** Hệ thống phân giải tên miền DNS (Domain Name System) hoạt động như một danh bạ khổng lồ trên Internet, chuyển đổi tên miền thân thiện (như google.com) thành địa chỉ IP số học.

---

### Câu 245 (Slide 245)

**Câu hỏi:** What is the function of a Digital to Analog Converter?

**Các lựa chọn:**
- **A.** to generate an analog voltage from digital signals
- **B.** to allow analog current to be controlled by a digital number
- **C.** to produce a waveform with an analog frequency
- **D.** to accept both digital and analog inputs

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (to generate an analog voltage from digital signals)

**💡 Giải thích chi tiết:** Bộ chuyển đổi số sang tương tự DAC (Digital-to-Analog Converter) có chức năng tạo ra điện áp tương tự liên tục từ các giá trị dữ liệu số nhị phân.

---

### Câu 246 (Slide 246)

**Câu hỏi:** What is the function of a photoresistor?

**Các lựa chọn:**
- **A.** It changes voltage according to light level
- **B.** It increases or decreases current through a wire
- **C.** It stores an image
- **D.** It changes resistance according to light level

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (It changes resistance according to light level)

**💡 Giải thích chi tiết:** Quang điện trở (Photoresistor / LDR) có đặc tính thay đổi trị số điện trở theo cường độ ánh sáng chiếu vào (khi trời sáng điện trở giảm, khi trời tối điện trở tăng).

---

### Câu 247 (Slide 247)

**Câu hỏi:** What is the function of a schematic diagram in electronics?

**Các lựa chọn:**
- **A.** To provide a realistic representation of the physical arrangement of components
- **B.** To show the components and interconnections in a circuit using symbolic representations
- **C.** To detail the manufacturing process of electronic devices
- **D.** To list all the components needed in a circuit

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (To show the components and interconnections in a circuit using symbolic representations)

**💡 Giải thích chi tiết:** Sơ đồ nguyên lý (Schematic diagram) sử dụng các ký hiệu đồ họa quy ước tiêu chuẩn để biểu diễn các linh kiện điện tử và mối liên kết dây dẫn giữa chúng trong mạch điện.

---

### Câu 248 (Slide 248)

**Câu hỏi:** What is the potential risk of a hacked IoT device being misused?

**Các lựa chọn:**
- **A.** Increased device efficiency
- **B.** Damage to other devices or operations
- **C.** Improved user experience
- **D.** Reduced maintenance costs

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (Damage to other devices or operations)

**💡 Giải thích chi tiết:** Khi một thiết bị IoT bị tin tặc chiếm quyền điều khiển (hacked), nguy cơ nghiêm trọng nhất là nó bị lợi dụng làm bàn đạp (botnet) để tấn công hoặc gây hư hại cho các thiết bị và hệ thống vận hành khác trong mạng.

---

### Câu 249 (Slide 249)

**Câu hỏi:** What is a critical consideration when programming analog input/output for IoT applications?

**Các lựa chọn:**
- **A.** The color depth of the display
- **B.** The refresh rate of the display
- **C.** The precision of the sensor data
- **D.** The size of the code

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (The precision of the sensor data)

**💡 Giải thích chi tiết:** Phương án C ('The precision of the sensor data') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 250 (Slide 250)

**Câu hỏi:** What is the full form of IDE in Arduino IDE software?

**Các lựa chọn:**
- **A.** Intra Defense Environment
- **B.** Intra Development Environment
- **C.** Integrated Development Environment
- **D.** Integrated Deployed Environment

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Integrated Development Environment)

**💡 Giải thích chi tiết:** IDE là viết tắt của Integrated Development Environment (Môi trường phát triển tích hợp), cung cấp trình soạn thảo mã nguồn, trình biên dịch và công cụ nạp code.

---

### Câu 251 (Slide 251)

**Câu hỏi:** What is the full form of DHCP in IoT network management protocol?

**Các lựa chọn:**
- **A.** Dynamic Host Configuration Protocol
- **B.** Domain Host Communication Protocol
- **C.** Dynamic Host Control Protocol
- **D.** Domain Host Control Protocol

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (Dynamic Host Configuration Protocol)

**💡 Giải thích chi tiết:** DHCP là viết tắt của Dynamic Host Configuration Protocol (Giao thức cấu hình máy chủ động), tự động cấp phát địa chỉ IP và thông số mạng cho các thiết bị khi kết nối vào mạng.

---

### Câu 252 (Slide 252)

**Câu hỏi:** What is a critical consideration when programming analog input/output for IoT applications?

**Các lựa chọn:**
- **A.** The color depth of the display
- **B.** The refresh rate of the display
- **C.** The precision of the sensor data
- **D.** The size of the code

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (The precision of the sensor data)

**💡 Giải thích chi tiết:** Phương án C ('The precision of the sensor data') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 253 (Slide 253)

**Câu hỏi:** What is the significance of programming sensors/actuators in IoT projects?

**Các lựa chọn:**
- **A.** To display information
- **B.** To interact with the physical world
- **C.** To improve battery life
- **D.** To enhance audio quality

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (To interact with the physical world)

**💡 Giải thích chi tiết:** Phương án B ('To interact with the physical world') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 254 (Slide 254)

**Câu hỏi:** What is the correct guideline when implementing adding a library through the Arduino IDE?

**Các lựa chọn:**
- **A.** Select Sketch -> Manage Libraries, search for the required library and install
- **B.** Select Include Library Manage Libraries, search for the library name and install
- **C.** Select Sketch Include Library Manage Libraries, search for the library name and install
- **D.** Select Sketch Manage Libraries, search for the library name and install

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Select Sketch Include Library Manage Libraries, search for the library name and install)

**💡 Giải thích chi tiết:** Để cài đặt thư viện mới trong Arduino IDE, ta chọn menu: Sketch > Include Library > Manage Libraries..., sau đó tìm kiếm tên thư viện và nhấn nút Install.

---

### Câu 255 (Slide 255)

**Câu hỏi:** What is the difference between an IDE and a compiler?

**Các lựa chọn:**
- **A.** The compiler executes the code while the IDE gives a graphical environment for writing the code
- **B.** The compiler links the code to the respective files and the IDE takes it from there
- **C.** The compiler and the IDE are the same thing
- **D.** The IDE executes the code while the compiler gives a graphical environment for writing the code

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (The compiler executes the code while the IDE gives a graphical environment for writing the code)

**💡 Giải thích chi tiết:** Trình biên dịch (Compiler) có nhiệm vụ dịch mã nguồn cấp cao thành mã máy nhị phân mà vi điều khiển thực thi được; trong khi IDE cung cấp môi trường đồ họa hỗ trợ lập trình viên viết và quản lý code.

---

### Câu 256 (Slide 256)

**Câu hỏi:** What is the fundamental process that leads to electricity when considering the structure of atoms? A The movement of protons within the nucleus

**Các lựa chọn:**
- **A.** Themovementofprotonswithinthenucleus
- **B.** The exchange of neutrons between atoms
- **C.** The interaction between electrons and protons
- **D.** The jumping of negatively charged electrons between atoms

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (The jumping of negatively charged electrons between atoms)

**💡 Giải thích chi tiết:** Bản chất của dòng điện trong kim loại ở cấp độ nguyên tử là sự dịch chuyển và nhảy có hướng của các electron mang điện tích âm tự do giữa các nguyên tử.

---

### Câu 257 (Slide 257)

**Câu hỏi:** What is the use of the Interrupt Service Routine in an Arduino?

**Các lựa chọn:**
- **A.** To boot up the Arduino
- **B.** To exit any code that is running
- **C.** To automate functions
- **D.** To make more memory

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (To automate functions)

**💡 Giải thích chi tiết:** Hàm xử lý ngắt ISR (Interrupt Service Routine) được vi điều khiển tự động gọi ngay lập tức khi xảy ra sự kiện ngắt phần cứng, giúp tự động hóa và đáp ứng tức thì với các sự kiện bên ngoài mà không cần thăm dò liên tục.

---

### Câu 258 (Slide 258)

**Câu hỏi:** What is the key benefit of using the Wi-Fi shield for Arduino? A It allows Arduino to operate wirelessly without needing a network connection

**Các lựa chọn:**
- **A.** It allowsArduinoto operatewirelesslywithout needing a networkconnection
- **B.** It provides high-speed internet connectivity over Wi-Fi
- **C.** It supports mesh networking for long-distance communication
- **D.** It provides Bluetooth connectivity

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (It provides high-speed internet connectivity over Wi-Fi)

**💡 Giải thích chi tiết:** Wi-Fi Shield bổ sung khả năng kết nối mạng không dây tốc độ cao chuẩn 802.11 b/g/n cho Arduino, cho phép bo mạch kết nối Internet và truyền dữ liệu qua giao thức TCP/IP.

---

### Câu 259 (Slide 259)

**Câu hỏi:** What is the primary advantage of using EEPROM memory in an Arduino project?

**Các lựa chọn:**
- **A.** EEPROM memory is faster than SRAM
- **B.** EEPROM memory retains its data even when the power is turned off.
- **C.** EEPROM memory has unlimited write cycles.
- **D.** EEPROM memory is less expensive than flash memory.

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (EEPROM memory retains its data even when the power is turned off.)

**💡 Giải thích chi tiết:** Ưu điểm lớn nhất của bộ nhớ EEPROM (Electrically Erasable Programmable Read-Only Memory) là bộ nhớ bất biến (non-volatile), dữ liệu vẫn được lưu trữ nguyên vẹn ngay cả khi ngắt toàn bộ nguồn điện.

---

### Câu 260 (Slide 260)

**Câu hỏi:** What is the correct syntax to output a string like: "l like IoT" in C program?

**Các lựa chọn:**
- **A.** System.out.println("l like IoT");
- **B.** Console.writeLine("l like IoT");
- **C.** System.output("l like IOT");
- **D.** Printf("l like loT");

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (Printf("l like loT");)

**💡 Giải thích chi tiết:** Phương án D ('Printf("l like loT");') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 261 (Slide 261)

**Câu hỏi:** What is the use of the Mn pin present on some Arduino Boards?

**Các lựa chọn:**
- **A.** To ground the Arduino board
- **B.** To power the Arduino board
- **C.** To provide a 5V output
- **D.** Is used for plugging in 3V supply

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (To power the Arduino board)

**💡 Giải thích chi tiết:** Chân Vin trên Arduino Uno (đôi khi bị OCR nhận dạng nhầm thành Mn) được dùng để cấp nguồn ngoài (7V - 12V) trực tiếp cho bo mạch thông qua bộ ổn áp tích hợp.

---

### Câu 262 (Slide 262)

**Câu hỏi:** What is the use of PWM signals in IoT development boards?

**Các lựa chọn:**
- **A.** They are used by sensors to have analog input
- **B.** They are used by sensors to have digital input
- **C.** They are used by actuators to have analog input
- **D.** They are used by actuators to have digital input

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (They are used by actuators to have analog input)

**💡 Giải thích chi tiết:** Phương án C ('They are used by actuators to have analog input') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 263 (Slide 263)

**Câu hỏi:** What is the use of the Interrupt Service Routine in an Arduino?

**Các lựa chọn:**
- **A.** To boot up the Arduino
- **B.** To exit any code that is running
- **C.** To automate functions
- **D.** To make more memory

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (To automate functions)

**💡 Giải thích chi tiết:** Hàm xử lý ngắt ISR (Interrupt Service Routine) được vi điều khiển tự động gọi ngay lập tức khi xảy ra sự kiện ngắt phần cứng, giúp tự động hóa và đáp ứng tức thì với các sự kiện bên ngoài mà không cần thăm dò liên tục.

---

### Câu 264 (Slide 264)

**Câu hỏi:** What is each controller in memory-mapped 1/0 used for?

**Các lựa chọn:**
- **A.** Perform any error correction necessary
- **B.** Communication with memory
- **C.** Communication with the CPU
- **D.** Perform read and write with 1/0 devices

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (Perform read and write with 1/0 devices)

**💡 Giải thích chi tiết:** Phương án D ('Perform read and write with 1/0 devices') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 265 (Slide 265)

**Câu hỏi:** What is the significance of programming sensors/actuators in IoT projects? A To display information

**Các lựa chọn:**
- **A.** To display information
- **B.** To interact with the physical world
- **C.** To improve battery life
- **D.** To enhance audio quality

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (To interact with the physical world)

**💡 Giải thích chi tiết:** Phương án B ('To interact with the physical world') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 266 (Slide 266)

**Câu hỏi:** What are the key components in ensuring the security of IoT networks and devices?

**Các lựa chọn:**
- **A.** Data encryption, hardware configuration, and network optimization
- **B.** Authentication, authorization, network enforced policy, and secure analytics
- **C.** Biometrics, X. 509 digital certificates, and endpoint MAC addresses
- **D.** Data monitoring, cloud integration, and device management

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (Authentication, authorization, network enforced policy, and secure analytics)

**💡 Giải thích chi tiết:** Phương án B ('Authentication, authorization, network enforced policy, and secure analytics') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 267 (Slide 267)

**Câu hỏi:** What are the four V's of big data defined by the IBM?

**Các lựa chọn:**
- **A.** Volume, Velocity, Variety, and Veracity
- **B.** Vendor, Variety, and Volume
- **C.** Vocation, Veracity, Venture, and Variety
- **D.** Venture, Volume, Variety, and Velocity

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (Volume, Velocity, Variety, and Veracity)

**💡 Giải thích chi tiết:** Theo định nghĩa của tập đoàn IBM, 4 chữ V đặc trưng của Dữ liệu lớn (Big Data) gồm: Volume (Khối lượng), Velocity (Tốc độ sinh dữ liệu), Variety (Sự đa dạng của định dạng), và Veracity (Độ tin cậy/tính xác thực).

---

### Câu 268 (Slide 268)

**Câu hỏi:** What are the 4 V's of Big Data, as described by IBM?

**Các lựa chọn:**
- **A.** Volume, Velocity, Value, Variability.
- **B.** Velocity, Versatility, Verification, Viscosity.
- **C.** Volume, Velocity, Variety, Veracity.
- **D.** Volatility, Vibration, Visualization, Viability.

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Volume, Velocity, Variety, Veracity.)

**💡 Giải thích chi tiết:** Theo định nghĩa của tập đoàn IBM, 4 chữ V đặc trưng của Dữ liệu lớn (Big Data) gồm: Volume (Khối lượng), Velocity (Tốc độ sinh dữ liệu), Variety (Sự đa dạng của định dạng), và Veracity (Độ tin cậy/tính xác thực).

---

### Câu 269 (Slide 269)

**Câu hỏi:** What are the two main functions of a program in Arduino IDE?

**Các lựa chọn:**
- **A.** build() and loop()
- **B.** setup() and build()
- **C.** setup() and loop()
- **D.** build() and setup()

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (setup() and loop())

**💡 Giải thích chi tiết:** Phương án C ('setup() and loop() D build() and setup()') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 270 (Slide 270)

**Câu hỏi:** What are properties of a tree

**Các lựa chọn:**
- **A.** One node is marked as Root node
- **B.** Every node other than the root is associated with one parent node
- **C.** Each node can have an arbitary number of child node
- **D.** All of the others

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (All of the others)

**💡 Giải thích chi tiết:** Phương án D ('All of the others') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 271 (Slide 271)

**Câu hỏi:** What does the analogRead() function do physically when invoked in a code?

**Các lựa chọn:**
- **A.** It accepts a digital input
- **B.** It reads the raw voltage value
- **C.** It activates the ADC Circuit to read voltage values
- **D.** It activates the DAC Circuit to read voltage values

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (It activates the ADC Circuit to read voltage values)

**💡 Giải thích chi tiết:** Phương án C ('It activates the ADC Circuit to read voltage values') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 272 (Slide 272)

**Câu hỏi:** What does interoperability in IoT refer to?

**Các lựa chọn:**
- **A.** Efficient storage, processing, and analysis of IoT data
- **B.** Seamless communication between different IoT devices
- **C.** Responsible data collection and privacy protection
- **D.** Ensuring user data remains confidential and secure

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (Seamless communication between different IoT devices)

**💡 Giải thích chi tiết:** Phương án B ('Seamless communication between different IoT devices') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 273 (Slide 273)

**Câu hỏi:** What does the RX LED blinking on an Arduino board signify? A The Arduino is receiving data from a connected device.

**Các lựa chọn:**
- **A.** TheArduino is receiving data from a connected device.
- **B.** The Arduino is sending data to a connected device.
- **C.** The Arduino is in programming mode.
- **D.** The Arduino is disconnected from the serial monitorR U

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (TheArduino is receiving data from a connected device.)

**💡 Giải thích chi tiết:** Phương án A ('TheArduino is receiving data from a connected device.') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 274 (Slide 274)

**Câu hỏi:** What does MAC stand for? A Media Area Control

**Các lựa chọn:**
- **A.** MediaAreaControl
- **B.** Memory Access Control
- **C.** Media Access Control
- **D.** Memory Access Control

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Media Access Control)

**💡 Giải thích chi tiết:** Phương án C ('Media Access Control') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 275 (Slide 275)

**Câu hỏi:** What does the RX LED on an Arduino board indicate?

**Các lựa chọn:**
- **A.** The Arduino is transmitting data
- **B.** The Arduino is receiving data
- **C.** The Arduino is powered on
- **D.** The Arduino is in programming mode

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (The Arduino is receiving data)

**💡 Giải thích chi tiết:** Phương án B ('The Arduino is receiving data') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 276 (Slide 276)

**Câu hỏi:** What does the analogRead() function do physically when invoked in a code?

**Các lựa chọn:**
- **A.** It accepts a digital input
- **B.** It reads the raw voltage value
- **C.** It activates the ADC Circuit to read voltage values
- **D.** It activates the DAC Circuit to read voltage values

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (It activates the ADC Circuit to read voltage values)

**💡 Giải thích chi tiết:** Phương án C ('It activates the ADC Circuit to read voltage values') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 277 (Slide 277)

**Câu hỏi:** What does interoperability in IoT refer to? A Efficient storage, processing, and analysis of IoT data

**Các lựa chọn:**
- **A.** Efficient storage, processing,and analysis of loT data
- **B.** Seamless communication between different IoT devices
- **C.** Responsible data collection and privacy protection
- **D.** Ensuring user data remains confidential and secure

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (Seamless communication between different IoT devices)

**💡 Giải thích chi tiết:** Phương án B ('Seamless communication between different IoT devices') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 278 (Slide 278)

**Câu hỏi:** What programming strategies could be employed to handle the "velocity" aspect of big data in an IoT system? A Implementing strict data type casting in all functions

**Các lựa chọn:**
- **A.** Implementing strict data type castingin all functions
- **B.** Utilizing just-in-time compilation for all code
- **C.** Employing data streaming and real-time processing frameworks
- **D.** Using older data protocols to ensure compatibility

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Employing data streaming and real-time processing frameworks)

**💡 Giải thích chi tiết:** Phương án C ('Employing data streaming and real-time processing frameworks') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 279 (Slide 279)

**Câu hỏi:** What type of signal does the analogWrite() function output?

**Các lựa chọn:**
- **A.** Pulse Code Modulated Signal
- **B.** Frequency Modulated Signal
- **C.** Pulse Width Modulated Signal
- **D.** Pulse Amplitude Modulated Signal

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Pulse Width Modulated Signal)

**💡 Giải thích chi tiết:** Phương án C ('Pulse Width Modulated Signal') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 280 (Slide 280)

**Câu hỏi:** What types of programming languages are commonly used for IoT systems?

**Các lựa chọn:**
- **A.** JavaScript, HTML, and CSS
- **B.** Python, C++, Java, Arduino, and Raspberry Pi platforms
- **C.** PHP and SQL
- **D.** Assembly language only

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (Python, C++, Java, Arduino, and Raspberry Pi platforms)

**💡 Giải thích chi tiết:** Ngôn ngữ C/C++ là ngôn ngữ lập trình phổ biến nhất cho phần cứng thiết bị nhúng và IoT nhờ tốc độ thực thi cao, quản lý bộ nhớ trực tiếp và hỗ trợ thư viện phần cứng rộng rãi.

---

### Câu 281 (Slide 281)

**Câu hỏi:** What types of programming languages are commonly used for IoT systems?

**Các lựa chọn:**
- **A.** JavaScript, HTML, and CSS
- **B.** Python, C++, Java, Arduino, and Raspberry Pi platforms
- **C.** PHP and SQL
- **D.** Assembly language only

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (Python, C++, Java, Arduino, and Raspberry Pi platforms)

**💡 Giải thích chi tiết:** Ngôn ngữ C/C++ là ngôn ngữ lập trình phổ biến nhất cho phần cứng thiết bị nhúng và IoT nhờ tốc độ thực thi cao, quản lý bộ nhớ trực tiếp và hỗ trợ thư viện phần cứng rộng rãi.

---

### Câu 282 (Slide 282)

**Câu hỏi:** What two key pieces of information should you have a clear idea of when planning an IoT project?

**Các lựa chọn:**
- **A.** The marketing strategy and the products brand name.
- **B.** The target audience and their requirements.
- **C.** The specific programming languages and hardware components you will use.
- **D.** The project's budget and timeline.

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (The target audience and their requirements.)

**💡 Giải thích chi tiết:** Phương án B ('The target audience and their requirements.') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 283 (Slide 283)

**Câu hỏi:** What factors should be considered when selecting a communication medium in a network?

**Các lựa chọn:**
- **A.** The distance a signal needs to travel
- **B.** The environment the signal will travel in
- **C.** The amount and speed of data
- **D.** All of the others

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (All of the others)

**💡 Giải thích chi tiết:** Phương án D ('All of the others') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 284 (Slide 284)

**Câu hỏi:** Which function to retrieve text sent from the computer?

**Các lựa chọn:**
- **A.** Serial.readStringUntil("\n')
- **B.** ReadStringUntil('\n')
- **C.** Serial.readingStringUntil('\n')

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (Serial.readStringUntil("\n'))

**💡 Giải thích chi tiết:** Phương án A ('Serial.readStringUntil("\n')') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 285 (Slide 285)

**Câu hỏi:** Which of the following is an example of an IoT application?

**Các lựa chọn:**
- **A.** Wearable device to monitor blood glucose level
- **B.** Manufacturing Bolt using CNC machine
- **C.** Bank web page to monitor customer experience

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (Wearable device to monitor blood glucose level)

**💡 Giải thích chi tiết:** Phương án A ('Wearable device to monitor blood glucose level') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 286 (Slide 286)

**Câu hỏi:** Which of the following IoT deployment models involves direct communication between nearby devices without relying on a centralized infrastructure?

**Các lựa chọn:**
- **A.** Cloud based IoT
- **B.** Peer-to-peer loT
- **C.** Hybrid IoT
- **D.** Edge computing IoT

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (Peer-to-peer loT)

**💡 Giải thích chi tiết:** Phương án B ('Peer-to-peer loT') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 287 (Slide 287)

**Câu hỏi:** Which of the following is a challenge that arises when manipulating big data for analysis?

**Các lựa chọn:**
- **A.** The difficulty in storing data
- **B.** Ensuring data accuracy and consistency
- **C.** The lack of data collection sources
- **D.** The absence of tools for manipulating the data

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (Ensuring data accuracy and consistency)

**💡 Giải thích chi tiết:** Phương án B ('Ensuring data accuracy and consistency') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 288 (Slide 288)

**Câu hỏi:** Which of the following is an example of a fog computing concept in IoT?

**Các lựa chọn:**
- **A.** Storing data on remote servers
- **B.** Routing data through multiple gateways
- **C.** Performing data analytics on edge devices
- **D.** Using blockchain technology for secure transactions

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Performing data analytics on edge devices)

**💡 Giải thích chi tiết:** Phương án C ('Performing data analytics on edge devices') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 289 (Slide 289)

**Câu hỏi:** Which of the following is an example of a method used for authenticating IoT devices?

**Các lựa chọn:**
- **A.** RFID (Radio Frequency Identification)
- **B.** Device power consumption monitoring
- **C.** Device software version tracking
- **D.** Physical device location tracking

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (RFID (Radio Frequency Identification))

**💡 Giải thích chi tiết:** Phương án A ('RFID (Radio Frequency Identification)') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 290 (Slide 290)

**Câu hỏi:** Which of the following best describes the role of sensors in the context of IoT?

**Các lựa chọn:**
- **A.** Sensors are used to create data signatures for various devices.
- **B.** Sensors collect and transmit data about the physical environment.
- **C.** Sensors generate power for IoT devices.
- **D.** Sensors are responsible for controlling mechanical movements.

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (Sensors collect and transmit data about the physical environment.)

**💡 Giải thích chi tiết:** Phương án B ('Sensors collect and transmit data about the physical environment.') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 291 (Slide 291)

**Câu hỏi:** Which of the following is a fundamental benefit of integrating IoT devices with cloud platforms?

**Các lựa chọn:**
- **A.** Reduced power consumption of IoT devices
- **B.** Enhanced local processing capabilities of IoT devices
- **C.** Scalable data storage and processing
- **D.** Elimination of network connectivity requirements

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Scalable data storage and processing)

**💡 Giải thích chi tiết:** Phương án C ('Scalable data storage and processing') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 292 (Slide 292)

**Câu hỏi:** Which of the following IoT deployment models involves direct communication between nearby devices without relying on a centralized infrastructure?

**Các lựa chọn:**
- **A.** Cloud based IoT
- **B.** Peer-to-peer IoT
- **C.** Hybrid IoT
- **D.** Edge computing IoT

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (Peer-to-peer IoT)

**💡 Giải thích chi tiết:** Phương án B ('Peer-to-peer IoT') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 293 (Slide 293)

**Câu hỏi:** Which of the following best describes 'Veracity'?

**Các lựa chọn:**
- **A.** The quantity of data that is being observed and tracked without sampling.
- **B.** The speed at which big data is available
- **C.** The extraction of data from multiple sources like text, images, and video.
- **D.** The quality of the data, and whether it stays true or is lost or damaged -U 1-(1

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (The quality of the data, and whether it stays true or is lost or damaged -U 1-(1)

**💡 Giải thích chi tiết:** Phương án D ('The quality of the data, and whether it stays true or is lost or damaged -U 1-(1') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 294 (Slide 294)

**Câu hỏi:** Which type of input pins does the Arduino Uno have? A Digital pins only

**Các lựa chọn:**
- **A.** Digital pins only
- **B.** Digital and Analog input pins
- **C.** PWM pins only
- **D.** UART and SPI pins

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (Digital and Analog input pins)

**💡 Giải thích chi tiết:** Phương án B ('Digital and Analog input pins') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 295 (Slide 295)

**Câu hỏi:** When integrating IoT devices with cloud platforms, what is the main programming challenge related to data flow?

**Các lựa chọn:**
- **A.** Minimizing the physical size of data packets
- **B.** Ensuring real-time data synchronization across devices
- **C.** Prioritizing graphical data over textual data
- **D.** Creating aesthetically pleasing data visualizations

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (Ensuring real-time data synchronization across devices)

**💡 Giải thích chi tiết:** Phương án B ('Ensuring real-time data synchronization across devices') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 296 (Slide 296)

**Câu hỏi:** When does electricity occur?

**Các lựa chọn:**
- **A.** The negatively charged electrons jump between atoms.
- **B.** The positively charged protons jump from one atom to another.
- **C.** The neutral neutrons jump between atoms
- **D.** The positively charged protons and negatively charged electrons cancel each other out.

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (The negatively charged electrons jump between atoms.)

**💡 Giải thích chi tiết:** Phương án A ('The negatively charged electrons jump between atoms.') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 297 (Slide 297)

**Câu hỏi:** When using the LCD 1602 display with an Arduino, what is the purpose of wiring a 10k ohm potentiometer to the VO pin of the LCD?

**Các lựa chọn:**
- **A.** To adjust the display contrast
- **B.** To provide power to the LCD
- **C.** To set the refresh rate of the display
- **D.** To enable the autoscroll feature

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (To adjust the display contrast)

**💡 Giải thích chi tiết:** Phương án A ('To adjust the display contrast') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 298 (Slide 298)

**Câu hỏi:** Why is the motion sensor in the responder important on a dairy farm? A It tracks the cows milk yield

**Các lựa chọn:**
- **A.** It tracksthecow'smilkyield
- **B.** It monitors the cow's movements, potentially detecting health issues
- **C.** It tracks the cow's location to ensure it stays in a designated area
- **D.** It measures the temperature of the milk being produced

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (It monitors the cow's movements, potentially detecting health issues)

**💡 Giải thích chi tiết:** Trong ứng dụng IoT chăn nuôi thông minh (Smart Dairy Farming), các thiết bị cảm biến responder gắn trên cổ hoặc tai bò dùng để theo dõi sức khỏe, hành vi vận động và phát hiện sớm dịch bệnh của đàn bò (To monitor the health and movement of the cows).

---

### Câu 299 (Slide 299)

**Câu hỏi:** Why do you use a breadboard?

**Các lựa chọn:**
- **A.** It's an inexpensive way to check the design and function of your circuit.
- **B.** It can be used to mass produce lots of identical circuits easily and cost effectively.
- **C.** The plug board versions are extremely reliable and will last for years, you might never need to do anything else.
- **D.** Breadboards aren't used any more. It's an old technology that is not needed with modern circuits.

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (It's an inexpensive way to check the design and function of your circuit.)

**💡 Giải thích chi tiết:** Phương án A ('It's an inexpensive way to check the design and function of your circuit.') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 300 (Slide 300)

**Câu hỏi:** Why is it essential to focus on the unique value proposition of an IoT product in the early planning stages of development and commercialization?

**Các lựa chọn:**
- **A.** It helps reduce the cost of production.
- **B.** It allows for more efficient product distribution.
- **C.** Differentiation from competitors is crucial for success.
- **D.** It ensures compatibility with all existing IoT devices

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Differentiation from competitors is crucial for success.)

**💡 Giải thích chi tiết:** Phương án C ('Differentiation from competitors is crucial for success. D It ensures compatibility with all existing IoT devices') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 301 (Slide 301)

**Câu hỏi:** Why is security a major concem in the context of the Internet of Things (loT)?

**Các lựa chọn:**
- **A.** Because IoT devices are not capable of transmitting data
- **B.** Because IoT introduces many new entry points for hackers to access data
- **C.** Because IoT does not transmit data in real-time
- **D.** Because IoT devices are always offline

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (Because IoT introduces many new entry points for hackers to access data)

**💡 Giải thích chi tiết:** Phương án B ('Because IoT introduces many new entry points for hackers to access data') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 302 (Slide 302)

**Câu hỏi:** Why might having 20 billion connected devices cause a major disruption in employment?

**Các lựa chọn:**
- **A.** Automation may replace jobs traditionally done by humans
- **B.** New job sectors will be created, making previous roles obsolete
- **C.** There will be fewer jobs available due to more devices doing the work
- **D.** Workers will need to learn new internet communication tools

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (Automation may replace jobs traditionally done by humans)

**💡 Giải thích chi tiết:** Hàm xử lý ngắt ISR (Interrupt Service Routine) được vi điều khiển tự động gọi ngay lập tức khi xảy ra sự kiện ngắt phần cứng, giúp tự động hóa và đáp ứng tức thì với các sự kiện bên ngoài mà không cần thăm dò liên tục.

---

### Câu 303 (Slide 303)

**Câu hỏi:** Why is it important to consider limited power supply when programming IoT devices?

**Các lựa chọn:**
- **A.** It affects the device's physical size
- **B.** It determines the maximum number of devices in a network
- **C.** Devices need to operate efficiently on minimal power for long durations
- **D.** It limits the types of sensors that can be used

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Devices need to operate efficiently on minimal power for long durations)

**💡 Giải thích chi tiết:** Phương án C ('Devices need to operate efficiently on minimal power for long durations') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 304 (Slide 304)

**Câu hỏi:** How does the veracity of big data impact IoT applications?

**Các lựa chọn:**
- **A.** By increasing the data transmission range
- **B.** By improving the energy efficiency of devices
- **C.** By ensuring the reliability and accuracy of the data used for decision-making
- **D.** By decreasing the cost of data storage

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (By ensuring the reliability and accuracy of the data used for decision-making)

**💡 Giải thích chi tiết:** Phương án C ('By ensuring the reliability and accuracy of the data used for decision-making') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 305 (Slide 305)

**Câu hỏi:** How do standards and protocols help communication between machines?

**Các lựa chọn:**
- **A.** By defining the TCP/IP model as the most common networking protocol suite.
- **B.** By creating an accepted set of rules for a procedure, which only applies to machine communication.
- **C.** By minimizing miscommunication and ensuring that messages can get through.
- **D.** By goveming the connection of computer systems to the Internet.

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (By minimizing miscommunication and ensuring that messages can get through.)

**💡 Giải thích chi tiết:** Phương án C ('By minimizing miscommunication and ensuring that messages can get through.') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 306 (Slide 306)

**Câu hỏi:** How can IoT systems address the issue of data privacy in the cloud?

**Các lựa chọn:**
- **A.** By restricting device access to the cloud
- **B.** By ensuring all data is publicly accessible
- **C.** By preventing misuse of private data
- **D.** By increasing the data storage capacity in the cloud

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (By preventing misuse of private data)

**💡 Giải thích chi tiết:** Phương án C ('By preventing misuse of private data') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 307 (Slide 307)

**Câu hỏi:** How can you create a network of IoT devices that efficiently exchange data?

**Các lựa chọn:**
- **A.** By using a single protocol for all devices
- **B.** By connecting all devices directly to the internet
- **C.** By designing a mesh network topology
- **D.** By using the highest data rate possible

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (By designing a mesh network topology)

**💡 Giải thích chi tiết:** Phương án C ('By designing a mesh network topology') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 308 (Slide 308)

**Câu hỏi:** How is the distance to an object calculated using the ultrasonic sensor?

**Các lựa chọn:**
- **A.** By measuring the intensity of the returned pulse
- **B.** By calculating the time it takes for a pulse to return
- **C.** By detecting the angle of the returned pulse
- **D.** By the frequency shift of the returned pulse

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (By calculating the time it takes for a pulse to return)

**💡 Giải thích chi tiết:** Phương án B ('By calculating the time it takes for a pulse to return') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 309 (Slide 309)

**Câu hỏi:** How might the evolving nature of the internet, where it's no longer just a means of communication, but also connects various devices like refrigerators, impact various aspects of our society?

**Các lựa chọn:**
- **A.** It will simplify security measures and reduce the need for big data analysis.
- **B.** It will have no significant impact on employment as most jobs remain unchanged.
- **C.** It could introduce new security challenges, require advanced big data solutions, and potentially disrupt employment.
- **D.** It will lead to reduced complexity in our daily lives and fewer security concerns.

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (It could introduce new security challenges, require advanced big data solutions, and potentially disrupt employment.)

**💡 Giải thích chi tiết:** Sự phát triển mạnh mẽ của IoT kết nối hàng loạt thiết bị gia dụng sẽ đặt ra các thách thức lớn về an ninh mạng, đòi hỏi các giải pháp xử lý dữ liệu lớn (Big Data) và có thể tác động sâu sắc đến cơ cấu việc làm.

---

### Câu 310 (Slide 310)

**Câu hỏi:** How is the input voltage range of 0 to 5 volts converted to a digital value between 0 and 1023 in an Arduino microcontroller?

**Các lựa chọn:**
- **A.** By using an external circuit.
- **B.** By using a digital-to-analog converter (DAC).
- **C.** By a process called analog-to-digital conversion (ADC) inside the microcontroller.
- **D.** By directly mapping the voltage to the digital value without conversion.

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (By a process called analog-to-digital conversion (ADC) inside the microcontroller.)

**💡 Giải thích chi tiết:** Điện áp analog 0 - 5V được chuyển đổi thành số nguyên 0 - 1023 nhờ bộ chuyển đổi tương tự sang số tích hợp bên trong vi điều khiển (ADC - Analog-to-Digital Conversion).

---

## Phần 4: Câu hỏi Lý thuyết & Ứng dụng Bổ sung (Slides 311+)

### Câu 312 (Slide 312)

**Câu hỏi:** How does IoT help improve tire maintenance in mining vehicles? A By inflating tires automatically

**Các lựa chọn:**
- **A.** By inflating tires automatically
- **B.** By monitoring tire pressure
- **C.** By replacing tires remotely
- **D.** By making tires more durable

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (By monitoring tire pressure)

**💡 Giải thích chi tiết:** Phương án B ('By monitoring tire pressure') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 313 (Slide 313)

**Câu hỏi:** How has the Internet of Things prompted new concerns over security issues?

**Các lựa chọn:**
- **A.** Devices are equipped with security from the manufacturer.
- **B.** Devices are less likely to be compromised in today's age.
- **C.** Devices are not compatible with traditional security measures.
- **D.** Devices respond only to user-installed security protocols.

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Devices are not compatible with traditional security measures.)

**💡 Giải thích chi tiết:** Phương án C ('Devices are not compatible with traditional security measures.') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 314 (Slide 314)

**Câu hỏi:** How many times does the loop() function run on every startup of the Arduino System?

**Các lựa chọn:**
- **A.** 1
- **B.** Depends upon the setup() function
- **C.** Infinitely till the power is supplied to the Arduino
- **D.** 3

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Infinitely till the power is supplied to the Arduino)

**💡 Giải thích chi tiết:** Phương án C ('Infinitely till the power is supplied to the Arduino') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 315 (Slide 315)

**Câu hỏi:** Why is C commonly used in IoT programming?

**Các lựa chọn:**
- **A.** Easy to use in graphic design
- **B.** Efficient in memory and performance
- **C.** Strong support for artificial intelligence
- **D.** Beautiful user interface

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (Efficient in memory and performance)

**💡 Giải thích chi tiết:** Phương án B ('Efficient in memory and performance') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 316 (Slide 316)

**Câu hỏi:** A photoresistor

**Các lựa chọn:**
- **A.** changes voltage according to light level
- **B.** increases or decreases current through a wire
- **C.** stores an image
- **D.** changes resistance according to light level

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (changes resistance according to light level)

**💡 Giải thích chi tiết:** Quang điện trở (Photoresistor / LDR) là linh kiện điện tử có điện trở thay đổi phụ thuộc vào mức độ chiếu sáng của môi trường xung quanh (ánh sáng càng mạnh điện trở càng giảm).

---

### Câu 317 (Slide 317)

**Câu hỏi:** Among the following protocols commonly used in IoT, which one is considered lightweight?

**Các lựa chọn:**
- **A.** IP (Internet Protocol)
- **B.** HTTP (Hypertext Transfer Protocol)
- **C.** MQTT (Message Queuing Telemetry Transport)
- **D.** Bluetooth

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (MQTT (Message Queuing Telemetry Transport))

**💡 Giải thích chi tiết:** Phương án C ('MQTT (Message Queuing Telemetry Transport)') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 318 (Slide 318)

**Câu hỏi:** An IOT device can most easily be differentiated from a standard computer based on

**Các lựa chọn:**
- **A.** Computational Performance
- **B.** Interface with the user and the world
- **C.** Memory Capacity
- **D.** Weight/Size

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (Interface with the user and the world)

**💡 Giải thích chi tiết:** Phương án B ('Interface with the user and the world') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 319 (Slide 319)

**Câu hỏi:** Can the loop() function be used to call another function that is custom defined by the programmer?

**Các lựa chọn:**
- **A.** Yes, it can call
- **B.** No, it cannot call
- **C.** Yes, it can call but only functions with no return values
- **D.** Yes, it can call but only functions with return values

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (Yes, it can call)

**💡 Giải thích chi tiết:** Phương án A ('Yes, it can call') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 320 (Slide 320)

**Câu hỏi:** Can the setup() function change the value of constant variables?

**Các lựa chọn:**
- **A.** Yes, it can change
- **B.** No, it cannot change
- **C.** Yes, it can change but only integer values
- **D.** Yes, it can change but only byte values

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (No, it cannot change)

**💡 Giải thích chi tiết:** Phương án B ('No, it cannot change') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 321 (Slide 321)

**Câu hỏi:** To program sending and receiving data between Arduino and BLUETOOTH HC06, how to connect the pins?

**Các lựa chọn:**
- **A.** TX connects to pin 0 and RX pin connects to pin 1 on Arduino
- **B.** TX connects to pin I and RX pin connects to pin O on Arduino
- **C.** TX connects to pin 1 and TX pin connects to pin 0 on Arduino
- **D.** RX connects to pin 1 and RX pin connects to pin 0 on Arduino

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (TX connects to pin 0 and RX pin connects to pin 1 on Arduino)

**💡 Giải thích chi tiết:** Phương án A ('TX connects to pin 0 and RX pin connects to pin 1 on Arduino B- TX connects to pin I and RX pin connects to pin O on Arduino') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 322 (Slide 322)

**Câu hỏi:** In the smart grid architecture of IoT, what is the primary function of the Cloud?

**Các lựa chọn:**
- **A.** Enhancing security
- **B.** Collecting data
- **C.** Managing data
- **D.** Storing data

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Managing data)

**💡 Giải thích chi tiết:** Trong kiến trúc lưới điện thông minh (Smart Grid), điện toán đám mây (Cloud) đóng vai trò trung tâm trong việc quản lý, tổng hợp và điều phối dữ liệu lớn (Managing data) từ hàng triệu đồng hồ đo điện thông minh.

---

### Câu 323 (Slide 323)

**Câu hỏi:** In a thin client setup, where is most of the software and data processing performed?

**Các lựa chọn:**
- **A.** Locally on the thin client device.
- **B.** On a central server or cloud infrastructure.
- **C.** On a central server or client infrastructure.
- **D.** On a dedicated network switch.

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (On a central server or cloud infrastructure.)

**💡 Giải thích chi tiết:** Phương án B ('On a central server or cloud infrastructure.') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 324 (Slide 324)

**Câu hỏi:** In IoT, what is the purpose of a Gateway? A To act as an intermediary for data transmission between different network protocols

**Các lựa chọn:**
- **A.** To act as an intermediary for data transmission between different network protocols
- **B.** To store data collected from IoT devices
- **C.** To increase the power supply to IoT devices
- **D.** To directly connect sensors to the internet

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (To act as an intermediary for data transmission between different network protocols)

**💡 Giải thích chi tiết:** Cổng kết nối IoT Gateway đóng vai trò làm cầu nối giữa mạng cảm biến cục bộ và mạng Internet toàn cầu, thực hiện chuyển đổi giao thức (protocol translation) và hỗ trợ định tuyến dữ liệu.

---

### Câu 325 (Slide 325)

**Câu hỏi:** In IoT, what is the purpose of a Gateway? A To act as an intermediary for data transmission between different network protocols

**Các lựa chọn:**
- **A.** Toactasanintermediaryfordatatransmissionbetweendifferentnetworkprotocols
- **B.** To store data collected from IoT devices
- **C.** To increase the power supply to IoT devices
- **D.** To directly connect sensors to the internet

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (Toactasanintermediaryfordatatransmissionbetweendifferentnetworkprotocols)

**💡 Giải thích chi tiết:** Cổng kết nối IoT Gateway đóng vai trò làm cầu nối giữa mạng cảm biến cục bộ và mạng Internet toàn cầu, thực hiện chuyển đổi giao thức (protocol translation) và hỗ trợ định tuyến dữ liệu.

---

### Câu 326 (Slide 326)

**Câu hỏi:** In a software simulation environment (Tinkercad) for Arduino programming, which of the following options is typically used to write and run code for your Arduino projects?

**Các lựa chọn:**
- **A.** Selecting the code option to start coding.
- **B.** Using a physical Arduino board to write code.
- **C.** Connecting various electronic components to a breadboard.
- **D.** Employing a real-time oscilloscope for debugging.

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (Selecting the code option to start coding.)

**💡 Giải thích chi tiết:** Phương án A ('Selecting the code option to start coding.') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 327 (Slide 327)

**Câu hỏi:** IOT devices gather private information about users. Which statement is most true about the security of that data?

**Các lựa chọn:**
- **A.** User can ensure security of collected data by encrypting it manually
- **B.** User can sue data collecting agencies if their data is not held securely
- **C.** Users must rely on data collecting agencies to securely store and transmit their data
- **D.** Most data gathered by IOT devices is safe because IOT devices are not a target of hackers

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Users must rely on data collecting agencies to securely store and transmit their data)

**💡 Giải thích chi tiết:** Phương án C ('Users must rely on data collecting agencies to securely store and transmit their data') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 328 (Slide 328)

**Câu hỏi:** IoT devices create more significant security challenges for networks due to all of these concerns EXCEPT which?

**Các lựa chọn:**
- **A.** They do not have security alerts.
- **B.** They are always on.
- **C.** They are always connected.
- **D.** They produce an event log

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (They produce an event log)

**💡 Giải thích chi tiết:** Phương án D ('They produce an event log') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 329 (Slide 329)

**Câu hỏi:** In the smart grid architecture of IoT, what is the primary function of the Cloud?

**Các lựa chọn:**
- **A.** Enhancing security
- **B.** Collecting data
- **C.** Managing data
- **D.** Storing data

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Managing data)

**💡 Giải thích chi tiết:** Trong kiến trúc lưới điện thông minh (Smart Grid), điện toán đám mây (Cloud) đóng vai trò trung tâm trong việc quản lý, tổng hợp và điều phối dữ liệu lớn (Managing data) từ hàng triệu đồng hồ đo điện thông minh.

---

### Câu 330 (Slide 330)

**Câu hỏi:** In a software simulation environment (Tinkercad) for Arduino programming, which of the following options is typically used to write and run code for your Arduino projects?

**Các lựa chọn:**
- **A.** Selecting the code option to start coding.
- **B.** Using a physical Arduino board to write code.
- **C.** Connecting various electronic components to a breadboard.
- **D.** Employing a real-time oscilloscope for debugging

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (Selecting the code option to start coding.)

**💡 Giải thích chi tiết:** Phương án A ('Selecting the code option to start coding.') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 331 (Slide 331)

**Câu hỏi:** In the context of IoT and networking, what does the abbreviation LPWAN stand for? A Lightweight Protocol for Wide Area Network

**Các lựa chọn:**
- **A.** Lightweight Protocol for Wide Area Network
- **B.** Low-Profile Wireless Access Node
- **C.** Low Power Wide Area Network
- **D.** Longitudinal Packet Wireless Architecture

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Low Power Wide Area Network)

**💡 Giải thích chi tiết:** Phương án C ('Low Power Wide Area Network') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 332 (Slide 332)

**Câu hỏi:** In the given Arduino code, what is the purpose of the "analogWrite" function, and how is it used to control the LED's behavior?

**Các lựa chọn:**
- **A.** The "analogWrite" function is used to read analog values from a sensor.
- **B.** The "analogWrite" function is used to blink the LED on and off.
- **C.** The "analogWrite" function is used to control the brightness of the LED.
- **D.** The "analogWrite" function is used to read digital values from a sensor.

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (The "analogWrite" function is used to control the brightness of the LED.)

**💡 Giải thích chi tiết:** Phương án C ('The "analogWrite" function is used to control the brightness of the LED.') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 333 (Slide 333)

**Câu hỏi:** In the Windows OS, which statement is true about the blocked state of a process?

**Các lựa chọn:**
- **A.** Waiting for an event triggered by the CPU's scheduling mechanism
- **B.** Waiting for an event that has not happened yet
- **C.** Waiting to input/output and Waiting for an event that has not happened yet
- **D.** The CPU and Memory are waiting to other events

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Waiting to input/output and Waiting for an event that has not happened yet)

**💡 Giải thích chi tiết:** Phương án C ('Waiting to input/output and Waiting for an event that has not happened yet') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 334 (Slide 334)

**Câu hỏi:** In what scenarios would you observe the TX LED blinking on an Arduino?

**Các lựa chọn:**
- **A.** When the Arduino is reading analog values
- **B.** When the Arduino is processing data
- **C.** VVhen the Arduino is transmitting data through the serial port
- **D.** VVhen the Arduino is in deep sleep mode

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (VVhen the Arduino is transmitting data through the serial port)

**💡 Giải thích chi tiết:** Phương án C ('VVhen the Arduino is transmitting data through the serial port') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 335 (Slide 335)

**Câu hỏi:** In terms of output format, how does the LM35 temperature sensor differ from the DS 1820? A LM35 provides temperature readings in digital format

**Các lựa chọn:**
- **A.** LM35providestemperaturereadingsindigitalformat
- **B.** DSI 820 provides temperature readings in analog format
- **C.** LM35 provides temperature readings in analog voltage
- **D.** DS1820 provides temperature readings in serial communication protocol

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (LM35 provides temperature readings in analog voltage)

**💡 Giải thích chi tiết:** Phương án C ('LM35 provides temperature readings in analog voltage') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 336 (Slide 336)

**Câu hỏi:** Is the Arduino code an Objectented programming language or a Procedural programming language? A The Arduino Code follows the Top-Down Procedural ideology

**Các lựa chọn:**
- **A.** TheArduinoCodefollowstheTop-DownProcedural ideology
- **B.** The Arduino Code follows a custom Procedural ideology
- **C.** The Arduino Code follows the Object-Oriented ideology
- **D.** The Arduino Code follows the Bottom-Up Procedural ideology

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (TheArduinoCodefollowstheTop-DownProcedural ideology)

**💡 Giải thích chi tiết:** Phương án A ('TheArduinoCodefollowstheTop-DownProcedural ideology') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 337 (Slide 337)

**Câu hỏi:** In a common cathode seven-segment display, what is common among all segments?

**Các lựa chọn:**
- **A.** All segments are connected to VCC
- **B.** All segments are connected to GND
- **C.** All segments have individual resistors
- **D.** All segments are controlled by separate pins

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (All segments are connected to GND)

**💡 Giải thích chi tiết:** Phương án B ('All segments are connected to GND') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 338 (Slide 338)

**Câu hỏi:** Is it possible to have multiple software serial ports (UART) with speeds up to 115200 bps?

**Các lựa chọn:**
- **A.** Yes, only one software serial port is possible.
- **B.** Yes, but the maximum speed is limited to 9600 bps.
- **C.** No, software serial ports are limited to a single port.
- **D.** Yes, multiple software serial ports are possible with speeds up to 115200 bps.

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (Yes, multiple software serial ports are possible with speeds up to 115200 bps.)

**💡 Giải thích chi tiết:** Phương án D ('Yes, multiple software serial ports are possible with speeds up to 115200 bps.') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 339 (Slide 339)

**Câu hỏi:** Which of the following statements about DHTII power consumption is NOT TRUE?

**Các lựa chọn:**
- **A.** It has low standby current
- **B.** It consumes high power continuously
- **C.** It draws current during measurement process
- **D.** It can work on battery power

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (It consumes high power continuously)

**💡 Giải thích chi tiết:** Phương án B ('It consumes high power continuously') là đáp án chính xác theo giáo trình môn IOT102. Khái niệm này thể hiện chuẩn xác nguyên lý kỹ thuật được đề cập trong câu hỏi.

---

### Câu 340 (Slide 340)

**Câu hỏi:** When using software serial, how many ports can receive data at a time? A Multiple ports can receive data simultaneously.

**Các lựa chọn:**
- **A.** Multiple ports can receive data simultaneously.
- **B.** Only one port can receive data at a time.
- **C.** All ports can send and receive data simultaneously.
- **D.** No ports can receive data, only send.

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (Only one port can receive data at a time.)

**💡 Giải thích chi tiết:** Khi sử dụng thư viện SoftwareSerial trên Arduino, tại một thời điểm chỉ có duy nhất một cổng nối tiếp ảo có thể nhận dữ liệu (Only one port can receive data at a time).

---

### Câu 341 (Slide 341)

**Câu hỏi:** Why is analogRead() useful in environmental monitoring projects with Arduino?

**Các lựa chọn:**
- **A.** It allows capturing continuous sensor values
- **B.** It converts digital pins to analog pins
- **C.** It stores values in EEPROM automatically
- **D.** It generates (Pulse Width Modulation) signals

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (It allows capturing continuous sensor values)

**💡 Giải thích chi tiết:** Hàm analogRead() cực kỳ hữu ích trong các dự án quan trắc môi trường vì nó cho phép đọc và chuyển đổi các giá trị vật lý liên tục (nhiệt độ, ánh sáng, độ ẩm) thành giá trị số nguyên.

---

### Câu 342 (Slide 342)

**Câu hỏi:** What is an actuator in an Arduino UNO?

**Các lựa chọn:**
- **A.** A device that receives data
- **B.** A device that outputs data
- **C.** A device that stores data
- **D.** A device that communicates with other devices

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (A device that outputs data)

**💡 Giải thích chi tiết:** Trong hệ thống Arduino, cơ cấu chấp hành (Actuator) là thiết bị nhận tín hiệu điều khiển đầu ra từ vi điều khiển để thực hiện tác vụ cơ học, quang học hoặc âm thanh.

---

### Câu 343 (Slide 343)

**Câu hỏi:** If you observe that pressing a key on your keypad sometimes prints incorrect characters, which debugging steps should you take to identify and correct the issue?

**Các lựa chọn:**
- **A.** Check if the row and column pins are defined correctly in the code.
- **B.** Ensure that the Keypad library is installed correctly.
- **C.** Verify the wiring connections between the keypad and Arduino.
- **D.** All of the others

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (All of the others)

**💡 Giải thích chi tiết:** Khi bàn phím ma trận keypad in sai ký tự, các bước gỡ lỗi cần thiết là: kiểm tra thứ tự khai báo chân hàng và cột trong code, kiểm tra thư viện Keypad và kiểm tra lại dây nối phần cứng (All of the others).

---

### Câu 344 (Slide 344)

**Câu hỏi:** What is a key characteristic of IoT?

**Các lựa chọn:**
- **A.** Devices operate independently without connectivity.
- **B.** Devices connect and communicate over the internet.
- **C.** Devices function only with human intervention.
- **D.** Devices do not collect any data

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (Devices connect and communicate over the internet.)

**💡 Giải thích chi tiết:** Đặc tính cốt lõi của IoT là các thiết bị có khả năng kết nối và giao tiếp dữ liệu với nhau qua mạng Internet (Devices connect and communicate over the internet).

---

### Câu 345 (Slide 345)

**Câu hỏi:** Identify the main considerations that small devices generally have when programming for IoT devices.

**Các lựa chọn:**
- **A.** Limited power supply, limited network bandwidth, and limited memory.
- **B.** Limited power supply, limited computational power, and limited memory.
- **C.** Advanced security features, simple user interfaces, and high-resolution displays.
- **D.** Advanced security features, complex user interfaces, and high-resolution displays.

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (Limited power supply, limited computational power, and limited memory.)

**💡 Giải thích chi tiết:** Khi lập trình cho các thiết bị IoT nhỏ gọn (như vi điều khiển), 3 hạn chế chính cần lưu tâm là: nguồn năng lượng giới hạn, năng lực tính toán hạn chế và dung lượng bộ nhớ nhỏ.

---

## Phần 5: Dạng câu hỏi NOT (Chọn đáp án SAI / Không đúng)

### Câu 347 (Slide 347)

**Câu hỏi:** Which of these colors is NOT used in the resistor color code? A Violet

**Các lựa chọn:**
- **A.** Violet
- **B.** Yellow
- **C.** Magenta
- **D.** White

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Magenta)

**💡 Giải thích chi tiết:** Trong bảng mã màu điện trở quốc tế (đen, nâu, đỏ, cam, vàng, lục, lam, tím, xám, trắng), màu hồng tím Magenta KHÔNG được sử dụng.

---

### Câu 348 (Slide 348)

**Câu hỏi:** Which factor is NOT essential for a successful IoT project?

**Các lựa chọn:**
- **A.** Addressing a real-world problem
- **B.** Providing a unique benefit
- **C.** Targeting a specific audience
- **D.** Using the most expensive technology available

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (Using the most expensive technology available)

**💡 Giải thích chi tiết:** Để một dự án IoT thành công, việc sử dụng công nghệ đắt tiền nhất (Using the most expensive technology available) KHÔNG PHẢI là yếu tố cần thiết, quan trọng là giải quyết đúng bài toán thực tế với chi phí tối ưu.

---

### Câu 349 (Slide 349)

**Câu hỏi:** Which Arduino UNO pin is NOT typically used for external interrupts?

**Các lựa chọn:**
- **A.** Pin 2
- **B.** Pin 3
- **C.** Pin 5
- **D.** None of the above

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Pin 5)

> ⚠️ LƯU Ý LỖI IN: Slide gốc in thiếu phương án D thành ký tự "e.". Đáp án đúng là C: Pin 5 không phải chân ngắt ngoài.

**💡 Giải thích chi tiết:** ⚠️ LƯU Ý LỖI IN: Trên Arduino Uno R3, ngắt ngoài phần cứng chỉ hỗ trợ trên chân 2 và 3. Chân 5 là chân PWM, KHÔNG hỗ trợ ngắt ngoài.

---

### Câu 350 (Slide 350)

**Câu hỏi:** Which digital pin of Arduino Uno Rev3 does NOT provide PWM output?

**Các lựa chọn:**
- **A.** 3
- **B.** 5
- **C.** 8
- **D.** 10

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (8)

**💡 Giải thích chi tiết:** Trên Arduino Uno Rev3, các chân PWM là 3, 5, 6, 9, 10, 11. Chân Digital số 8 KHÔNG hỗ trợ xuất xung PWM.

---

### Câu 351 (Slide 351)

**Câu hỏi:** Which of the following factors is NOT typically considered when choosing the medium for network communication in an IoT setup? A The distance a signal needs to travel.

**Các lựa chọn:**
- **A.** The distance a signal needs to travel.
- **B.** The type of data being transmitted.
- **C.** The color of the cables.
- **D.** The cost of the media and its installation.

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (The color of the cables.)

**💡 Giải thích chi tiết:** Màu sắc của vỏ bọc dây cáp mạng (The color of the cables) chỉ mang tính quy ước quản lý, KHÔNG PHẢI là yếu tố kỹ thuật quyết định khi chọn môi trường truyền dẫn mạng.

---

### Câu 352 (Slide 352)

**Câu hỏi:** Which of the following statements is WRONG about the IoT devices?

**Các lựa chọn:**
- **A.** IoT devices use the internet for collecting and sharing data
- **B.** IoT devices need microcontroller
- **C.** IoT devices use wireless technology
- **D.** IoT devices are completely safe

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (IoT devices are completely safe)

**💡 Giải thích chi tiết:** Phát biểu cho rằng các thiết bị IoT 'hoàn toàn an toàn' (IoT devices are completely safe) là SAI, vì thiết bị IoT là đối tượng thường xuyên phải đối mặt với nhiều nguy cơ tấn công mạng.

---

### Câu 353 (Slide 353)

**Câu hỏi:** Which of these is NOT a benefit of Arduino shields?

**Các lựa chọn:**
- **A.** It is simple to use.
- **B.** It makes the Arduino faster
- **C.** It is pre-wired.
- **D.** None of the mentioned

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (It makes the Arduino faster)

**💡 Giải thích chi tiết:** Arduino Shield là các bo mạch mở rộng cắm chồng lên Arduino giúp mở rộng tính năng và tiện lợi khi nối dây, nhưng nó KHÔNG làm tăng tốc độ xử lý xung nhịp của vi điều khiển (It makes the Arduino faster là SAI).

---

### Câu 354 (Slide 354)

**Câu hỏi:** Which of the following is NOT an advantage of IoTQ

**Các lựa chọn:**
- **A.** Security
- **B.** Enhanced data collection
- **C.** Reduced waste
- **D.** Improved customer engagement

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (Security)

**💡 Giải thích chi tiết:** Bảo mật (Security) là một trong những thách thức và điểm yếu lớn nhất của IoT chứ KHÔNG PHẢI là ưu điểm (advantage) của nó.

---

### Câu 355 (Slide 355)

**Câu hỏi:** Which of the following is NOT the essential elements of a use case?

**Các lựa chọn:**
- **A.** ID and Name
- **B.** Description
- **C.** A trigger condition
- **D.** Zero or more preconditions, one or more postconditions
- **E.** Normal Flow
- **F.** Alternative flow

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (A trigger condition)

**💡 Giải thích chi tiết:** Các thành phần cốt lõi của một use case gồm ID, tên, mô tả, luồng chính, luồng phụ, điều kiện tiên quyết và hậu quyết; Trigger condition không phải là thành phần định nghĩa thiết yếu trong mọi mô hình use case chuẩn.

---

### Câu 356 (Slide 356)

**Câu hỏi:** Which of the following is NOT related to Arduino IDE software?

**Các lựa chọn:**
- **A.** Serial monitor
- **B.** Upload
- **C.** Terminate
- **D.** verify

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (Terminate)

**💡 Giải thích chi tiết:** Trong giao diện phần mềm Arduino IDE có các nút Verify (biên dịch), Upload (nạp code), Serial Monitor (cửa sổ theo dõi). Chức năng 'Terminate' KHÔNG thuộc về Arduino IDE.

---

### Câu 357 (Slide 357)

**Câu hỏi:** Which of the following is NOT a sensor in IoT?

**Các lựa chọn:**
- **A.** BMP280
- **B.** DHTII
- **C.** Photoresistor
- **D.** LED

- **Đáp án trong ghi chú:** `D`
- **Đáp án chính xác:** **D** (LED)

**💡 Giải thích chi tiết:** LED (Light Emitting Diode) là một cơ cấu chấp hành phát quang đầu ra (Actuator/Output), KHÔNG PHẢI là một cảm biến (Sensor).

---

### Câu 358 (Slide 358)

**Câu hỏi:** Which of the following statements about the MQ-3 sensor is NOT TRUE?

**Các lựa chọn:**
- **A.** It has a preheat time requirement
- **B.** It responds instantly after power-on
- **C.** It needs warm-up for stable readings
- **D.** Temperature affects its sensitivity

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (It responds instantly after power-on)

**💡 Giải thích chi tiết:** Cảm biến khí cồn MQ-3 sử dụng dây đốt nóng hóa học bên trong, đòi hỏi phải có thời gian sấy nóng (preheat time khoảng 24-48h khi mới dùng hoặc vài phút khi bật) mới ổn định, do đó phát biểu nó đáp ứng tức thì ngay sau khi bật nguồn là SAI.

---

### Câu 359 (Slide 359)

**Câu hỏi:** Which of the following is NOT an actuator in IoT?

**Các lựa chọn:**
- **A.** A push button
- **B.** An LED
- **C.** A servo motor
- **D.** A buzzer

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (A push button)

**💡 Giải thích chi tiết:** Nút nhấn (Push button) là một cảm biến tiếp xúc / thiết bị đầu vào (Input/Sensor), KHÔNG PHẢI là cơ cấu chấp hành (Actuator). Các phương án LED, động cơ servo, còi buzzer đều là actuator.

---

### Câu 360 (Slide 360)

**Câu hỏi:** The following trend is NOT related to the growth in IOT technology

**Các lựa chọn:**
- **A.** Increase in computer monitor size over time
- **B.** Decrease in computer size over time
- **C.** Increase in computer performance over time
- **D.** Decrease in computer cost over time

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (Increase in computer monitor size over time)

**💡 Giải thích chi tiết:** Kích thước màn hình máy tính tăng lên không liên quan trực tiếp đến sự phát triển của công nghệ IoT. IoT gắn liền với xu hướng chip máy tính ngày càng nhỏ, hiệu năng cao hơn và giá thành rẻ hơn.

---

### Câu 361 (Slide 361)

**Câu hỏi:** Which of the following is FALSE about the IoT hardware component?

**Các lựa chọn:**
- **A.** A keyboard is a digital sensor
- **B.** A photodiode is an analog sensor.
- **C.** A microphone is a digital sensor.
- **D.** A push button is a digital sensor.

- **Đáp án trong ghi chú:** `C`
- **Đáp án chính xác:** **C** (A microphone is a digital sensor.)

**💡 Giải thích chi tiết:** Microphone là một cảm biến tương tự (Analog sensor) chuyển đổi sóng âm thanh liên tục thành điện áp analog, do đó phát biểu cho rằng microphone là cảm biến số (digital sensor) là SAI.

---

## Phần 6: Dạng True / False

### Câu 363 (Slide 363)

**Câu hỏi:** Arduino can be used to develop interactive objects that can work without a computer.

**Các lựa chọn:**
- **A.** TRUE
- **B.** FALSE

- **Đáp án trong ghi chú:** `A`
- **Đáp án chính xác:** **A** (TRUE)

**💡 Giải thích chi tiết:** ĐÚNG: Sau khi nạp code, Arduino có thể hoạt động độc lập bằng nguồn pin/adapter mà không cần kết nối với máy tính.

---

### Câu 364 (Slide 364)

**Câu hỏi:** In Arduino, a "Sketch" is a diagram that shows the physical arrangement of the components.

**Các lựa chọn:**
- **A.** TRUE
- **B.** FALSE

- **Đáp án trong ghi chú:** `B`
- **Đáp án chính xác:** **B** (FALSE)

**💡 Giải thích chi tiết:** SAI: Trong thuật ngữ Arduino, 'Sketch' là tên gọi của chương trình phần mềm (mã code) viết cho vi điều khiển, KHÔNG PHẢI là sơ đồ bố trí linh kiện vật lý.

---

