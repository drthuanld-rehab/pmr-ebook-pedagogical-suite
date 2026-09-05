# Kiến Trúc Hệ Thống: PM&R Pedagogical Skill Suite

Bộ SKILL này được thiết kế theo chuẩn **Universal Markdown Architecture (UMA)**, cho phép hoạt động tương thích chéo 100% trên cả 3 nền tảng trợ lý AI hàng đầu hiện nay:

1. **Google Antigravity IDE:** 
   - Đặt trong `.agents/skills/<skill_name>/SKILL.md`.
   - Được nạp tự động qua cơ chế *Progressive Disclosure* dựa trên trường `description` trong YAML frontmatter.
2. **Anthropic Claude (Claude Projects & Claude Skills):**
   - Đọc trực tiếp tệp `SKILL.md` làm Project Instructions hoặc System Knowledge.
   - Nhận diện cực kỳ nhạy bén các thẻ định hướng quy trình và các khối Alert.
3. **OpenAI Codex / ChatGPT (Custom GPTs):**
   - Nạp các tệp `SKILL.md` vào Knowledge Base hoặc cấu hình vào System Instructions.

---

## 5 Nhóm Chức Năng Sư Phạm

```
                                [pmr-ebook-master] (Nhạc trưởng)
                                        │
    ┌───────────────────┬───────────────┴───────────────┬───────────────────┐
    ▼                   ▼                               ▼                   ▼
[1. CURRICULUM]    [2. SCIENCE-EBM]             [3. CLINICAL-AUTHOR]   [4. SAFETY & LAW]
├── matrix-designer ├── biophysics-explainer     ├── anchor-case-author ├── moh-legal-checker
└── icf-core-mapper └── pedro-ebm-verifier       ├── prescription-build └── safety-redflag-guard
                                                 └── postgrad-deepdive
                                                        │
                                                        ▼
                                              [5. EBOOK-ENGINEERING]
                                              ├── algorithm-generator
                                              ├── assessment-generator
                                              └── ebook-packager
```
