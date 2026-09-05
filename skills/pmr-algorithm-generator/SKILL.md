---
name: pmr-algorithm-generator
description: >-
  Sử dụng skill này khi cần chuyển đổi các phác đồ và quy trình can thiệp phức tạp thành Lưu đồ thuật toán ra quyết định lâm sàng (Clinical Decision Flowchart) trực quan bằng cú pháp Mermaid/Markdown.
---

# PMR Algorithm Generator: Dựng Lưu Đồ Quyết Định Lâm Sàng

Kỹ năng này phụ trách việc trực quan hóa các hướng dẫn điều trị dài dòng thành **Lưu đồ thuật toán (Flowchart)** mạch lạc, logic bằng cú pháp **Mermaid**. Giúp học viên Đại học và Sau đại học nắm bắt nhanh các bước ra quyết định lâm sàng từ lúc tiếp nhận đến khi ra viện.

---

## Quy Tắc Thiết Kế Sơ Đồ Mermaid Chuẩn

1. **Điểm bắt đầu & kết thúc:** Dùng hình ô van/viên thuốc `([Bắt đầu / Kết thúc])`.
2. **Hành động / Can thiệp:** Dùng hình chữ nhật `[Hành động / Lượng giá]`.
3. **Điểm rẽ nhánh quyết định:** Dùng hình thoi `{Câu hỏi quyết định?}` với nhánh `Yes` và `No`.
4. **Cảnh báo khẩn cấp / Cờ đỏ:** Đặt màu sắc cảnh báo hoặc khung nổi bật.

---

## Mẫu Thuật Toán Ra Quyết Định Mẫu (Decision Tree)

```mermaid
graph TD
    A([Tiếp nhận Người bệnh PHCN]) --> B[Khám Lâm sàng & Lượng giá ICF ban đầu]
    B --> C{Có Dấu hiệu Cờ đỏ Red Flags?}
    
    C -- Yes --> D[🚨 NGỪNG PHCN - Chuyển Cấp cứu / Ngoại khoa]
    C -- No --> E{Giai đoạn Tổn thương?}
    
    E -- Cấp tính ngày 1-14 --> F[Bảo vệ can xương + Giảm đau TENS + NMES chống teo cơ + PROM nhẹ nhàng]
    E -- Bán cấp tuần 3-6 --> G[AAROM + Di động khớp Maitland độ I-II + Hoạt động trị liệu ngón tay]
    E -- Mạn tính sau tuần 6 --> H{Đã có Can xương vững chắc?}
    
    H -- No --> I[Tiếp tục tập có kiểm soát + Sóng xung kích nếu chậm liền xương]
    H -- Yes --> K[Nhiệt sâu Siêu âm + Di động khớp độ III-IV + Bài tập đề kháng tăng tiến PRE + Phục hồi chức năng nghề nghiệp]
    
    F --> L[Tái lượng giá DASH / VAS mỗi tuần]
    G --> L
    K --> M([Đạt Tiêu chuẩn Xuất viện & Trở lại Hoạt động])
```
