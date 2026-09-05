---
name: pmr-ebook-master
description: >-
  Sử dụng skill này khi người dùng yêu cầu điều phối biên soạn trọn gói bài giảng hoặc chương sách Ebook Phục hồi chức năng (PM&R), bao gồm cả bài giảng Lý thuyết thuần và bài giảng Lý thuyết lâm sàng theo chuẩn mực sư phạm y khoa Singapore và quy định Bộ Y tế Việt Nam.
---

# Kỹ Năng Nhạc Trưởng: Biên Soạn Ebook Bài Giảng Phục Hồi Chức Năng (Master Orchestrator)

Kỹ năng này đóng vai trò **Nhạc trưởng (Orchestrator)** điều phối toàn bộ quy trình biên soạn giáo trình và bài giảng Phục hồi Chức năng & Vật lý Trị liệu (PM&R) ở đẳng cấp học thuật cao, tích hợp chuẩn giáo dục y khoa Singapore (NUS / Duke-NUS) và khung pháp lý - kỹ thuật Bộ Y tế Việt Nam 2024–2025.

---

## Khi Nào Kích Hoạt (Trigger Conditions)

- Người dùng yêu cầu: *"Soạn bài giảng PHCN..."*, *"Biên soạn chương sách Ebook về..."*, *"Viết bài giảng lý thuyết / lâm sàng cho..."*.
- Cần xây dựng giáo trình hoàn chỉnh phân tầng rõ giữa Đại học (Bác sĩ Y khoa - Bậc 7 VQF) và Sau đại học (BSNT, CKI, ThS - Bậc 8 VQF).

---

## Khung Quy Trình 5 Bước Điều Phối Tuần Hoàn (Master Workflow)

Khi nhận chủ đề bài giảng (ví dụ: *PHCN Gãy Xương Cẳng Tay*, *Điện Trị Liệu Giảm Đau*, *PHCN Đột Quỵ Não*):

```text
[BƯỚC 1: SƯ PHẠM & CHUẨN ĐẦU RA]
  ├── Kích hoạt `pmr-matrix-designer`: Phân định Chuẩn đầu ra ĐH (Bậc 7) vs SĐH (Bậc 8).
  └── Kích hoạt `pmr-icf-core-mapper`: Phân tích khiếm khuyết b/s, d, e theo khung ICF của WHO.
         │
         ▼
[BƯỚC 2: CƠ SỞ KHOA HỌC & BẰNG CHỨNG (Cho Bài Lý Thuyết Thuần)]
  ├── Kích hoạt `pmr-biophysics-explainer`: Biện giải chuỗi Vật lý cơ bản ➔ Vật lý Y sinh ➔ Mô học.
  └── Kích hoạt `pmr-pedro-ebm-verifier`: Rà soát Tháp chứng cứ 3 tầng (Textbooks kinh điển, CPGs, Q1 RCTs).
         │
         ▼
[BƯỚC 3: THIẾT KẾ LÂM SÀNG CHUYÊN SÂU (Cho Bài Lý Thuyết Lâm Sàng)]
  ├── Kích hoạt `pmr-anchor-case-author`: Dựng ca bệnh mỏ neo thực tế (Anchor Case - CBL Singapore).
  ├── Kích hoạt `pmr-prescription-builder`: Kê đơn PHCN chi tiết từng thông số (FITT, mA, μs, Hz...).
  └── Kích hoạt `pmr-postgrad-deepdive`: Xây dựng module SĐH (Xử trí ca khó, biến chứng, kỹ thuật cao).
         │
         ▼
[BƯỚC 4: RÀ SOÁT PHÁP LÝ & AN TOÀN NGƯỜI BỆNH]
  ├── Kích hoạt `pmr-moh-legal-checker`: Khớp mã quy trình kỹ thuật BYT 2024–2025, phân quyền BS vs KTV.
  └── Kích hoạt `pmr-safety-redflag-guard`: Thiết lập hộp Cờ đỏ (Red Flags), chống chỉ định, an toàn điện.
         │
         ▼
[BƯỚC 5: CHẾ BẢN, LƯU ĐỒ THUẬT TOÁN & LƯỢNG GIÁ]
  ├── Kích hoạt `pmr-algorithm-generator`: Dựng sơ đồ dòng quyết định lâm sàng (Mermaid Flowchart).
  ├── Kích hoạt `pmr-assessment-generator`: Soạn ngân hàng câu hỏi MCQ/MEQ chuẩn thi Quốc gia/SĐH.
  └── Kích hoạt `pmr-ebook-packager`: Đóng gói chuẩn Markdown, hộp sư phạm Clinical Pearls & xuất bản.
```

---

## Nguyên Tắc Vận Hành Cốt Lõi

1. **Không Viết Tùy Tiện:** Mọi thông số điều trị (tần số, cường độ, thời gian) phải có trích dẫn từ Textbook kinh điển (Cameron, Braddom) hoặc nghiên cứu Q1 (PEDro $\ge 7/10$).
2. **Tuân Thủ Pháp Lý Tuyệt Đối:** Mọi can thiệp phải đối chiếu với Danh mục kỹ thuật Bộ Y tế Việt Nam 2024–2025 và Luật Khám bệnh, chữa bệnh 2023.
3. **Phân Định 2 Dạng Bài:** Luôn hỏi rõ hoặc tự động tạo cấu trúc song hành: *Bài giảng Lý thuyết thuần* (bản chất cơ chế) và *Bài giảng Lý thuyết lâm sàng* (ứng dụng điều trị).
