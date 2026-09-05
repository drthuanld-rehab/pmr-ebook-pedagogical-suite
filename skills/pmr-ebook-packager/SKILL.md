---
name: pmr-ebook-packager
description: >-
  Sử dụng skill này khi cần đóng gói, kiểm soát định dạng bản thảo Markdown, thiết kế cấu trúc chương sách Ebook chuẩn xuất bản, tạo các khối sư phạm đặc biệt (Clinical Pearls, Safety Warning Boxes, Evidence Summary Tables) và chuẩn bị cho việc biên dịch sang PDF/ePub.
---

# PMR Ebook Packager: Chế Bản & Đóng Gói Ebook Tương Tác

Kỹ năng này hoàn thiện khâu cuối cùng của quá trình biên soạn: **Chế bản mỹ thuật học thuật**, chuẩn hóa cấu trúc tệp Markdown, tích hợp các thành tố sư phạm tương tác cao và sẵn sàng xuất bản sang các định dạng sách điện tử hiện đại (PDF, ePub3, HTML5).

---

## Các Khối Sư Phạm Đặc Biệt (Pedagogical Callout Boxes)

Agent phải sử dụng cú pháp chuẩn GitHub Alert để tạo các hộp nổi bật trong bài giảng:

> [!NOTE]
> **Khung Lý thuyết Nền tảng (Theoretical Foundations):** Tóm tắt các định luật vật lý, sinh cơ học hoặc mô học cốt lõi cần ghi nhớ.

> [!TIP]
> **Viên Ngọc Lâm Sàng (Clinical Pearls):** Mẹo thực hành lâm sàng đúc rút từ các chuyên gia đầu ngành, kinh nghiệm đặt điện cực, xử lý da tiếp xúc hoặc tư thế bệnh nhân thoải mái nhất.

> [!IMPORTANT]
> **Điểm Nhấn Quy Trình Bộ Y Tế:** Các lưu ý bắt buộc về quy chuẩn hồ sơ bệnh án, mã quy trình kỹ thuật và định mức BHYT.

> [!WARNING]
> **Cảnh Báo Chống Chỉ Định (Contraindication Alert):** Nhắc nhở nguy cơ bỏng nhiệt, tổn thương mô hoặc biến chứng nếu không tuân thủ thông số kỹ thuật.

> [!CAUTION]
> **Cờ Đỏ Cấp Cứu (Red Flags Alert):** Các dấu hiệu yêu cầu dừng can thiệp PHCN khẩn cấp và chuyển viện/ngoại khoa.

---

## Cấu Trúc Đặt Tên & Quản Lý Tệp Bài Giảng

* **Bài giảng Lý thuyết thuần:** `[SốThứTự]-LT-[TênChủĐề].md` (Ví dụ: `01-LT-Gay-Xuong-Cang-Tay-Co-So-Sinh-Hoc-Vat-Ly-Y-Sinh.md`).
* **Bài giảng Lý thuyết lâm sàng:** `[SốThứTự]-LS-[TênChủĐề].md` (Ví dụ: `02-LS-Gay-Xuong-Cang-Tay-Luong-Gia-Ke-Don-PHCN.md`).
* Mọi tệp đều có mục lục liên kết (Table of Contents), trích dẫn tài liệu tham khảo theo chuẩn Vancouver hoặc APA 7th.
