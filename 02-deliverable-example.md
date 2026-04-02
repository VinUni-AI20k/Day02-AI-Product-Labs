# Deliverable Example — Tổng hợp báo cáo tuần (v2 theo rubric mới)

> Ví dụ bài nộp hoàn chỉnh từ đầu đến cuối lab, đã được chỉnh lại để **khớp với metric/rubric mới**:
> - tách rõ phần nào là **cá nhân**
> - phần nào là **nhóm**
> - vì sao bài này đạt mức **Hiểu đầy đủ / gần Xuất sắc**
>
> Mục tiêu của file này không phải để học viên “copy”, mà để:
> 1. thấy output tốt trông như thế nào,
> 2. hiểu **điểm sẽ được chấm ở đâu**,
> 3. phân biệt bài làm “đủ dùng” với bài làm “thật sự chặt”.

---

## Cách đọc file ví dụ này

Trong rubric mới, điểm được chia theo hướng:

- **Điểm cá nhân (40%)**
  - Scan breadth + Quick Problem Cards
  - Pitch + Challenge participation
  - AI Support Log + Reflection
  - Individual understanding check
- **Điểm nhóm (60%)**
  - Workflow Mapping
  - Problem Statement + Metrics + Boundary
  - AI Fit + Alternatives + Future Flow
  - Decision Quality

Vì vậy, trong file ví dụ này sẽ có 2 loại note:

- **[INDIVIDUAL SIGNAL]** = tín hiệu giúp học viên lấy điểm cá nhân
- **[GROUP SIGNAL]** = tín hiệu giúp nhóm lấy điểm chung

---

## Context: Tôi là ai?

Tôi là **Minh**, 26 tuổi, Junior Product Manager tại một công ty SaaS ~50 người. Mỗi tuần tôi phải:

- Tổng hợp số liệu từ nhiều nguồn (Google Sheets, Jira, Slack)
- Viết "Weekly Report" gửi cho Engineering Manager + CEO
- Theo dõi OKR tiến độ sprint

Ngoài ra tôi còn review PRD, họp daily standup, sync cross-team. Bài toán tôi mang vào lab hôm nay đến từ chính công việc hàng ngày.

**Vì sao context này tốt cho lab?**
- Có actor rõ
- Có workflow thật
- Có pain lặp lại
- Có metric đo được
- Không quá rộng

**[INDIVIDUAL SIGNAL]** Một bài toán tốt thường đến từ trải nghiệm thật, không phải ý tưởng “nghe hay”.
**[GROUP SIGNAL]** Một nhóm dễ deep-dive tốt hơn khi chọn bài toán mà ít nhất 1 người hiểu workflow thật.

---

# Phase 1 — SCAN: Tìm kiếm cơ hội

Dùng **4 Lenses** để quét. Ghi mọi thứ, không filter.

| #  | Lens               | Bài toán |
|----|--------------------|----------|
| 1  | Lặp lại            | Mỗi thứ Hai tổng hợp Weekly Report từ 4 nguồn dữ liệu |
| 2  | Lặp lại            | Copy-paste sprint velocity từ Jira vào Slides mỗi tuần |
| 3  | Tốn thời gian      | Review 10-15 trang PRD mỗi tuần, mất 45 phút/bản để hiểu context |
| 4  | Tốn thời gian      | Viết meeting notes sau mỗi buổi họp cross-team (30 min/buổi) |
| 5  | AI có thể tốt hơn  | App quản lý task (Notion) không gợi ý priority dựa trên deadline |
| 6  | AI có thể tốt hơn  | Slack search quá tệ — tìm quyết định cũ mất 10-15 phút |
| 7  | Pain từ người khác | Designer phàn nàn: spec từ PM mập mờ, phải hỏi lại 2-3 lần |
| 8  | Pain từ người khác | CEO hỏi: "Tuần này team làm gì?" mà report chưa sẵn thì không trả lời được |
| 9  | Tốn thời gian      | Mỗi tháng tổng hợp monthly KPI từ 3 dashboard khác nhau |
| 10 | Lặp lại            | Gửi standup update trên Slack mỗi sáng — cùng format, copy-paste |

**Tổng:** 10 bài toán.

### Vì sao phần SCAN này đạt điểm cao
- Có **10 bài toán**, vượt ngưỡng tối thiểu
- Dùng đủ **4 lenses**
- Có bài toán từ bản thân và từ người khác
- Có breadth trước khi converge

**[INDIVIDUAL SIGNAL]**
Một bài scan mạnh không chỉ là “đủ 5 ý”, mà phải cho thấy:
- breadth,
- đa dạng lens,
- có pain thật,
- có khả năng chọn được 1 bài toán để đi tiếp.

**Nếu chỉ scan kiểu yếu**
- 5 ý quá giống nhau
- chỉ dùng 1 lens
- toàn ý tưởng solution-first như “làm chatbot cho trường”
→ thì thường chỉ đạt mức pass tối thiểu.

---

# Phase 2 — QUICK-ASSESS: 3 Quick Problem Cards

Chọn top 3 từ list:
- **#1 — Weekly Report**
- **#3 — Review PRD**
- **#6 — Slack Search**

## Card #1 — Tổng hợp Weekly Report

```text
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
│   → 4. Viết narrative trong Google Docs          │
│   → 5. Gửi email cho stakeholders                │
│                                                  │
│ Bước nào tốn nhất? Bước 4 (⏱ 40 min/lần)        │
│                                                  │
│ AI có thể giúp ở bước nào? Bước 3-4              │
│ (tổng hợp thông tin + draft narrative)           │
│                                                  │
│ Đo thành công bằng gì?                           │
│ Giảm tổng thời gian từ 90 min → dưới 30 min     │
│                                                  │
│ Quick gut: ☑ LLM Feature                         │
└──────────────────────────────────────────────────┘
```

## Card #2 — Review PRD

```text
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
│   → 3. Ghi chú câu hỏi → 4. Comment trên doc    │
│                                                  │
│ Bước nào tốn nhất? Bước 2 (⏱ 30 min/lần)        │
│                                                  │
│ AI có thể giúp ở bước nào? Bước 2               │
│ (tóm tắt + highlight gaps)                      │
│                                                  │
│ Đo thành công bằng gì?                           │
│ Giảm thời gian review từ 45 min → 20 min        │
│                                                  │
│ Quick gut: ☑ LLM Feature                         │
└──────────────────────────────────────────────────┘
```

## Card #3 — Slack Search

```text
┌──────────────────────────────────────────────────┐
│ QUICK PROBLEM CARD #3                            │
│                                                  │
│ Bài toán: Tìm quyết định cũ trên Slack mất      │
│ 10-15 phút, nhiều khi không tìm được             │
│                                                  │
│ Ai đang đau? Tất cả thành viên team (~12 người) │
│                                                  │
│ Workflow hiện tại:                                │
│   1. Nhớ keyword → 2. Search Slack              │
│   → 3. Scroll kết quả → 4. Đọc thread          │
│   → 5. Xác nhận đúng context                    │
│                                                  │
│ Bước nào tốn nhất? Bước 3-4 (⏱ 10 min/lần)      │
│                                                  │
│ AI có thể giúp ở bước nào? Chưa rõ —            │
│ cần index Slack history trước                    │
│                                                  │
│ Đo thành công bằng gì?                           │
│ Tìm đúng quyết định trong < 2 phút              │
│                                                  │
│ Quick gut: ☑ Agent (cần RAG pipeline)            │
└──────────────────────────────────────────────────┘
```

### Vì sao 3 cards này mạnh
- Mỗi card đều có:
  - actor,
  - flow ngắn,
  - bottleneck,
  - metric có số,
  - quick hypothesis về mức giải pháp
- Card #3 rất hay vì **không chắc AI giúp ở đâu** — đây là dấu hiệu trung thực, không phải điểm yếu

**[INDIVIDUAL SIGNAL]**
Đây là chỗ người chấm nhìn ra học viên có hiểu “metric có số” hay chưa.
Ví dụ tốt:
- “90 phút → dưới 30 phút”
- “< 2 phút”
Ví dụ yếu:
- “nhanh hơn”
- “tốt hơn”
- “đỡ mệt hơn”

---

# Phase 3 — PITCH-CHALLENGE-VOTE

## Minh pitch Card #1 cho nhóm

Minh nói ngắn gọn:
> “Mỗi thứ Hai tôi mất 90 phút tổng hợp report từ Jira + Sheets + Slack. Bước viết narrative tốn nhất vì phải tự tìm insight từ raw data. Nếu giải được bước này thì khả năng giảm hơn nửa thời gian.”

## Nhóm challenge

| Câu challenge | Trả lời của Minh |
|---------------|-----------------|
| “Rule/script đủ chưa? Có thật sự cần AI không?” | “Thu thập data ở bước 1-3 thì script đủ. Nhưng viết narrative cần diễn đạt tự nhiên, mỗi tuần khác nhau — rule không đủ.” |
| “Ngoài bạn, ai đau nữa? Bao nhiêu người?” | “Team có 3 PM, tất cả đều viết report kiểu này mỗi tuần.” |
| “Metric đo được không? Có số cụ thể chưa?” | “Có — từ 90 min xuống dưới 30 min. Và tỉ lệ trễ deadline từ 30% xuống 5%.” |

## Vote kết quả
Sau khi cả nhóm pitch xong: **3/4 phiếu cho Card #1**.

## Cards bị loại

| Card bị loại | Lý do |
|--------------|-------|
| #2 — Review PRD | Impact hẹp, khó đo quality improvement, metric yếu hơn |
| #3 — Slack Search | Scope quá lớn cho lab, data access khó, chưa rõ feasibility |

### Vì sao phần này quan trọng trong rubric mới
Đây là phần **NO-AI**, nên rất hữu ích để phân biệt:
- ai thật sự hiểu bài toán
- ai chỉ đi theo nhóm

**[INDIVIDUAL SIGNAL]**
Một học viên được chấm cao ở phần này khi:
- pitch rõ problem → workflow → bottleneck → metric
- trả lời challenge không lảng tránh
- chấp nhận kill card nếu hợp lý

**[GROUP SIGNAL]**
Một nhóm được chấm tốt khi:
- không chọn bài trivial
- không chọn bài “ngầu nhưng không làm nổi”
- có kill rationale rõ ràng

---

# Phase 4 — DEEP-DIVE

## 4.1 — Current-State Workflow

```text
┌─────────────┐     ┌─────────────┐     ┌──────────────┐     ┌──────────────────┐
│ Bước 1      │     │ Bước 2      │     │ Bước 3       │     │ Bước 4           │
│ Export Jira │     │ Lấy metrics │     │ Đọc Slack    │     │ Tổng hợp vào     │
│ sprint data │     │ từ Google   │     │ recap tuần   │     │ Google Docs      │
│             │ ──→ │ Sheets      │ ──→ │              │ ──→ │                  │
│ Ai: PM      │     │ Ai: PM      │     │ Ai: PM       │     │ Ai: PM           │
│ ⏱ 10 min    │     │ ⏱ 10 min    │     │ ⏱ 15 min     │     │ ⏱ 15 min         │
│ In: Jira    │     │ In: Sheets  │     │ In: 3-5 Slack│     │ In: raw data     │
│ Out: CSV    │     │ Out: bảng   │     │ Out: bullet  │     │ Out: draft bảng  │
└─────────────┘     └─────────────┘     └──────────────┘     └──────────────────┘
                                                                      │
                                                                      ▼
┌──────────────────┐     ┌──────────────────┐     ┌─────────────┐
│ Bước 5           │     │ Bước 6           │     │ Bước 7      │
│ Viết narrative   │     │ Self-review +    │     │ Gửi email   │
│ (phân tích,      │ ──→ │ format           │ ──→ │ cho CEO +   │
│ highlight,       │     │                  │     │ EM          │
│ action items)    │     │ Ai: PM           │     │ Ai: PM      │
│ Ai: PM           │     │ ⏱ 10 min         │     │ ⏱ 5 min     │
│ ⏱ 25 min 🔴     │     │                  │     │             │
└──────────────────┘     └──────────────────┘     └─────────────┘

🔴 = Bottleneck
⏱ Tổng thời gian: 90 min/lần
```

### Ghi chú bottleneck
- Bước 5 chiếm **28% tổng thời gian**
- Đây là bước sáng tạo nhất
- Hay bị “blank page syndrome”

### Vì sao workflow này đạt điểm cao
- Có đủ **7 bước**
- Có thời gian mỗi bước
- Có bottleneck rõ
- Có thể đọc và hiểu bởi người ngoài nhóm

**[GROUP SIGNAL]**
Một workflow mạnh không chỉ là “đẹp”, mà phải giúp kéo ra được:
- bottleneck thật
- impact thật
- nơi AI có thể chen vào
- nơi AI không nên chen vào

---

## 4.2 — Problem Statement (6-field)

| Field | Nội dung |
|-------|----------|
| **Actor / Operator** | Junior PM tại công ty SaaS 50 người, chịu trách nhiệm weekly report cho leadership |
| **Current Workflow** | Mỗi thứ Hai: export Jira → lấy metrics từ Sheets → đọc Slack recap → tổng hợp → viết narrative → review → gửi email. 7 bước, 90 phút, hoàn toàn thủ công |
| **Bottleneck** | Bước viết narrative mất 25 phút vì phải tự phân tích trend từ raw data, diễn đạt lại thành insight cho leadership đọc nhanh |
| **Impact** | 90 phút/tuần = ~78 giờ/năm cho 1 PM. Team có 3 PM → ~234 giờ/năm. 30% tuần report bị trễ deadline |
| **Success Metric** | Giảm tổng thời gian từ 90 phút xuống dưới 30 phút. Tỉ lệ trễ deadline từ 30% xuống dưới 5% |
| **Operational Boundary** | AI được phép draft narrative từ data có sẵn. AI không được tự gửi report, không được bịa số liệu, PM phải review trước khi gửi |

### Sub-goals Decomposition

**TRƯỚC khi dùng AI**
- Set up API connection tới Jira, Sheets, Slack
- Tạo prompt template đúng format report

**TRONG khi dùng AI**
- PM review AI draft để bắt lỗi
- PM quyết định giữ/bỏ/sửa từng section

### Metrics

| Loại | Metric | Ngưỡng |
|------|--------|--------|
| Efficiency | Tổng thời gian làm weekly report | 90 min → dưới 30 min |
| Quality | Tỉ lệ CEO yêu cầu sửa/hỏi thêm | Không tăng quá mức hiện tại |

### Vì sao PS này mạnh
- Cụ thể đúng **1 workflow**
- Có impact định lượng
- Có boundary rõ
- Metric có thể dùng để ra quyết định

**[GROUP SIGNAL]**
Đây là phần dễ kéo điểm nhóm lên hoặc kéo tụt mạnh nhất.
PS yếu thường có 3 lỗi:
1. scope quá rộng,
2. metric không có ngưỡng,
3. boundary không rõ.

---

## 4.3 — Research

### Existing solution
- **Recapped.io / fellow.app / weekly report templates**
- mạnh ở phần thu thập data
- yếu ở phần viết insight

### Case study
- **Stripe internal reporting**
- LLM generate summary từ structured data
- PM review trước khi gửi
- giảm 60% thời gian viết report

### Quick poll
- 2/3 PM ngoài nhóm nói họ cũng mất nhiều thời gian tương tự
- 1 người nói dùng template thì đỡ format, nhưng vẫn đau ở narrative

### Vì sao research này đạt điểm tốt
- Không chỉ tìm “tool”
- Có **existing solution**
- Có **case study**
- Có **quick poll**
- Có **bài học rút ra cho bài toán nhóm mình**

**[GROUP SIGNAL]**
Research tốt không phải là copy tên công cụ AI, mà là:
- biết trên thị trường đã có gì
- biết khoảng trống thật ở đâu
- biết vì sao nên buy / boost / build

---

## 4.4 — Future-State Flow + AI Fit

### AI Fit Check
Bài toán nằm ở:
**Complexity thấp + Ambiguity cao → LLM Feature**

### AI Suitability Check
Tick thiên về bên **phù hợp**, nhưng không tuyệt đối:
- cần NLP
- output đa dạng tốt hơn cố định
- vẫn có một điểm “không phù hợp” là cần output khá nhất quán

### UX Check
Nếu AI draft sai:
- PM sửa trực tiếp
- tệ nhất thì PM bỏ draft và viết lại

## Future-State Flow

```text
┌─────────────┐     ┌──────────────────┐     ┌──────────────────┐
│ Bước 1      │     │ Bước 2           │     │ Bước 3           │
│ 🔵 Auto-pull│ ──→ │ 🔵 AI tổng hợp  │ ──→ │ 🔵 AI draft      │
│ data        │     │ data             │     │ narrative        │
└─────────────┘     └──────────────────┘     └──────────────────┘
                                                      │
                                                      ▼
┌──────────────────┐     ┌─────────────┐
│ Bước 4           │     │ Bước 5      │
│ 🟢 PM review     │ ──→ │ 🟢 PM gửi   │
│ + edit           │     │ email       │
│ 🔴 Boundary:     │     │             │
│ phải approve     │     │             │
└──────────────────┘     └─────────────┘

➡️ Fallback: AI draft kém → PM tự viết lại
```

### AI Fit Decision
**Chốt: LLM Feature**

**Vì sao không phải Agent**
1. workflow tuyến tính
2. không cần planning nhiều bước động
3. chỉ một phần cần AI, phần còn lại script/rule đủ

### Underspecification Check

| Điều chưa rõ | Hậu quả | Cách tìm ra |
|---|---|---|
| “Narrative đủ tốt” nghĩa là gì? | PM vẫn phải viết lại gần hết | Pilot 2 tuần, đo thời gian edit |
| CEO đọc narrative hay chỉ nhìn bảng số? | Nếu chỉ nhìn số → không cần LLM | Hỏi trực tiếp CEO |
| API có truy cập được không? | Không build được automation | Check với IT |

### Vì sao phần này mạnh
- Không mặc định Agent
- Có so sánh alternatives
- Có fallback
- Có boundary
- Có thoughtfulness về unknowns

**[GROUP SIGNAL]**
Đây là khu vực phân biệt nhóm “hiểu khá” với nhóm “hiểu đầy đủ”.
Nhóm mạnh thường:
- nói rõ vì sao **chưa cần agent**
- chỉ ra được **fallback**
- viết được **underspecification** thay vì giả vờ mọi thứ đã rõ

---

# Phase 5 — EVALUATE

## AI Readiness Checklist

| # | Câu hỏi | Kết quả | Ghi chú |
|---|---------|---------|---------|
| 1 | Có data/input đủ chất lượng? | Yes | Jira, Sheets, Slack có data |
| 2 | Có metric rõ? | Yes | 90→30 min; 30%→5% |
| 3 | Sai thì hậu quả có chấp nhận được? | Yes | PM review được |
| 4 | User sẵn sàng dùng AI? | Yes | PM rất muốn giảm thời gian |
| 5 | Có resource để maintain? | Not Yet | Cần dev resource |

## Optimization Check

**Lợi ích**
- Tiết kiệm ~60 phút/tuần
- Report đến leadership đúng giờ hơn

**Rủi ro nếu optimize sai**
- AI summary nhàn nhạt, bỏ sót trend quan trọng
- AI hallucinate insight không có trong data

## Quyết định
**Go (với scope nhỏ)**

### Justify
- Có 4/5 điều kiện đủ
- có thể bắt đầu bằng pilot thủ công trước
- điều kiện thiếu là dev resource, không phải problem sai

### Nếu pilot thất bại
- quay về Not Yet
- hoặc hạ xuống Rule + template + automation

### Vì sao quyết định này tốt
Một quyết định tốt không nhất thiết phải “Go to production”.
Ở đây, quyết định tốt là:
- **Go nhưng scope nhỏ**
- biết điều gì cần validate trước
- có đường lui nếu assumption sai

**[GROUP SIGNAL]**
Đây là phần coach/người chấm nhìn vào để xác định nhóm có “trưởng thành” hay không.

---

# Phase 6 — AI Support Log

| Câu hỏi | Trả lời |
|---------|---------|
| AI giúp gì? | Research, brainstorm thêm 3 problems, digitize flow |
| AI sai ở đâu? | Viết PS quá chung, metric vô nghĩa kiểu “nhanh hơn” |
| Nhóm phải sửa gì bằng tay? | Tự đo thời gian thật, tự hỏi stakeholder, sửa số liệu và boundary |
| Prompt hay nhất? | “Hãy phân tích workflow này thành 5-8 bước, ghi thời gian mỗi bước, và chỉ ra bottleneck lớn nhất.” |

### Vì sao AI Support Log này tốt
- Không khoe dùng AI nhiều
- Không copy output AI
- Có honest reflection
- Chỉ rõ AI sai ở đâu và con người sửa gì

**[INDIVIDUAL SIGNAL]**
Đây là chỗ rất tốt để phân biệt:
- người học thật sự hiểu
- với người chỉ “nhờ AI làm hộ”

---

# Vì sao bài ví dụ này sẽ đạt điểm cao theo rubric mới

## Điểm cá nhân
Bài này mạnh ở:
- scan breadth tốt
- quick cards có metric cụ thể
- pitch/challenge trả lời được bằng evidence
- AI Support Log trung thực

## Điểm nhóm
Bài này mạnh ở:
- workflow rõ
- PS chặt
- AI fit không overclaim
- research có chiều sâu
- quyết định Go nhỏ, không liều

## Mức năng lực dự kiến
Bài này nên nằm ở mức:

**Hiểu đầy đủ** hoặc **gần Hiểu xuất sắc**

vì:
- problem framing rất rõ
- không solution-first
- biết chọn **LLM Feature** thay vì Agent
- có pilot thinking
- có fallback và unknowns

Nó chưa chắc tuyệt đối xuất sắc vì vẫn còn một số assumption cần validate thật ngoài lab, nhưng đó lại chính là điều làm bài này thực tế và đáng tin.

---

# Hướng dẫn nộp bài

```text
HoTen-day02.zip
├── 01-problem-scan.md
├── 02-deep-dive-report.md
├── 03-ai-log.md
├── 04-workflow-diagram.png/pdf
└── extras/
```

### Lưu ý
- Mỗi người nộp **1 zip riêng**
- File `01` và `03` là **cá nhân**
- File `02` và `04` là **nhóm**
- Có thể nộp thêm screenshot AI conversation trong `extras/`, nhưng **không bắt buộc**

---

# Chốt thông điệp

Một bài nộp mạnh của Ngày 2 **không phải** bài:
- nghe “agentic” nhất,
- hay phức tạp nhất.

Một bài nộp mạnh là bài:
- chọn đúng problem,
- vẽ đúng workflow,
- viết đúng metric,
- chọn đúng mức AI,
- và ra được quyết định trung thực.

**Problem first, not AI first.**
