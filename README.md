# PM&R Pedagogical Skill Suite (Medical Ebook Suite)
### Hệ Thống Kỹ Năng AI Chuyên Sâu Biên Soạn Ebook Bài Giảng Phục Hồi Chức Năng & Vật Lý Trị Liệu

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Antigravity IDE](https://img.shields.io/badge/Antigravity-Compatible-blue.svg)](https://antigravity.google)
[![Claude Projects](https://img.shields.io/badge/Claude-Compatible-purple.svg)](https://anthropic.com)
[![Codex / OpenAI](https://img.shields.io/badge/Codex-Compatible-green.svg)](https://openai.com)

**PM&R Pedagogical Skill Suite** là bộ kỹ năng chuyên biệt dành cho các Trợ lý AI (Antigravity IDE, Anthropic Claude, OpenAI Codex/ChatGPT) nhằm tự động hóa quy trình biên soạn giáo trình, chương sách Ebook và bài giảng Y khoa chuẩn mực cao cho chuyên ngành **Phục hồi Chức năng & Vật lý Trị liệu (PM&R)**.

Bộ kỹ năng được xây dựng trên triết lý kết hợp **Chuẩn mực sư phạm y khoa Singapore** (NUS Medicine, Duke-NUS, mô hình ICF của WHO, Case-Based Learning) với **Khung pháp lý & Danh mục kỹ thuật mới nhất của Bộ Y tế Việt Nam (2024–2025)** và **Tháp y học chứng cứ 3 tầng (Textbook kinh điển, CPGs, Q1 RCTs với thang PEDro)**.

---

## 🌟 Tính Năng Nổi Bật

1. **Phân Tầng Năng Lực Rõ Ràng (VQF):**
   - **Bậc Đại học (Bác sĩ Y khoa - Bậc 7 VQF):** Tập trung chỉ định, khám lượng giá cơ bản, nhận diện cờ đỏ an toàn, quy trình BYT.
   - **Bậc Sau đại học (BSNT, CKI, ThS - Bậc 8 VQF):** Đi sâu vào bệnh sinh phân tử, điện sinh lý, lập luận ca khó, kỹ thuật can thiệp cao (BoNT-A dưới siêu âm, robot, rTMS).
2. **Gốc Rễ Toán - Lý - Sinh Học Vững Chắc:** Không chỉ dạy thông số điều trị ngọn mà giải thích cặn kẽ chuỗi: *Vật lý phổ thông $ightarrow$ Vật lý y sinh $ightarrow$ Điện sinh lý $ightarrow$ Tương tác mô học*.
3. **Tuân Thủ Pháp Lý Bộ Y Tế Việt Nam 2024–2025:** Phân định rõ trách nhiệm Bác sĩ PHCN (kê đơn, ký bệnh án) vs Kỹ thuật viên (thực hiện kỹ thuật), khớp mã quy trình kỹ thuật BYT.
4. **Chuẩn Hóa Đơn Can Thiệp:** Kê đơn chi tiết như đơn thuốc: dạng dòng điện, mA, $\mu s$, Hz, tỷ lệ co:nghỉ, nguyên tắc FITT, Maitland...
5. **Tương Thích Đa Nền Tảng (Universal Markdown Architecture):** Sử dụng chung cho Antigravity IDE, Claude và Codex.

---

## 📂 Cấu Trúc Hệ Thống (13 Skills Chuyên Biệt)

```text
pmr-ebook-pedagogical-suite/
├── docs/                                      # Tài liệu nền tảng y học & pháp lý
│   ├── ARCHITECTURE.md                        # Kiến trúc hệ thống UMA
│   ├── BYT_TECHNIQUES_2025.md                 # Quy trình kỹ thuật BYT 2024-2025 & Luật KBCB 2023
│   └── PEDRO_EBM_GUIDE.md                     # Hướng dẫn thang đo PEDro & Tháp chứng cứ Q1
├── examples/                                  # Bài giảng mẫu hoàn chỉnh
│   ├── 01-pure-theory-forearm-fracture.md     # Bài 1: Lý thuyết cơ sở sinh học & vật lý y sinh
│   └── 02-clinical-theory-forearm-fracture.md # Bài 2: Lý thuyết lâm sàng lượng giá & kê đơn
└── skills/                                    # 13 thư mục Custom Skills
    ├── pmr-ebook-master/                      # [Nhạc trưởng] Điều phối toàn bộ quy trình biên soạn
    ├── pmr-matrix-designer/                   # [Nhóm 1] Ma trận Chuẩn đầu ra ĐH (Bậc 7) vs SĐH (Bậc 8)
    ├── pmr-icf-core-mapper/                   # [Nhóm 1] Chuẩn hóa lượng giá theo mô hình ICF của WHO
    ├── pmr-biophysics-explainer/              # [Nhóm 2] Biện giải cơ sở vật lý cơ bản & vật lý y sinh
    ├── pmr-pedro-ebm-verifier/                # [Nhóm 2] Thẩm định chứng cứ lâm sàng PEDro & Guidelines
    ├── pmr-anchor-case-author/                # [Nhóm 3] Xây dựng ca lâm sàng mỏ neo (Anchor Case - CBL)
    ├── pmr-prescription-builder/              # [Nhóm 3] Kê đơn thông số can thiệp PHCN chi tiết (FITT, mA...)
    ├── pmr-postgrad-deepdive/                 # [Nhóm 3] Chuyên đề Sau đại học: Ca khó, can thiệp kỹ thuật cao
    ├── pmr-moh-legal-checker/                 # [Nhóm 4] Đối chiếu quy trình BYT 2024-2025, phân quyền BS vs KTV
    ├── pmr-safety-redflag-guard/              # [Nhóm 4] Rà soát cờ đỏ (Red Flags), chống chỉ định, an toàn điện
    ├── pmr-algorithm-generator/               # [Nhóm 5] Dựng lưu đồ thuật toán quyết định lâm sàng Mermaid
    ├── pmr-assessment-generator/              # [Nhóm 5] Soạn câu hỏi tự lượng giá MCQ/MEQ chuẩn quốc gia
    └── pmr-ebook-packager/                    # [Nhóm 5] Định dạng Markdown & đóng gói Ebook tương tác
```

---

## 🚀 Hướng Dẫn Cài Đặt & Sử Dụng

### 1. Dành cho Google Antigravity IDE
* Sao chép toàn bộ các thư mục trong `skills/` vào thư mục `.agents/skills/` trong workspace của bạn:
  ```bash
  cp -r skills/* /path/to/your/workspace/.agents/skills/
  ```
* Antigravity IDE sẽ tự động kích hoạt các skill tương ứng khi bạn nhập câu lệnh yêu cầu biên soạn bài giảng.

### 2. Dành cho Anthropic Claude (Claude Projects)
* Nạp tệp `skills/pmr-ebook-master/SKILL.md` và các skill bạn quan tâm vào phần **Project Knowledge**.
* Thêm hướng dẫn vào System Prompt: *"Bạn là chuyên gia sư phạm y khoa PM&R tuân thủ các quy tắc trong Project Knowledge"*.

### 3. Dành cho OpenAI Codex / Custom GPTs
* Nén thư mục `skills/` và tải lên phần **Knowledge** của Custom GPT.
* Cấu hình phần Instructions tham chiếu đến quy trình trong `pmr-ebook-master`.

---

## 📄 Bản Quyền & Giấy Phép
Dự án được phân phối dưới giấy phép mã nguồn mở **MIT License**.
