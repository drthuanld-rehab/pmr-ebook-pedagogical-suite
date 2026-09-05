---
name: pmr-prescription-builder
description: >-
  Sử dụng skill này khi cần soạn thảo Đơn điều trị Phục hồi chức năng (Rehabilitation Prescription) chi tiết và chuẩn xác đến từng thông số kỹ thuật (dạng dòng điện, cường độ mA, độ rộng xung μs, tần số Hz, chu kỳ co/nghỉ, vị trí điện cực, thông số siêu âm BNR/ERA, nguyên tắc FITT và kỹ thuật di động khớp Maitland).
---

# PMR Prescription Builder: Kê Đơn Phục Hồi Chức Năng Chi Tiết Từng Thông Số

Kỹ năng này chuẩn hóa việc ra y lệnh can thiệp PHCN. Y lệnh PHCN không được viết chung chung (như *"chiếu đèn hồng ngoại, tập vận động"*) mà phải chi tiết, định lượng chuẩn xác như một đơn thuốc điều trị.

---

## Cấu Trúc Kê Đơn Các Phương Thức Cụ Thể

### 1. Kê Đơn Điện Trị Liệu (Electrotherapy Rx)
* **Dòng giảm đau (TENS):**
  * Loại: TENS quy ước (High-rate) hoặc TENS châm cứu (Low-rate/Acupuncture-like).
  * Dạng sóng: Xung chữ nhật 2 pha cân đối (Symmetrical biphasic).
  * Tần số ($f$): $80 - 100	ext{ Hz}$ (quy ước) hoặc $2 - 4	ext{ Hz}$ (châm cứu).
  * Độ rộng xung ($t$): $50 - 80\ \mu s$ (quy ước) hoặc $150 - 250\ \mu s$ (châm cứu).
  * Cường độ ($I$): Chỉnh đến ngưỡng "tê rần dễ chịu, không co cơ" (mA).
  * Vị trí đặt điện cực: Cực âm - cực dương bao quanh vùng đau hoặc dọc đường đi rễ thần kinh.
  * Thời gian & Liệu trình: 30 phút/lần, 1-2 lần/ngày, liệu trình 10-14 ngày.
* **Dòng kích thích thần kinh - cơ (NMES):**
  * Dạng sóng: Dòng Russian (2500 Hz burst modulated at 50 Hz) hoặc Biphasic.
  * Tần số: $35 - 50	ext{ Hz}$ (đạt co cứng cơ trơn tru - tetanic contraction).
  * Độ rộng xung: $200 - 400\ \mu s$.
  * Chu kỳ co/nghỉ (Duty Cycle): Tỷ lệ $1:3$ hoặc $1:5$ (ví dụ: Co 6 giây, nghỉ 18-30 giây) tránh mỏi cơ.
  * Thời gian dốc (Ramp up/down): 1-2 giây.
  * Vị trí: Đặt trên điểm vận động (Motor points) của bụng cơ.

### 2. Kê Đơn Siêu Âm Trị Liệu (Ultrasound Rx)
* Tần số: $1	ext{ MHz}$ (mô sâu 3-5 cm) hoặc $3	ext{ MHz}$ (mô nông 1-2 cm).
* Chế độ: Xung (Pulsed 20% duty cycle) cho giai đoạn cấp/bán cấp (hiệu ứng cơ sinh); Liên tục (Continuous 100%) cho giai đoạn mạn cần nhiệt sâu.
* Cường độ: $0.5 - 1.0	ext{ W/cm}^2$ (xung) hoặc $1.0 - 1.5	ext{ W/cm}^2$ (liên tục).
* Thời gian: $5 - 8	ext{ phút}$ cho mỗi vùng diện tích bằng 2 lần ERA của đầu dò.
* Kỹ thuật: Di động đầu dò liên tục xoay tròn hoặc ziczac với tốc độ $2 - 4	ext{ cm/s}$, dùng gel dẫn âm tiêu chuẩn.

### 3. Kê Đơn Bài Tập Vận Động (Therapeutic Exercise Rx - Nguyên tắc FITT)
* **F (Frequency):** Số buổi/tuần, số lần/ngày.
* **I (Intensity):** Kháng trở (% 1RM), góc độ ROM cho phép, thang điểm gắng sức RPE (Borg scale).
* **T (Time):** Số hiệp (Sets), số lần lặp (Reps), thời gian giữ đẳng trường (Hold time).
* **T (Type):** Bài tập thụ động (PROM), chủ động có trợ giúp (AAROM), chủ động tự do (AROM), đề kháng tăng tiến (PRE), kéo giãn tĩnh (Static stretch).
* **Kỹ thuật Di động khớp (Joint Mobilization - Maitland):**
  * Độ I-II: Biên độ nhỏ/lớn ở đầu tầm $ightarrow$ Giảm đau, tăng tuần hoàn hoạt dịch (dùng giai đoạn cấp/đau nhiều).
  * Độ III-IV: Biên độ lớn/nhỏ ở cuối tầm $ightarrow$ Kéo giãn bao khớp, phá vỡ dính khớp (giai đoạn mạn).
