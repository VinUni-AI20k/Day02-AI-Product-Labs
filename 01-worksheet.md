# Lab 2 — AI Opportunity Discovery Sprint (v2)
## Worksheet + Self-Check Metric chi tiết

**Mục tiêu của bản v2:** giữ nguyên flow lab cũ, nhưng bổ sung rõ hơn cách tự kiểm tra chất lượng bài làm và cách điểm **nhóm / cá nhân** sẽ được tính.

---

## 1. Cách tính điểm tổng quát

<<<<<<< HEAD:day-02/01-worksheet.md
### Tổng điểm: 100
- **Điểm nhóm:** 60
- **Điểm cá nhân:** 40

### Điểm nhóm (60 điểm)
| Gate | Điểm | Deliverable | Chấm cái gì |
|---|---:|---|---|
| G1. Workflow Mapping | 20 | Problem Deep-Dive | Flow hiện tại có đủ bước, bottleneck, thời gian, handoff |
| G2. Problem Statement + Metrics | 20 | Problem Deep-Dive | PS 6-field, metric có ngưỡng, boundary rõ |
| G3. AI Fit + Research + Future Flow | 10 | Problem Deep-Dive | So sánh mức giải pháp, research, future flow có AI/Human/Boundary/Fallback |
| G4. Decision Quality | 10 | Problem Deep-Dive | Go / Not Yet / No-Go có justify bằng evidence |

### Điểm cá nhân (40 điểm)
| Gate | Điểm | Deliverable | Chấm cái gì |
|---|---:|---|---|
| I1. Scan & Quick Cards | 15 | Scan & Filter Log | Breadth, 4 lenses, 3 cards đủ chất lượng |
| I2. Pitch + Challenge Participation | 10 | Quan sát Phase 3 | Pitch rõ, challenge đúng 3 câu chuẩn, có phản biện chất lượng |
| I3. AI Support Log + Reflection | 15 | AI Support Log | Honest reflection: AI giúp gì, sai gì, mình sửa gì, học gì |

> **Nguyên tắc:** Một nhóm mạnh không đủ để kéo tất cả thành viên lên điểm cao. Mỗi người phải chứng minh được phần tư duy cá nhân.
=======
1. **Xuất phát từ bản thân** — bài toán đến từ chính workflow, sản phẩm, công việc của bạn
2. **AI không thay bạn ra quyết định** — AI brainstorm/draft, bạn chọn/sửa/chốt
3. **"Không cần AI" vẫn là kết luận tốt** — điểm dựa trên chất lượng tư duy, không phải mức phức tạp
4. **Vẽ trước, viết sau** — flow vẽ tay trên giấy, không phải list text
5. **Bắt buộc có Reflection Log** — ghi lại AI giúp gì, sai gì, bạn sửa gì
>>>>>>> main:01-worksheet.md

---

## 2. Thang mức độ hiểu

| Mức | Điểm | Ý nghĩa |
|---|---:|---|
| **Không pass** | < 50 | Chưa nắm được problem-first, metric, boundary, hoặc gần như không đóng góp |
| **Vừa đủ pass** | 50–64 | Có làm được phần cơ bản nhưng còn mơ hồ, solution-first hoặc metric yếu |
| **Hiểu khá** | 65–79 | Logic tương đối rõ, có thể chọn bài toán và justify ở mức ổn |
| **Hiểu đầy đủ** | 80–89 | Bài làm chặt, nhất quán từ problem → workflow → metric → AI fit → decision |
| **Hiểu xuất sắc** | 90–100 | Tư duy rất chắc, phản biện tốt, chọn đúng mức giải pháp, quyết định trung thực và có chiều sâu |

---

## 3. Deliverables và điểm gắn với từng phần

| Deliverable | Ai làm | Điểm liên quan |
|---|---|---:|
| Scan & Filter Log | Cá nhân | 15 |
| Problem Deep-Dive | Nhóm | 60 |
| AI Support Log | Cá nhân | 15 |
| Pitch + Challenge Participation | Cá nhân (coach quan sát) | 10 |

> **Lưu ý:** Không có file riêng cho Pitch + Challenge Participation, nên phần này sẽ được coach/giảng viên đánh dấu trực tiếp trong lúc lab.

---

<<<<<<< HEAD:day-02/01-worksheet.md
## 4. Self-check theo từng phase
=======
# Phase 0 — Worked Example (15 min)

> *Giảng viên demo. Bạn chỉ cần xem và hiểu flow.*

Giảng viên sẽ walk through 1 ví dụ thật từ đầu đến cuối:

**Tôi gặp pain gì → Tôi scan → Tôi vẽ flow → Tôi thấy bottleneck → Tôi viết PS → Tôi check AI fit → Kết luận.**

Xem file [`02-deliverable-example.md`](02-deliverable-example.md) để đọc lại ví dụ đầy đủ.

**Bạn cần nắm:**
- Cách dùng 4 Lenses để tìm bài toán
- Cách vẽ workflow trên giấy
- Cách viết Problem Statement theo 6-field từ slide
- Cách check AI Fit

> **🤖 AI Tip — Chuẩn bị trước buổi lab: Deep Research**
> Dùng trước hoặc trong Phase 1 — không cần dùng ngay lúc xem demo.
> **Dùng AI để:** Research nhanh về domain, tìm data/case study liên quan
> **Tool gợi ý:** Claude, Gemini, ChatGPT, Perplexity, NotebookLM (nếu nhiều tài liệu)
> **Example prompt:** "Tôi đang nghiên cứu quy trình [tên quy trình] trong ngành [ngành]. Cho tôi 5 pain point phổ biến nhất và số liệu về thời gian/chi phí lãng phí ở mỗi bước."
> **Lưu ý:** Luôn verify nguồn — AI có thể bịa số liệu. Cross-check với ít nhất 1 nguồn khác.
> **→ Ghi vào Reflection Log:** AI giúp gì, sai gì, bạn sửa gì
>>>>>>> main:01-worksheet.md

---

# Phase 1 — SCAN (Cá nhân)

## Yêu cầu tối thiểu
- Liệt kê **ít nhất 5 problems**
- Dùng **ít nhất 3/4 lenses**
- Bài toán đến từ workflow thật, không phải ý tưởng chung chung kiểu “AI cho giáo dục”

<<<<<<< HEAD:day-02/01-worksheet.md
## Tự chấm nhanh I1.1 — Scan Breadth (5 điểm)
| Mức | Mô tả |
=======
## Bước 1.1 — Cá nhân: Liệt kê (12 min)

Dùng **4 Lenses** để quét xung quanh mình. Ghi **ít nhất 5 problems**.

### 4 Lenses tìm bài toán AI

| Lens | Câu hỏi | Ví dụ |
|------|---------|-------|
| **Lặp lại** | Việc gì tôi/team làm đi làm lại mỗi ngày/tuần? | "Mỗi thứ Hai tổng hợp báo cáo từ 4 file" |
| **Tốn thời gian** | Việc gì mất nhiều thời gian hơn lẽ ra nên mất? | "Duyệt 20 đơn hàng/ngày, mỗi đơn mất 15 min kiểm tra thông tin" |
| **AI có thể tốt hơn** | Sản phẩm nào tôi dùng mà AI có thể cải thiện? | "App đặt vé, mỗi lần hỏi CSKH phải chờ 20 phút" |
| **Pain từ người khác** | Đồng nghiệp/bạn bè hay phàn nàn gì? | "Team họp xong, follow-up rơi rụng hết" |

### Gợi ý thêm cách tìm
- Nghĩ về 1 ngày làm việc điển hình — chỗ nào bạn thấy mệt/chán nhất?
- Sản phẩm nào bạn dùng hàng ngày mà hay nghĩ "giá như nó có feature X"?
- Ở công ty/trường, quy trình nào mọi người hay phàn nàn?
- Đọc review 1-star trên app bạn hay dùng — pain point nào lặp lại?

> Nếu bạn chưa nghĩ ra, xem [`03-inspiration-kit.md`](03-inspiration-kit.md) để lấy ý tưởng.

### List của tôi

| # | Lens | Bài toán |
|---|------|----------|
| 1 | | |
| 2 | | |
| 3 | | |
| 4 | | |
| 5 | | |
| 6 | | |
| 7 | | |
| 8 | | |
| ... | | |

> **🤖 AI Tip — Phase 1: Thought Partner nếu bí**
> **Dùng AI để:** Gợi ý thêm góc nhìn nếu bạn chưa đủ 5 bài toán. **Tự brainstorm trước, AI sau.**
> **Tool gợi ý:** ChatGPT, Claude, Gemini, Perplexity — tuỳ bạn
> **Example prompt:** "Tôi là [vai trò] làm trong [lĩnh vực], công việc hàng ngày gồm [liệt kê tasks]. Có những pain point nào mà AI có thể giúp cải thiện?"
> **Lưu ý:** Prompt này chỉ gợi ý — bạn cần filter lại dựa trên kinh nghiệm thật của mình.
> **→ Ghi vào Reflection Log:** AI gợi ý gì, bạn giữ lại bao nhiêu ý?

## Bước 1.2 — Nhóm: Quick Share (8 min)

Mỗi người đọc nhanh **top 3** cho nhóm nghe (~1 min/người). Chỉ nghe, không thảo luận sâu.

Ghi nhận: có pain nào trùng nhau giữa các thành viên không?

---

# Phase 2 — QUICK-ASSESS: Round 1 (40 min)

## Mục tiêu
Quick-pass qua top 3 bài toán. Mỗi cái 10 phút — buộc ra quyết định nhanh, không overthink.

## Bước 2.1 — Cá nhân: Viết 3 Quick Problem Cards (30 min)

Chọn **top 3** từ list → với mỗi cái, điền 1 **Quick Problem Card** (10 min/card).

> Dùng template bên dưới hoặc tự kẻ trên giấy.

### Quick Problem Card

```
┌─────────────────────────────────────────────┐
│ QUICK PROBLEM CARD #___                     │
│                                             │
│ Bài toán (1 câu): ______________________   │
│                                             │
│ Ai đang đau? ___________________________   │
│                                             │
│ Workflow hiện tại (3-5 bước):               │
│   1. ___ → 2. ___ → 3. ___ → 4. ___       │
│                                             │
│ Bước nào tốn nhất? ___  (⏱ ___ min/lần)   │
│                                             │
│ AI có thể giúp ở bước nào? ____            │
│                                             │
│ Đo thành công bằng gì? _____ (có số!)      │
│   VD: "Giảm từ 90 min → 30 min"            │
│                                             │
│ Quick gut: □ No AI  □ Rule  □ LLM  □ Agent │
└─────────────────────────────────────────────┘
```

**Lưu ý:**
- "Đo thành công" phải có **con số hoặc ngưỡng cụ thể** — không viết "nhanh hơn" hay "tốt hơn"
- "Quick gut" dùng thang từ slide: No AI → Rule/Workflow → LLM Feature → Agent
- Nếu không biết AI giúp ở đâu → ghi "chưa rõ" — đó là signal tốt, không phải lỗi

> **🤖 AI Tip — Phase 2: Mở rộng góc nhìn + Phản biện**
> **Dùng AI để:** Check lại Quick Problem Card — AI có thể chỉ ra góc bạn bỏ sót. **Tự điền card trước, AI phản biện sau.**
> **Tool gợi ý:** Để mở — dùng tool bạn quen nhất
> **Example prompt:** "Đây là bài toán của tôi: [paste nội dung card]. Hãy đặt 3 câu hỏi phản biện để kiểm tra xem bài toán này có thật sự cần AI không, và metric đã đủ cụ thể chưa."
> **Lưu ý:** AI hay đồng ý với bạn — hãy yêu cầu nó phản biện, đừng hỏi "bài toán này tốt không?"

## Bước 2.2 — Nhóm: Gallery Mini (10 min)

Trải tất cả cards lên bàn (12-15 cards/nhóm).

Mỗi người có **2 dots** (vẽ bằng bút) → dán vào cards hay nhất (của mình hoặc của bạn).

Quick reactions — nếu thấy card nào:
- "Cái này rule đủ rồi" → ghi bên cạnh
- "Cái này thú vị, muốn biết thêm" → ghi bên cạnh

---

# Break (10 min)

---

# Phase 3 — PITCH-CHALLENGE-VOTE (30 min)

## Mục tiêu
Fix thiên kiến cá nhân (self-referential bias) + học cách nói KHÔNG.

> Phase này không dùng AI — tự tư duy và phản biện trong nhóm.

## Bước 3.1 — Pitch + Challenge (20 min)

Mỗi người lần lượt pitch card **được vote nhiều nhất** của mình cho cả nhóm.

**Mỗi lượt (5 min/người, nhóm 5 người: 4 min/người):**

1. **PITCH (2 min):** Present bài toán của mình. Dùng Quick Problem Card làm visual.

2. **CHALLENGE (3 min):** Nhóm hỏi **3 câu có sẵn**:
   - *"Rule/script đủ chưa? Có thật sự cần AI không?"*
   - *"Ngoài bạn, ai đau nữa? Bao nhiêu người?"*
   - *"Metric đo được không? Có số cụ thể chưa?"*

> **Vì sao bước này quan trọng?** Nếu bạn thiết kế cho chính mình, bạn dễ mặc định "ai cũng đau giống tôi." 3 câu challenge giúp nhóm kiểm tra giả định đó.

## Bước 3.2 — Vote + Kill Round (10 min)

Sau khi tất cả pitch xong: **Mỗi người 1 phiếu** → bình chọn bài toán hay nhất.

**Nhóm quyết định:** Từ tất cả cards → chọn **1 bài toán** để deep-dive.

### Tiêu chí lựa chọn

| Tiêu chí | Hỏi |
|----------|-----|
| **Frequency** | Nhiều người trong nhóm cùng gặp? |
| **Impact** | Tốn thời gian/tiền thật sự đo được? |
| **AI-likely** | AI có khả năng giúp? (không quá trivial, không quá impossible) |
| **Vẽ flow được** | Có thể mô tả rõ workflow hiện tại? |

**Bắt buộc:** Viết **1 dòng lý do kill** cho mỗi card bị loại.

| Card bị loại | Lý do |
|--------------|-------|
| | |
| | |
| | |
| | |

**Card được chọn:** _______________

**Vì sao chọn:** _______________

---

# Phase 4 — DEEP-DIVE: Round 2 (85 min)

## Mục tiêu
Phân tích kỹ 1 bài toán. Đây là phần chính — output ở đây là deliverable nộp bài.

Cả nhóm cùng làm. **Dùng giấy A3 hoặc whiteboard.**

## Bước 4.1 — Current-State Workflow Mapping (25 min)

### Cách vẽ

**VẼ trên giấy**, không viết text list.

Mỗi bước = 1 ô. Nối bằng mũi tên. Ghi lên mỗi ô:

```
┌─────────────┐     ┌─────────────┐     ┌─────────────┐
│ Bước 1      │     │ Bước 2      │     │ Bước 3      │
│ Ai: ___     │ ──→ │ Ai: ___     │ ──→ │ Ai: ___     │
│ ⏱ ___ min   │     │ ⏱ ___ min   │     │ ⏱ ___ min   │
│ Input: ___  │     │ Input: ___  │     │ Input: ___  │
│ Output: ___ │     │ Output: ___ │     │ Output: ___ │
└─────────────┘     └─────────────┘     └─────────────┘
```

### Ký hiệu

- 🔴 **Bottleneck** — bước tốn thời gian/lỗi nhiều nhất
- 🔄 **Handoff** — chỗ chuyển giao giữa người/hệ thống
- ⏱ **Thời gian** — ghi rõ mỗi bước mất bao lâu

### Yêu cầu
- Ít nhất **5-8 bước**
- Phải có ít nhất 1 bottleneck đánh dấu đỏ
- Ghi tổng thời gian hiện tại: ___ min/lần

### Digitize bằng AI (sau khi vẽ xong)

Chụp ảnh flow vẽ tay → dùng AI để chuyển thành diagram đẹp hơn.

> **🤖 AI Tip — Phase 4a: Digitize Workflow**
> **Dùng AI để:** Chuyển flow vẽ tay thành diagram digital
> **Tool gợi ý:** Claude, ChatGPT, Gemini — tool nào đọc ảnh được (hoặc Antigravity nếu bạn có)
> **Example prompt:** "Đây là ảnh chụp workflow vẽ tay của nhóm tôi [paste ảnh]. Hãy chuyển thành flowchart diagram, giữ đúng thứ tự các bước, ghi rõ ai làm, thời gian mỗi bước, và đánh dấu bottleneck bằng màu đỏ."
> **Lưu ý:** So sánh diagram AI tạo với bản vẽ tay — AI hay bỏ sót bước hoặc đổi thứ tự. Sửa lại nếu sai.
> **→ Ghi vào Reflection Log:** AI digitize đúng bao nhiêu %, bạn phải sửa gì?

> **Thứ tự quan trọng:** Vẽ tay **trước** để tư duy rõ flow, AI digitize **sau** để trực quan hoá.

## Bước 4.2 — Problem Statement + Metrics (15 min)

### Problem Statement (6-field)

Dùng đúng khung từ slide:

| Field | Nội dung |
|-------|----------|
| **Actor / Operator** | Ai đang làm việc này hằng ngày? |
| **Current Workflow** | Hiện tại họ xử lý qua những bước nào, dùng tool gì? |
| **Bottleneck** | Bước nào chậm, lỗi, không nhất quán, hoặc cần tổng hợp quá nhiều? |
| **Impact** | Tổn thất đo bằng thời gian, chi phí, SLA, error rate, hay conversion nào? |
| **Success Metric** | Khi nào được coi là thành công? Mức ngưỡng là bao nhiêu? |
| **Operational Boundary** | Hệ thống được phép làm gì, không được phép làm gì, và điểm nào cần human-in-the-loop? |

> **Nhớ:** Nếu viết xong mà bạn chưa hình dung được cách thử nghiệm (test cases), cách đo thành/bại (eval metric), và giới hạn hệ thống được phép làm gì (architecture boundary), thì problem statement vẫn chưa đủ chặt.

Điền:

| Field | Nội dung |
|-------|----------|
| Actor / Operator | |
| Current Workflow | |
| Bottleneck | |
| Impact | |
| Success Metric | |
| Operational Boundary | |

> **🤖 AI Tip — Phase 4b: Phản biện Problem Statement**
> **Dùng AI để:** Check logic và tìm lỗ hổng trong PS. **Viết PS xong trước, AI phản biện sau.**
> **Tool gợi ý:** Để mở — dùng tool bạn quen nhất
> **Example prompt:** "Đây là Problem Statement của nhóm tôi: [paste 6 fields]. Hãy chỉ ra: (1) field nào còn mơ hồ, (2) metric đã đo được chưa, (3) operational boundary đã rõ chưa, (4) thiếu gì để suy ra test cases?"
> **Lưu ý:** AI hay khen PS của bạn — hãy yêu cầu rõ "chỉ ra điểm yếu, đừng khen."

### Sub-goals Decomposition

Trước khi giải bài toán lớn, user phải giải những bài phụ nào?

**Sub-goals user phải giải TRƯỚC khi dùng AI solution:**
- _______________________________________________
- _______________________________________________

**Sub-goals user phải giải TRONG KHI dùng AI solution:**
- _______________________________________________
- _______________________________________________

Các sub-goals này {nhất quán / mâu thuẫn} với primary goal vì:
_______________________________________________

> *Ví dụ: Bài toán "AI phân loại email support tự động". Sub-goal trước: team phải gắn label cho 500+ email cũ để train. Sub-goal trong khi: user phải review các email AI phân loại sai. Cả hai nhất quán với goal vì đều hướng đến giảm thời gian xử lý.*

### Success Metrics — ít nhất 2, phải có ngưỡng

| Loại | Metric | Ngưỡng |
|------|--------|--------|
| Efficiency (thời gian/chi phí) | | |
| Quality (chất lượng output) | | |

**Ví dụ tốt:** "Giảm thời gian xử lý từ 8 min → dưới 3 min" / "Tỉ lệ lỗi không tăng quá 2%"
**Ví dụ xấu:** "Nhanh hơn" / "Tốt hơn" / "User hài lòng"

## Bước 4.3 — Research (20 min)

> **🤖 AI Tip — Phase 4c: Deep Research**
> **Dùng AI để:** Tìm existing solutions, case studies, và data liên quan đến bài toán
> **Tool gợi ý:** Claude, Gemini, ChatGPT, Perplexity (tốt cho tìm nguồn), NotebookLM (nếu có nhiều tài liệu)
> **Example prompt:** "Nhóm tôi đang giải bài toán [mô tả ngắn]. Tìm cho tôi: (1) 2-3 sản phẩm/startup đã giải bài toán tương tự, (2) 1 case study có kết quả đo được, (3) con số thống kê về pain point này trong ngành [ngành]."
> **Lưu ý:** AI hay bịa tên công ty và số liệu — verify mọi nguồn bằng Google trước khi ghi vào worksheet.
> **→ Ghi vào Reflection Log:** AI tìm được gì đúng, bịa gì, bạn verify thế nào?

Phân công trong nhóm:

| Ai | Làm gì | Ghi kết quả |
|----|--------|-------------|
| 1-2 người | Tìm **1 sản phẩm/tool** đã giải bài toán tương tự | Tên: ___ / Approach: ___ / Điểm mạnh: ___ / Điểm yếu: ___ |
| 1-2 người | Tìm **1 case study** hoặc bài viết liên quan | Nguồn: ___ / Họ làm gì: ___ / Kết quả: ___ / Bài học: ___ |
| 1 người | Quick poll: hỏi 2-3 người ngoài nhóm "bạn có gặp pain này không?" | Người 1: ___ / Người 2: ___ / Người 3: ___ |

**Share findings (5 min cuối):** Gộp lại, ghi lên giấy/board.

### Research findings tổng hợp

**Existing solution:**

**Case study / bài viết:**

**Quick poll kết quả:**

**Bài học rút ra cho bài toán của mình:**

## Bước 4.4 — Future-State Flow + AI Fit (25 min)

### Trước khi vẽ — trả lời 3 câu hỏi

Dùng các framework từ slide:

**1. AI Fit Check (dùng AI-Fit Matrix từ slide)**

| | Ambiguity thấp | Ambiguity cao |
|--|----------------|---------------|
| **Complexity thấp** | Rule/workflow đủ | LLM feature |
| **Complexity cao** | Workflow + automation | Agent (cẩn thận!) |

Bài toán của nhóm nằm ở ô nào? ___

**2. AI Suitability Check**

| AI có lẽ PHÙ HỢP khi... | AI có lẽ KHÔNG phù hợp khi... |
>>>>>>> main:01-worksheet.md
|---|---|
| 0–1 | Dưới 3 problems, gần như chỉ có 1 loại lens |
| 2–3 | Có 3–4 problems, dùng 2–3 lenses |
| 4 | Có 5+ problems, dùng 3 lenses |
| 5 | Có 5+ problems, dùng 3–4 lenses, pain point cụ thể và đa dạng |

### Checklist tự kiểm tra
- [ ] Tôi có ít nhất 5 problems
- [ ] Tôi dùng ít nhất 3 lenses
- [ ] Mỗi problem đủ cụ thể để hình dung workflow
- [ ] Không problem nào quá rộng kiểu “xây AI agent cho công ty”

---

# Phase 2 — QUICK-ASSESS (Cá nhân)

## Yêu cầu tối thiểu
- Viết **3 Quick Problem Cards**
- Mỗi card có:
  - actor hoặc người chịu đau
  - 3–5 bước workflow hiện tại
  - bottleneck
  - 1 metric có số hoặc ngưỡng
  - quick gut: No AI / Rule / LLM / Agent

## Tự chấm nhanh I1.2 — Quick Problem Cards (10 điểm)
| Mức | Mô tả |
|---|---|
| 0–3 | Thiếu nhiều field, metric kiểu “nhanh hơn/tốt hơn” |
| 4–6 | Đủ field cơ bản nhưng flow còn hời hợt hoặc metric chưa rõ ngưỡng |
| 7–8 | Cả 3 cards đều khá rõ, metric có số, quick gut hợp lý |
| 9–10 | Cards rõ, có critical thinking, chỉ ra đúng bottleneck và đo được thành công |

### Checklist tự kiểm tra
- [ ] Tôi có đủ 3 cards
- [ ] Mỗi card có metric cụ thể, không mơ hồ
- [ ] Tôi mô tả được 3–5 bước workflow hiện tại
- [ ] Tôi không mặc định chọn Agent cho mọi card

---

# Phase 3 — PITCH-CHALLENGE-VOTE (Nhóm, NO-AI)

## Mục tiêu của phần này
- kiểm tra chất lượng ý tưởng bằng phản biện người thật
- loại bỏ confirmation bias
- buộc mỗi người phải nói được vì sao bài toán của mình đáng đi tiếp

## Điểm cá nhân I2 — Pitch + Challenge Participation (10 điểm)
| Mức | Mô tả |
|---|---|
| 0–2 | Không pitch rõ được, không challenge hoặc challenge rất hời hợt |
| 3–5 | Pitch được ý chính nhưng còn solution-first, challenge chưa sắc |
| 6–8 | Pitch rõ workflow, pain, metric; challenge bám đúng 3 câu chuẩn |
| 9–10 | Pitch rất rõ, challenge có chất lượng, giúp nhóm chọn tốt hơn |

## 3 câu challenge bắt buộc
1. **Rule/script đủ chưa? Có thật sự cần AI không?**
2. **Ngoài bạn, ai đau nữa? Bao nhiêu người?**
3. **Metric đo được không? Có số cụ thể chưa?**

### Checklist tự kiểm tra
- [ ] Tôi đã pitch rõ trong 2 phút
- [ ] Tôi đã challenge ít nhất 1 bạn khác bằng 3 câu chuẩn
- [ ] Tôi có thể nói rõ vì sao card của mình bị kill hoặc được chọn
- [ ] Tôi chấp nhận “No AI / Rule” là kết luận hợp lệ nếu đúng

---

<<<<<<< HEAD:day-02/01-worksheet.md
# Phase 4 — DEEP-DIVE (Nhóm)
=======
# Phase 6 — Reflection + Reflection Log (10 min)
>>>>>>> main:01-worksheet.md

## G1. Workflow Mapping (20 điểm)

<<<<<<< HEAD:day-02/01-worksheet.md
### Tiêu chí chấm
| Tiêu chí | Điểm tối đa | Cần có |
|---|---:|---|
| Số bước & cấu trúc diagram | 5 | Ít nhất 5 bước, không phải text list |
| Bottleneck & handoff | 5 | Có ít nhất 1 bottleneck, có handoff nếu có chuyển giao |
| Thời gian | 5 | Có thời gian từng bước hoặc đủ để suy ra tổng |
| Độ rõ | 5 | Người khác nhìn vào hiểu được workflow |
=======
## Reflection Log (bắt buộc)
>>>>>>> main:01-worksheet.md

### Tự kiểm tra
- [ ] Flow có ít nhất 5 bước
- [ ] Có bottleneck đánh dấu rõ
- [ ] Có thời gian từng bước hoặc tổng workflow hợp lý
- [ ] Flow thể hiện được ai làm gì, không chỉ “hệ thống làm”

---

## G2. Problem Statement + Metrics (20 điểm)

### 6 field bắt buộc
1. Actor / Operator
2. Current Workflow
3. Bottleneck
4. Impact
5. Success Metric
6. Operational Boundary

<<<<<<< HEAD:day-02/01-worksheet.md
### Tiêu chí chấm
| Tiêu chí | Điểm tối đa | Cần có |
|---|---:|---|
| Đủ 6 fields | 6 | Không thiếu field nào |
| Cụ thể & scope hẹp | 4 | Đúng 1 workflow, không solution-first |
| Success metrics | 5 | Ít nhất 2 metrics, có ngưỡng |
| Boundary + HITL | 5 | Rõ AI được/không được làm gì |
=======
| # | Deliverable | Ai làm | Mô tả |
|---|-------------|--------|-------|
| 1 | **Scan & Filter Log** | Cá nhân | List 5+ problems + 3 Quick Problem Cards + kill rationale |
| 2 | **Problem Deep-Dive** | Nhóm | Current flow (vẽ) + PS 6-field + Metrics + Research + Future flow (vẽ) + AI Fit + Go/Not Yet/No-Go |
| 3 | **Reflection Log** | Cá nhân | AI giúp gì / sai gì / sửa gì |
>>>>>>> main:01-worksheet.md

### Tự kiểm tra
- [ ] PS đủ 6 field
- [ ] Scope đủ hẹp để hình dung test case
- [ ] Metric có số/ngưỡng, không chỉ là mong muốn chung chung
- [ ] Boundary nói rõ AI không được làm gì

> **Test nhanh:** Nếu đọc PS mà chưa suy ra được test cases, eval metric, boundary, thì PS chưa đủ chặt.

---

## G3. AI Fit + Research + Future Flow (10 điểm)

### Tiêu chí chấm
| Tiêu chí | Điểm tối đa | Cần có |
|---|---:|---|
| AI Fit justification | 3 | So sánh Rule / LLM / Agent |
| Research | 2 | Có existing solution hoặc case study |
| Future-state flow | 3 | Có AI/Human/Boundary/Fallback |
| Underspecification / Suitability | 2 | Có ít nhất 2 assumptions hoặc điều chưa rõ |

### Tự kiểm tra
- [ ] Chúng tôi đã so sánh alternatives, không mặc định chọn Agent
- [ ] Có ít nhất 1 existing solution hoặc case study
- [ ] Future flow có AI/Human/Boundary/Fallback
- [ ] Có ít nhất 2 điều chưa rõ và cách tìm ra chúng

---

# Phase 5 — EVALUATE (Nhóm, NO-AI)

## G4. Decision Quality (10 điểm)

### Tiêu chí chấm
| Tiêu chí | Điểm tối đa | Cần có |
|---|---:|---|
| AI Readiness checklist | 3 | Điền đủ 5 câu, có ghi chú |
| Optimization check | 2 | Nêu benefits và risks cụ thể |
| Go / Not Yet / No-Go | 3 | Quyết định rõ |
| Justification | 2 | Bám evidence từ workflow, PS, research |

### Tự kiểm tra
- [ ] Chúng tôi điền đủ AI Readiness checklist
- [ ] Quyết định khớp với evidence
- [ ] Nếu chọn Not Yet, đã nói rõ cần validate gì tiếp
- [ ] Nếu chọn Go, đã nói rõ scope nhỏ/pilot là gì

> **Nhắc lại:** “Not Yet” với justify tốt có thể cao điểm hơn “Go” với lập luận yếu.

---

# Phase 6 — REFLECTION + AI SUPPORT LOG (Cá nhân, NO-AI)

## I3. AI Support Log + Reflection (15 điểm)

### Tiêu chí chấm
| Tiêu chí | Điểm tối đa | Cần có |
|---|---:|---|
| AI giúp gì | 4 | Nói rõ AI hỗ trợ phase nào |
| AI sai ở đâu | 4 | Chỉ ra lỗi, thiếu, hoặc hallucination |
| Tôi sửa gì | 4 | Có human correction cụ thể |
| Reflection quality | 3 | Nói được bài học và nếu làm lại sẽ đổi gì |

### Checklist tự kiểm tra
- [ ] Tôi ghi rõ AI giúp ở đâu, không viết chung chung “AI hỗ trợ tốt”
- [ ] Tôi ghi rõ AI sai/hời hợt ở đâu
- [ ] Tôi ghi rõ mình/nhóm đã sửa gì bằng tay
- [ ] Reflection trung thực, không “tô hồng” việc dùng AI

---

## 5. Cách tính điểm cuối cùng

### Bước 1 — Tính điểm nhóm
- G1 + G2 + G3 + G4 = **60 điểm**

### Bước 2 — Tính điểm cá nhân
- I1 + I2 + I3 = **40 điểm**

### Bước 3 — Cộng điểm
- **Final = Group Score (60) + Individual Score (40)**

---

## 6. Điều gì làm bài được điểm cao?

- Chọn **đúng bài toán**, không chọn bài “ngầu” nhưng mơ hồ
- Biết nói **“chưa cần AI”** hoặc **“rule đủ rồi”** khi phù hợp
- Metric đủ rõ để người khác thấy “thành công” là gì
- Boundary đủ rõ để biết AI **được phép làm gì / không được phép làm gì**
- Reflection trung thực về chỗ AI hữu ích và chỗ AI gây hại

---

## 7. Điều gì thường làm mất điểm?

- Chỉ liệt kê pain chung chung, không ra được workflow
- Metric kiểu “nhanh hơn / tốt hơn / user thích hơn”
- Mặc định chọn Agent mà không justify
- Không có fallback nếu AI sai
- AI Support Log kiểu copy-paste, không phản ánh gì thật

---

**Bản v2 này dùng để học viên tự kiểm tra chất lượng bài làm trước khi nộp.**
