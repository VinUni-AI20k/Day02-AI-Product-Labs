# Deliverable Example — Tổng hợp báo cáo tuần

> Ví dụ bài nộp hoàn chỉnh từ đầu đến cuối lab. Đọc trước buổi học để hiểu output mỗi phase trông như thế nào.
> Kết luận cuối cùng **không phải lúc nào cũng là Agent** — đôi khi Rule đủ, đôi khi LLM chỉ cần hỗ trợ 1 bước. **Problem First, not AI First.**

---

## Context: Tôi là ai?

Tôi là **Minh**, 26 tuổi, Junior Product Manager tại một công ty SaaS ~50 người. Mỗi tuần tôi phải:

- Tổng hợp số liệu từ nhiều nguồn (Google Sheets, Jira, Slack)
- Viết "Weekly Report" gửi cho Engineering Manager + CEO
- Theo dõi OKR tiến độ sprint

Ngoài ra tôi còn review PRD, họp daily standup, sync cross-team. Bài toán tôi mang vào lab hôm nay đến từ chính công việc hàng ngày.

---

## Phase 1 — SCAN: Tìm kiếm cơ hội

Dùng **4 Lenses** để quét. Ghi mọi thứ, không filter.

| #  | Lens               | Bài toán                                                               |
|----|--------------------|------------------------------------------------------------------------|
| 1  | Lặp lại            | Mỗi thứ Hai tổng hợp Weekly Report từ 4 nguồn dữ liệu                |
| 2  | Lặp lại            | Copy-paste sprint velocity từ Jira vào Slides mỗi tuần                |
| 3  | Tốn thời gian      | Review 10-15 trang PRD mỗi tuần, mất 45 phút/bản để hiểu context     |
| 4  | Tốn thời gian      | Viết meeting notes sau mỗi buổi họp cross-team (30 min/buổi)          |
| 5  | AI có thể tốt hơn  | App quản lý task (Notion) không gợi ý priority dựa trên deadline       |
| 6  | AI có thể tốt hơn  | Slack search quá tệ — tìm quyết định cũ mất 10-15 phút              |
| 7  | Pain từ người khác  | Designer phàn nàn: spec từ PM mập mờ, phải hỏi lại 2-3 lần           |
| 8  | Pain từ người khác  | CEO hỏi: "Tuần này team làm gì?" mà report chưa sẵn thì không trả lời được |
| 9  | Tốn thời gian      | Mỗi tháng tổng hợp monthly KPI từ 3 dashboard khác nhau               |
| 10 | Lặp lại            | Gửi standup update trên Slack mỗi sáng — cùng format, copy-paste     |

**Tổng:** 10 bài toán. Yêu cầu tối thiểu 8 — đạt.

---

## Phase 2 — QUICK-ASSESS: 3 Quick Problem Cards

Chọn top 3 từ list: **#1 (Weekly Report)**, **#3 (Review PRD)**, **#6 (Slack search)**.

### Card #1 — Tổng hợp Weekly Report

```
┌──────────────────────────────────────────────────┐
│ QUICK PROBLEM CARD #1                            │
│                                                  │
│ Bài toán: Mỗi thứ Hai tổng hợp Weekly Report    │
│ từ 4 nguồn, mất 90 phút, hay bị muộn deadline   │
│                                                  │
│ Ai đang đau? PM (tôi), CEO (chờ report)          │
│                                                  │
│ Workflow hiện tại:                                │
│   1. Mở Jira export data                         │
│   → 2. Mở Google Sheets lấy metrics              │
│   → 3. Đọc Slack recap tuần                      │
│   → 4. Viết narrative trong Google Docs           │
│   → 5. Gửi email cho stakeholders                │
│                                                  │
│ Bước nào tốn nhất? Bước 4 (⏱ 40 min/lần)       │
│                                                  │
│ AI có thể giúp ở bước nào? Bước 3-4              │
│ (tổng hợp thông tin + draft narrative)            │
│                                                  │
│ Đo thành công bằng gì?                           │
│ Giảm tổng thời gian từ 90 min → dưới 30 min     │
│                                                  │
│ Quick gut: ☑ LLM Feature                         │
└──────────────────────────────────────────────────┘
```

### Card #2 — Review PRD

```
┌──────────────────────────────────────────────────┐
│ QUICK PROBLEM CARD #2                            │
│                                                  │
│ Bài toán: Review PRD mất 45 min/bản vì phải     │
│ đọc hết 10-15 trang để hiểu context trước khi   │
│ comment                                          │
│                                                  │
│ Ai đang đau? PM reviewer, Design lead            │
│                                                  │
│ Workflow hiện tại:                                │
│   1. Nhận PRD link → 2. Đọc toàn bộ             │
│   → 3. Ghi chú câu hỏi → 4. Comment trên doc   │
│                                                  │
│ Bước nào tốn nhất? Bước 2 (⏱ 30 min/lần)       │
│                                                  │
│ AI có thể giúp ở bước nào? Bước 2               │
│ (tóm tắt + highlight gaps)                       │
│                                                  │
│ Đo thành công bằng gì?                           │
│ Giảm thời gian review từ 45 min → 20 min        │
│                                                  │
│ Quick gut: ☑ LLM Feature                         │
└──────────────────────────────────────────────────┘
```

### Card #3 — Slack Search

```
┌──────────────────────────────────────────────────┐
│ QUICK PROBLEM CARD #3                            │
│                                                  │
│ Bài toán: Tìm quyết định cũ trên Slack mất      │
│ 10-15 phút, nhiều khi không tìm được             │
│                                                  │
│ Ai đang đau? Tất cả thành viên team (~12 người) │
│                                                  │
│ Workflow hiện tại:                                │
│   1. Nhớ keyword → 2. Search Slack               │
│   → 3. Scroll kết quả → 4. Đọc thread           │
│   → 5. Xác nhận đúng context                     │
│                                                  │
│ Bước nào tốn nhất? Bước 3-4 (⏱ 10 min/lần)     │
│                                                  │
│ AI có thể giúp ở bước nào? Chưa rõ —            │
│ cần index Slack history trước                     │
│                                                  │
│ Đo thành công bằng gì?                           │
│ Tìm đúng quyết định trong < 2 phút              │
│                                                  │
│ Quick gut: ☑ Agent (cần RAG pipeline)            │
└──────────────────────────────────────────────────┘
```

---

## Phase 3 — PITCH-CHALLENGE-VOTE

### Minh pitch Card #1 cho nhóm (2 min)

Minh giơ card lên: *"Mỗi thứ Hai tôi mất 90 phút tổng hợp report từ Jira + Sheets + Slack. Bước viết narrative tốn nhất — 25 phút — vì phải tự tìm insight từ raw data."*

### Nhóm challenge (3 min)

| Câu challenge | Trả lời của Minh |
|---------------|-----------------|
| "Rule/script đủ chưa? Có thật sự cần AI không?" | "Thu thập data (bước 1-3) thì script đủ. Nhưng viết narrative cần diễn đạt tự nhiên, thay đổi mỗi tuần — rule không đủ." |
| "Ngoài bạn, ai đau nữa? Bao nhiêu người?" | "Team có 3 PM, tất cả đều viết report kiểu này mỗi tuần." |
| "Metric đo được không? Có số cụ thể chưa?" | "Có — từ 90 min xuống dưới 30 min. Và tỉ lệ trễ deadline từ 30% xuống 5%." |

### Vote kết quả

Sau khi cả nhóm (4 người) pitch xong: **3/4 phiếu bầu cho Card #1** → chọn đi tiếp.

### Cards bị loại

| Card bị loại         | Lý do                                                                                 |
|----------------------|---------------------------------------------------------------------------------------|
| #2 — Review PRD     | Impact hẹp (chỉ 2-3 người review), khó đo quality improvement, metric mơ hồ           |
| #3 — Slack Search   | Cần xây RAG pipeline + index toàn bộ Slack → scope quá lớn cho lab, data access khó  |

### Card được chọn: **#1 — Tổng hợp Weekly Report**

**Vì sao:**
- **Frequency** cao: xảy ra mỗi tuần, mọi PM đều gặp
- **Impact** đo được: 90 min/tuần = ~78 giờ/năm cho 1 người
- **Vẽ flow được:** workflow rõ ràng, có input/output cụ thể
- **AI-likely:** tổng hợp text + số liệu là thế mạnh LLM

---

## Phase 4 — DEEP-DIVE

### 4.1 — Current-State Workflow

```
┌─────────────┐     ┌─────────────┐     ┌──────────────┐     ┌──────────────────┐
│ Bước 1      │     │ Bước 2      │     │ Bước 3       │     │ Bước 4           │
│ Export Jira │     │ Lấy metrics │     │ Đọc Slack    │     │ Tổng hợp vào     │
│ sprint data │     │ từ Google   │     │ recap tuần   │     │ Google Docs      │
│             │ ──→ │ Sheets      │ ──→ │              │ ──→ │                  │
│ Ai: PM      │     │ Ai: PM      │     │ Ai: PM       │     │ Ai: PM           │
│ ⏱ 10 min    │     │ ⏱ 10 min    │     │ ⏱ 15 min     │     │ ⏱ 15 min         │
│ In: Jira    │     │ In: Sheets  │     │ In: 3-5 Slack│     │ In: raw data     │
│ Out: CSV/   │     │ Out: bảng   │     │   channels   │     │   từ bước 1-3    │
│   screenshot│     │   số liệu   │     │ Out: bullet  │     │ Out: draft bảng  │
│             │     │             │     │   points     │     │   tổng hợp       │
└─────────────┘     └─────────────┘     └──────────────┘     └──────────────────┘
                                                                      │
        ┌─────────────────────────────────────────────────────────────┘
        ▼
┌──────────────────┐     ┌──────────────────┐     ┌─────────────┐
│ Bước 5           │     │ Bước 6           │     │ Bước 7      │
│ Viết narrative   │     │ Self-review +    │     │ Gửi email   │
│ (phân tích,      │     │ format           │     │ cho CEO +   │
│  highlight,      │ ──→ │                  │ ──→ │ EM          │
│  action items)   │     │ Ai: PM           │     │             │
│                  │     │ ⏱ 10 min         │     │ Ai: PM      │
│ Ai: PM           │     │ In: draft report │     │ ⏱ 5 min     │
│ ⏱ 25 min 🔴     │     │ Out: final       │     │ In: final   │
│ In: bảng tổng hợp│     │   report         │     │ Out: email  │
│ Out: narrative   │     │                  │     │   sent      │
│   paragraphs     │     │                  │     │             │
└──────────────────┘     └──────────────────┘     └─────────────┘

🔴 = Bottleneck (Bước 5: viết narrative tốn 25 min, hay bị writer's block)
🔄 = Handoff: Bước 4 → 5 (chuyển từ thu thập sang phân tích)
⏱  Tổng thời gian: 90 min/lần
```

**Ghi chú bottleneck:**
- Bước 5 chiếm **28% tổng thời gian** (25/90 min)
- Đây là bước sáng tạo nhất — phải nhìn dữ liệu, tìm insight, viết thành narrative có logic
- Hay bị "blank page syndrome": nhìn data mà không biết bắt đầu từ đâu
- Bước 1-3 cũng tốn thời gian (35 min) nhưng là công việc cơ học, ít lỗi

### 4.2 — Problem Statement (6-field)

| Field                    | Nội dung                                                                                                |
|--------------------------|---------------------------------------------------------------------------------------------------------|
| **Actor / Operator**     | Junior PM tại công ty SaaS 50 người, chịu trách nhiệm weekly report cho leadership                     |
| **Current Workflow**     | Mỗi thứ Hai: export Jira → lấy metrics từ Sheets → đọc Slack recap → tổng hợp → viết narrative → review → gửi email. 7 bước, 90 phút, hoàn toàn thủ công |
| **Bottleneck**           | Bước "viết narrative" mất 25 phút vì phải tự phân tích trend từ raw data, diễn đạt lại thành insight cho leadership đọc nhanh. Thường xuyên bị trễ deadline 10h sáng thứ Hai |
| **Impact**               | 90 phút/tuần = ~78 giờ/năm cho 1 PM. Team có 3 PM → ~234 giờ/năm. CEO nhận report muộn → thiếu context cho Monday standup. 30% tuần report bị trễ deadline |
| **Success Metric**       | Giảm tổng thời gian từ 90 min xuống dưới 30 min. Tỉ lệ trễ deadline giảm từ 30% xuống dưới 5%. Chất lượng narrative không giảm (đo bằng CEO satisfaction: giữ nguyên hoặc tăng) |
| **Operational Boundary** | AI được phép: draft narrative từ data có sẵn, gợi ý trend/insight. AI KHÔNG được phép: tự gửi report mà PM chưa review, bịa số liệu, access data ngoài 3 nguồn đã chỉ định. Human-in-the-loop: PM phải đọc và approve draft trước khi gửi |

### Sub-goals Decomposition

**Sub-goals user phải giải TRƯỚC khi dùng AI solution:**
- PM phải set up API connection tới Jira, Sheets, Slack (1 lần duy nhất)
- PM phải tạo prompt template mô tả format report CEO muốn nhận

**Sub-goals user phải giải TRONG KHI dùng AI solution:**
- PM phải review AI draft để catch số liệu sai hoặc insight thiếu context
- PM phải quyết định giữ/bỏ/sửa từng section AI generate

Các sub-goals này **nhất quán** với primary goal vì: tất cả đều hướng đến giảm thời gian tổng hợp report mà vẫn giữ chất lượng — setup 1 lần giúp tiết kiệm lâu dài, review đảm bảo output đáng tin.

### Metrics — 2 metric có ngưỡng

| Loại                          | Metric                           | Ngưỡng                        |
|-------------------------------|----------------------------------|--------------------------------|
| Efficiency (thời gian)        | Tổng thời gian làm weekly report | Từ 90 min → dưới 30 min       |
| Quality (chất lượng output)   | Tỉ lệ CEO yêu cầu sửa/hỏi thêm sau khi nhận report | Không tăng quá mức hiện tại (hiện ~10% tuần phải sửa) |

### 4.3 — Research

**Existing solution: Recapped.io**

| Field       | Nội dung                                                     |
|-------------|--------------------------------------------------------------|
| Tên         | Recapped.io / fellow.app / weekly report templates (Notion)  |
| Approach    | Template-based: tạo sẵn format, auto-pull data từ integrations |
| Điểm mạnh   | Giảm thời gian format, có sẵn integrations với Jira/Slack   |
| Điểm yếu    | Không viết narrative/insight — vẫn phải tự phân tích. Chỉ giải quyết bước 1-4 (thu thập), không giải quyết bước 5 (viết) |

**Case study: "How Stripe uses AI for internal reporting" (blog post)**

| Field       | Nội dung                                                     |
|-------------|--------------------------------------------------------------|
| Nguồn       | Blog post từ Lenny's Newsletter, 2024                         |
| Họ làm gì   | Dùng LLM để generate weekly summary từ structured data, PM review + edit trước khi gửi |
| Kết quả     | Giảm 60% thời gian viết report, adoption rate 70% sau 3 tháng |
| Bài học     | Human review vẫn cần thiết — LLM hallucinate insight nếu data không đủ context. Quan trọng nhất là structured input → LLM output tốt hơn |

**Bài học rút ra:** Bài toán này đã có người giải, nhưng phần lớn tool chỉ giải "thu thập data" chứ không giải "viết narrative." LLM có thể giúp ở đúng bottleneck (bước 5), nhưng cần structured input và human review.

### 4.4 — Future-State Flow

**Trước khi vẽ — 3 câu hỏi:**

**1. AI Fit Check (dùng AI-Fit Matrix):**

|                         | Ambiguity thấp        | Ambiguity cao     |
|-------------------------|-----------------------|-------------------|
| **Complexity thấp**     | Rule/workflow đủ      | LLM feature       |
| **Complexity cao**      | Workflow + automation  | Agent (cẩn thận!) |

Bài toán nằm ở: **Complexity thấp + Ambiguity cao → LLM Feature**
- Complexity thấp: workflow rõ ràng, input/output xác định, 1 người làm
- Ambiguity cao: narrative cần diễn đạt tự nhiên, insight phụ thuộc context tuần

**2. AI Suitability Check:**

| AI có lẽ PHÙ HỢP khi... | AI có lẽ KHÔNG phù hợp khi... |
|---|---|
| □ Cần personalization theo từng user | ☑ Cần kết quả predictable, nhất quán 100% |
| □ Cần prediction/dự đoán tương lai | □ Chi phí chạy AI quá cao cho tần suất cần |
| □ Scale lớn, không liệt kê hết được | □ Sai = hậu quả nghiêm trọng, không chấp nhận được |
| ☑ Cần xử lý ngôn ngữ tự nhiên | □ User không muốn bước này bị tự động hoá |
| ☑ Output đa dạng tốt hơn cố định | □ Cần giải thích 100% logic cho stakeholder |

Bài toán tick bên nào nhiều hơn? → **PHÙ HỢP (2-1)**. Narrative cần NLP + output đa dạng mỗi tuần. Duy nhất 1 tick "không phù hợp" vì CEO muốn format nhất quán — nhưng PM review sẽ đảm bảo.

**3. UX Check:** "PM recover thế nào khi AI draft sai?"
- PM đọc draft, thấy sai → sửa trực tiếp trên Google Docs. Flow recover giống hệt flow hiện tại (tự viết), chỉ mất thêm vài phút.
- Worst case: AI draft quá tệ → PM bỏ draft, tự viết lại. Tốn thêm ~5 phút so với không dùng AI.

**Future-State Flow:**

```
┌─────────────┐     ┌──────────────────┐     ┌──────────────────┐
│ Bước 1      │     │ Bước 2           │     │ Bước 3           │
│ 🔵 AUTO-    │     │ 🔵 AI tổng hợp  │     │ 🔵 AI draft      │
│ PULL data   │     │ raw data thành   │     │ narrative +      │
│ từ Jira +   │ ──→ │ bảng structured  │ ──→ │ highlight trends │
│ Sheets +    │     │                  │     │                  │
│ Slack API   │     │ ⏱ 1 min (auto)   │     │ ⏱ 1 min (auto)   │
│             │     │ In: raw data     │     │ In: structured   │
│ ⏱ 2 min     │     │ Out: structured  │     │   data           │
│ (config 1   │     │   summary table  │     │ Out: draft       │
│  lần đầu)   │     │                  │     │   narrative      │
└─────────────┘     └──────────────────┘     └──────────────────┘
                                                      │
        ┌─────────────────────────────────────────────┘
        ▼
┌──────────────────┐     ┌─────────────┐
│ Bước 4           │     │ Bước 5      │
│ 🟢 PM REVIEW     │     │ 🟢 PM gửi  │
│ + EDIT draft     │     │ email       │
│                  │     │             │
│ Ai: PM (human)   │ ──→ │ Ai: PM      │
│ ⏱ 15 min         │     │ ⏱ 2 min     │
│ In: AI draft     │     │ In: final   │
│ Out: approved    │     │ Out: sent   │
│   report         │     │             │
│ 🔴 BOUNDARY:     │     │             │
│ Phải approve     │     │             │
│ trước khi gửi   │     │             │
└──────────────────┘     └─────────────┘

Ký hiệu:
🔵 = AI xử lý
🟢 = Human quyết định
🔴 = Boundary (AI không được vượt)

Fallback: Nếu AI draft kém → PM tự viết lại (quay về flow cũ bước 5-6)

⏱ Tổng thời gian mới: ~21 min (giảm từ 90 min)
   Trong đó PM thực sự làm: ~17 min (review + gửi)
```

**So sánh:**

| Tiêu chí         | Hiện tại | Tương lai | Thay đổi     |
|-------------------|----------|-----------|--------------|
| Tổng thời gian    | 90 min   | ~21 min   | -77% (giảm 69 min) |
| Bước thủ công     | 7/7      | 2/5       | PM chỉ review + gửi |
| Bottleneck mới    | —       | Bước 4: review (15 min) | Chấp nhận được — đây là human judgment |

### AI Fit Decision

Chốt: **LLM Feature** (AI hỗ trợ 1-2 bước cụ thể)

**Summary:**
Nhóm cho rằng AI **có thể** giải quyết bài toán **tổng hợp + viết narrative cho weekly report**,
vì **generate text từ structured data là thế mạnh LLM, workflow tuyến tính không cần Agent, và human-in-the-loop đã có sẵn (PM review trước khi gửi).**

**Chi tiết:**
1. Rule/workflow không đủ vì narrative cần diễn đạt tự nhiên, tìm trend, viết khác nhau mỗi tuần.
2. Không cần Agent vì workflow tuyến tính, không có branching logic phức tạp.
3. Bước auto-pull data (bước 1) chỉ cần Rule/Automation (Zapier, script) — chỉ bước 2-3 cần LLM.

**Kết luận: Đây là bài toán "Boost" — AI tăng tốc cho con người, không thay thế con người.**

### Underspecification Check

| Điều chưa rõ | Nếu không chỉ rõ → hậu quả gì? | Cách tìm ra? |
|---|---|---|
| "Narrative đủ tốt" nghĩa là gì? Edit nhẹ (< 15 min) hay viết lại? | PM vẫn mất 25 min viết lại → không tiết kiệm gì | Pilot 2 tuần: đo thời gian edit thực tế |
| CEO đọc narrative hay chỉ nhìn bảng số? | Nếu chỉ nhìn số → template đủ, không cần LLM | Hỏi trực tiếp CEO: "Anh đọc phần nào trước?" |
| Jira/Sheets/Slack có API accessible không? | Không kết nối được → phải copy-paste thủ công | Check permission với IT team trước khi build |

---

## Phase 5 — EVALUATE

### AI Readiness Checklist

| #  | Câu hỏi                                                         | Yes/No | Ghi chú                                                       |
|----|------------------------------------------------------------------|--------|----------------------------------------------------------------|
| 1  | Có data/input đủ chất lượng và số lượng?                         | Yes    | Jira, Sheets, Slack đều có structured data, cập nhật realtime  |
| 2  | Có metric rõ ràng để đo thành/bại?                               | Yes    | Thời gian (90→30 min) + tỉ lệ trễ (30→5%) + CEO satisfaction  |
| 3  | Sai thì hậu quả có chấp nhận được không?                        | Yes    | Report sai → PM catch khi review. Worst case: gửi muộn 15 min |
| 4  | User sẵn sàng dùng AI trong workflow này không?                  | Yes    | PM (tôi) rất muốn giảm thời gian. Không có compliance blocker |
| 5  | Có resource (người, tiền, thời gian) để maintain không?          | Not Yet | Cần dev set up API integration + prompt engineering. Hiện chưa có dev resource rảnh |

**Kết quả: 4 Yes, 1 Not Yet.**

### Optimization Check

AI solution có thể mang lại:
- PM tiết kiệm ~60 min/tuần, report đến tay CEO đúng giờ
- Narrative nhất quán hơn vì LLM không bị "blank page syndrome"

Nhưng nếu AI optimize sai hướng thì sao?
- AI chỉ tóm tắt data mà không highlight trend quan trọng → CEO đọc report thấy "nhàn nhạt", mất trust
- AI generate insight không có trong data (hallucination) → PM không catch khi review → gửi số sai cho leadership

### Quyết định: **Go (với scope nhỏ)**

**Justify:**

Bài toán có đủ 4/5 điều kiện. Điều kiện thiếu (dev resource) có thể giải quyết bằng cách chia scope:

- **Tuần 1-2 (không cần dev):** Dùng ChatGPT/Claude trực tiếp. Copy-paste raw data vào prompt, nhận draft narrative, edit và gửi. Đây là pilot "manual AI" để validate assumption #2 (LLM có draft đủ tốt không?).
- **Tháng 2 (cần dev):** Nếu pilot thành công, xin dev resource để build automation (API pull + LLM generate + Google Docs output).

**Nếu pilot cho thấy LLM draft quá tệ (PM phải viết lại > 50%)** → quay về Not Yet, cần tìm approach khác hoặc chấp nhận dùng template + automation (Rule level) thay vì LLM.

---

## Reflection Log

Trong quá trình làm lab, tôi đã dùng AI (ChatGPT) ở các bước sau:

| Câu hỏi                                         | Trả lời                                                                                              |
|--------------------------------------------------|-------------------------------------------------------------------------------------------------------|
| **AI giúp gì?**                                  | Research: tìm Recapped.io và case study Stripe. Brainstorm: gợi ý thêm 3 problems cho Phase 1 SCAN   |
| **AI sai hoặc hời hợt ở đâu?**                  | Khi hỏi "viết Problem Statement cho tôi", AI viết quá chung chung, không có con số cụ thể. Metric ban đầu AI gợi ý là "nhanh hơn" — vô nghĩa |
| **Tôi phải sửa gì bằng tay?**                   | Tự đo thời gian thật (90 min) bằng cách time chính mình 1 tuần. Tự hỏi CEO "anh có đọc narrative không?" để validate assumption. Sửa PS thêm số liệu cụ thể |
| **Prompt hay nhất?**                             | "Tôi mất 90 phút mỗi thứ Hai để viết weekly report từ Jira + Sheets + Slack. Hãy phân tích workflow này thành 5-8 bước, ghi thời gian mỗi bước, và chỉ ra bước nào là bottleneck lớn nhất. Giải thích vì sao." |

---

## Tổng kết: Bài học từ ví dụ này

| Bài học                          | Chi tiết                                                                       |
|----------------------------------|--------------------------------------------------------------------------------|
| **Problem First, not AI First**  | Tôi không bắt đầu bằng "dùng AI gì?" mà bắt đầu bằng "tôi đau ở đâu?"       |
| **Rule cũng là giải pháp**       | Bước auto-pull data chỉ cần Zapier/script, không cần LLM. Đừng overengineer   |
| **Kill Cards là tốt**           | Slack Search bị kill vì scope quá lớn — đó là quyết định đúng, không phải thất bại |
| **Số liệu thật quan trọng**     | "90 phút" và "30% trễ deadline" mạnh hơn "mất nhiều thời gian"                |
| **AI là Boost, không phải Replace** | PM vẫn review, vẫn quyết định gửi. AI chỉ giúp draft nhanh hơn              |
| **Pilot trước, build sau**       | Dùng ChatGPT trực tiếp 2 tuần trước khi xin dev resource — rẻ và nhanh      |

---

## Hướng dẫn nộp bài

### File nộp

```
HoTen-day02.zip                       ← Ví dụ: NguyenVanMinh-day02.zip
├── 01-problem-scan.md                ← 5+ bài toán qua 4 Lenses + 3 Quick Cards + kill rationale
├── 02-deep-dive-report.md            ← Workflow + PS 6-field + metrics + research + AI fit + Go/No-Go
├── 03-reflection-log.md              ← AI giúp gì, sai gì, nhóm sửa gì
└── extras/                           ← Không bắt buộc
    ├── research-notes.md
    ├── screenshots/
    └── ...
```

### Lưu ý

- **Mỗi người nộp 1 zip riêng** — kể cả file nhóm (02) cũng nộp trong zip cá nhân
- **Tên file zip**: `HoTen-day02.zip` (không dấu, không khoảng trắng)
- **File 01 và 03**: mỗi người viết riêng
- **File 02**: cả nhóm viết chung — giống nhau trong zip của mọi thành viên
- **extras/**: tùy chọn — nộp thêm ghi chú, screenshot AI conversation, hoặc tài liệu bổ sung
