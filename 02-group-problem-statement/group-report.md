# 02 — Group Problem Statement (Bản nộp nhóm)

> Làm chung 1 bản, mỗi thành viên copy vào repo cá nhân. Đi theo Phase 3 → 6 trong `01-worksheet.md`. Nhóm chỉ chọn **candidate problem** ở Phase 3, viết Problem Statement sau khi validate + vẽ workflow.

## Thành viên nhóm

| STT | Họ và tên | Mã học viên | Vai trò trong nhóm (VD: facilitator, workflow, research, writer) |
|-----|-----------|-------------|---------------------------------------------------------------|
| 1   | Đỗ Trương Thành Ân | 2A202602889 | Facilitator |
|2   | Trần Tuấn Tú |             |                                                               |
| 3   |           |             |                                                               |
| 4   |           |             |                                                               |

**Candidate problem nhóm chọn (1 câu):**


---

## Phase 3 — Group Convergence: từ 9-12 candidates về 1

### 3.1. Trình bày top 3 mỗi người (mỗi candidate 1-2 phút)

| # | Người đưa ra | Candidate problem | Người gặp vấn đề | Điểm nghẽn | Cảm nhận nhanh của nhóm |
|---|---|---|---|---|---|
| 1 | Đỗ Trương Thành Ân | Ghi chép thông tin thủ công làm giảm hiệu suất và kết nối khách hàng | Nhân viên bán hàng | Cặm cụi ghi chép thông tin làm đứt gãy tương tác mắt (eye-contact) và cảm xúc của khách hàng. Nếu để đến cuối mới nhập liệu, nhân viên dễ bị quên, nhớ nhầm số điện thoại hoặc sót các chi tiết quan trọng về nhu cầu của khách. | Vấn đề trực quan, dễ nhận thấy. Giải pháp đề xuất khá thành hình, phù hợp để trình bày |
| 2 | Đỗ Trương Thành Ân | Kế toán mất quá nhiều thời gian dò đối chiếu thủ công từng khoản tiền gửi ngân hàng với đơn hàng trên hệ thống do khách hàng thường ghi chú chuyển khoản sai cú pháp, dẫn đến chậm trễ tiến độ giao hàng. | Kế toán | Việc khớp lệnh thủ công hoàn toàn bế tắc và mất thời gian khi nội dung chuyển khoản bị sai mã đơn, thiếu chữ, hoặc chỉ ghi tên/số điện thoại. Kế toán buộc phải tự suy luận dựa trên số tiền lẻ hoặc nhắn tin hỏi lại bộ phận Sales để xác nhận, làm gián đoạn toàn bộ luồng công việc. | Vấn đề trực quan, nhưng chưa cần AI để xử lý, hard code được |
| 3 | Đỗ Trương Thành Ân | Việc cập nhật tồn kho thủ công gây ra độ trễ dữ liệu | Quản lý cửa hàng | Số lượng tồn kho trên các nền tảng online không được cập nhật theo thời gian thực (real-time) cùng với số lượng vật lý. | Ý tưởng hay |
| 4 |  Trần Tuấn Tú | Giải cứu "nghĩa địa ghi chú": Xử lý tồn đọng 200+ quick note & bookmark do lịch học 8h/ngày dồn dập | Người học cường độ cao (học 9h-18h, hay lưu ý tưởng vội) | Mất ngữ cảnh ban đầu khi mở lại; việc dọn dẹp mất 2-4h và gây ngợp tâm lý nên bỏ xó | Pain point rất thật và phổ biến; AI có thế mạnh rõ rệt về gom cụm (clustering) và làm giàu ngữ cảnh |
| 5 | Trần Tuấn Tú | Tra cứu kiến thức trong kho Slide bài giảng PDF (10-15 file, 60-100 trang/file) khi làm lab/ôn thi | Sinh viên/học viên cần tìm lại công thức, định nghĩa để làm bài | Ctrl+F không hiệu quả nếu giảng viên dùng từ đồng nghĩa hoặc giải thích bằng hình ảnh (mất 20-30') | Bài toán RAG/Semantic search kinh điển, phạm vi hẹp và dữ liệu khép kín, rất khả thi |
| 6 | Trần Tuấn Tú | Tối ưu luồng tổng hợp & chắt lọc Tech News hằng ngày (5-7 kênh tin) vào buổi tối | Người học tech/AI cần cập nhật xu hướng liên tục | Mất 35' đọc lướt loại bỏ tin rác, clickbait và tin trùng lặp nội dung giữa các kênh | Workflow rõ ràng; có thể giải quyết tốt bằng AI đọc toàn văn + đánh giá + summary kèm link gốc |
| 7 | Lê Thanh Trường | Đọc tài liệu lab để hiểu yêu cầu nộp bài (40-60'/lab) | Mọi học viên | Tổng hợp yêu cầu rải rác từ 3 file | Ai cũng gật đầu — pain chung rõ nhất |
| 8 | Lê Thanh Trường | Luyện viết tiếng Anh không có feedback ngay (chờ 2-3 ngày) | Người tự học tiếng Anh | Tự review không chuẩn + feedback trễ  | Hay nhưng là pain cá nhân, ít người trong nhóm gặp |
| 9 | Lê  Thanh Trường | Viết reflection sau lab không nhớ chi tiết (30-45') | Mọi học viên | Trí nhớ sau lab 4 tiếng | Thú vị, có thể giải bằng process fix |
| 10 | Hoàng Văn Dương | Phân nhóm các output sai sau khi đánh giá model/prompt trên một batch khoảng 200 mẫu | AI/ML Engineer hoặc Model Evaluator; Tech Lead sử dụng báo cáo lỗi để chọn việc cần sửa | Phải đọc input, actual output, expected output và context rồi gán error type, severity và root cause; bước này mất khoảng 150 trong tổng số 210 phút/batch | Sát công việc AI Engineer, input/output rõ và có thể đo trên một batch trong lab; phù hợp với Workflow kết hợp Rule, AI và human review |
| 11 | Hoàng Văn Dương | Tổng hợp báo cáo tiến độ thí nghiệm AI hằng tuần từ notebook, experiment log và ghi chú rời rạc | AI Engineer lập báo cáo; Tech Lead và thành viên dự án đọc để quyết định thí nghiệm tiếp theo | Tìm đúng run, copy metric và đối chiếu dataset, config, model version từ nhiều nguồn mất khoảng 40 trong tổng số 85 phút/báo cáo | Tác vụ lặp lại, workflow rõ và dễ đo before/after; phần lấy metric có thể dùng Rule/script, còn AI chỉ nên draft narrative có nguồn dẫn |
| 12 | Hoàng Văn Dương | Trích xuất decision và action item sau các cuộc họp kỹ thuật rồi đồng bộ sang công cụ quản lý công việc | Người điều phối/người ghi biên bản; người tham dự và người được giao action item | Đọc transcript/notes, xác định decision, viết lại task và tìm owner/deadline còn thiếu mất khoảng 17 trong tổng số 25 phút/cuộc họp | Actor và output rõ, có thể prototype trên 5–10 transcript; cần giữ facilitator ở bước duyệt để tránh tạo hoặc giao nhầm task |
| 13 | Dương Hải Minh | Người đi đường đi vào đường bị ngập vào mỗi khi trời mưa ngập lụt | Người tham gia giao thông | Thiếu thông tin cảnh báo lộ trình ngập lụt theo thời gian thực khiến người dân không thể chủ động chọn hướng đi an toàn lúc tan tầm. | Vấn đề rất thực tế nhưng độ khả thi phụ thuộc hoàn toàn vào nguồn cấp dữ liệu ngập lụt (sensor/camera của thành phố), chưa rõ hệ thống hiện tại có open API không. |
| 14 | Dương Hải Minh | Mỗi ngày phải tập hợp task trên Jira về Google doc cho team | Người tổng hợp task và Team QA | Thao tác copy-paste lặp đi lặp lại hàng ngày để gom dữ liệu phân mảnh từ nhiều dashboard Jira khác nhau vào một nơi. | Rất dễ tự động hóa bằng API hoặc Workflow, nhưng cần đánh giá kỹ xem việc cấu hình lại trực tiếp Dashboard trên Jira có tối ưu hơn việc phải tạo Doc trung gian hay không. |
| 15 | Dương Hải Minh | Khi có thông báo trên khóa học thì ban tổ chức cần phải thông báo ở nhiều nền tảng | Ban tổ chức và Học viên | Quy trình đăng tải thủ công cùng một nội dung lên nhiều kênh (Email, Zalo, Facebook...) tốn thời gian và dễ xảy ra sai sót, bỏ sót học viên. | Problem này rất phù hợp để làm Automation Workflow/Agent. Tuy nhiên, nhóm cần khảo sát xem thị trường đã có sẵn các agent làm tốt chưa để tránh làm lại "bánh xe". |


### 3.2. Gom trùng / cluster (gom 9-12 ý thành 3-4 cụm)

| Cluster | Candidates included | Pattern chung | Ghi chú |
|---|---|---|---|
| A | | | |
| B | | | |
| C | | | |
| D (nếu có) | | | |

### 3.3. Shortlist (giữ 2-3 bài trả lời được 7 câu hỏi worksheet)

| Candidate | Vì sao vào shortlist (2-3 ý) | Rủi ro / điều chưa rõ |
|---|---|---|
| | | |
| | | |
| | | |

### 3.4. Score để đồng thuận (chấm 1-5, ép nói rõ vì sao cho 5 / cho 3)

| Candidate | Actor rõ | Workflow rõ | Pain có evidence | Impact đo được | Làm trong lab | So sánh R/W/A được | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| | | | | | | | | |
| | | | | | | | | |
| | | | | | | | | |

**Candidate nhóm chọn (1 bài duy nhất):**

```text

```

**Vì sao chọn (4-5 câu):**

```text

```

**Vì sao KHÔNG chọn các candidate còn lại (mỗi bài 2-3 câu):**

```text

```

**Disagreement (nếu có — ai lo gì, chốt ra sao):**

```text

```

---

## Phase 4 — Quick Validation + Research

### 4.1. Quick validation (ít nhất 1 cách: interview 2-3 người hoặc survey 5-10 người)

| Nguồn | Số người / mẫu | Tín hiệu xác nhận (kèm quote nguyên văn) | Tín hiệu phản bác | Nhóm sửa problem thế nào |
|---|---:|---|---|---|
| Interview | | | | |
| Survey / poll | | | | |
| Log / ticket / review (nếu có) | | | | |

**Insight sau validation (1-2 câu — pain thật nằm ở đâu):**

```text

```

Bằng chứng đính kèm (nếu có): `02-group-problem-statement-survey.png`, `...-interview-notes.md`

### 4.2. Research giải pháp đã có (ít nhất 2-3 tools/patterns + 1-2 link kiểm được)

| Nguồn / tool / case | Link | Họ giải quyết bước nào? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| | | | | | |
| | | | | | |
| | | | | | |

**Research takeaway (2-3 câu — nên build gì / không build gì):**

```text

```

> Lưu ý: không dùng số liệu AI đưa nếu không verify được link chính thức. Ghi rõ giả định chưa chắc.

---

## Phase 5 — Workflow + Problem Statement

### 5.1. Current workflow bản nhóm

Dán workflow hoặc link file: `02-group-problem-statement-workflow.png/pdf/md`

```text
[1 ...: __' - ai làm] → [2 ...: __'] → [3 ...: __'] → [4 ... bottleneck: __'] → ...
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú (handoff? bottleneck?) |
|---|---|---|---|---|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |
| 6 | | | | | |
| 7 | | | | | |

**Bottleneck chính (2-3 câu):**

```text

```

### 5.2. Future workflow bản nhóm

Phải nhìn ra 5 thứ: bước nào máy (Rule), bước nào AI, bước nào người, boundary ở đâu, fallback khi AI sai.

```text
[1 ...: __' - máy] → [2 AI ...: __'] → [3 ... review: __' - boundary] → [4 ... gửi]

Fallback: ...
```

**Before/after impact:**

| Metric | Trước | Sau kỳ vọng | Cách đo |
|---|---:|---:|---|
| Tổng thời gian | | | |
| Số bước | | | |
| Số bước thủ công | | | |
| Bottleneck chính | | | |
| Risk mới | | | |

### 5.3. Problem Statement v0 (mỗi field 2-3 câu)

| Field | Nội dung |
|---|---|
| **Actor** | |
| **Workflow** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** | |
| **Boundary** | |

**Câu hỏi AI phản biện v0 (nếu có):**
- Field nào mơ hồ:
- Tôi sửa gì:

---

## Phase 6 — Rule / Workflow / Agent + Decision

### 6.0. Ma trận độ phù hợp (suy nghĩ nhanh, không thay quyết định cuối)

- Độ mơ hồ: [ ] Thấp (có đúng/sai rõ) / [ ] Cao (nhiều cách trả lời vẫn OK) — Vì sao:
- Độ phức tạp: [ ] Thấp (1-2 bước) / [ ] Cao (3+ bước/nguồn, phụ thuộc nhau) — Vì sao:

**Bài toán nhóm nằm ở ô nào:**

```text

```

**Vì sao (2-3 câu):**

```text

```

### 6.1. So sánh Rule / Workflow / Agent (so trên cùng 1 bài)

| Mức | Phương án cho bài toán nhóm | Khi nào đủ | Rủi ro | Chọn? (Dùng cho bước nào?) |
|---|---|---|---|---|
| **Rule** | | | | |
| **Workflow** | | | | |
| **Agent** | | | | |

**5 câu hỏi chốt (trả lời câu đầy đủ):**
1. Rule có giải được 70-80% case không?
2. Các bước có đi thẳng một đường không hay phải rẽ nhánh?
3. Có thật sự cần Agent tự lập kế hoạch + gọi tool không?
4. Nếu AI sai, ai phát hiện đầu tiên và sửa trong bao lâu?
5. Có hạ được từ Agent → Workflow → Rule không?

**Mức chọn:**

```text
[Rule / Workflow / Agent]
```

**Vì sao chọn (3-4 câu):**

```text

```

**Vì sao không chọn mức đơn giản hơn (2-3 câu):**

```text

```

### 6.2. Problem Statement v1 (v0 sửa chặt hơn + 3 field cuối)

| Field | Nội dung |
|---|---|
| **Actor** | |
| **Workflow** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** | |
| **Boundary** (làm / không làm) | |
| **AI intervention point** (can thiệp sau bước nào, trước bước nào) | |
| **Mức chọn** (Rule / Workflow / Agent + 1 câu vì sao) | |
| **Rủi ro & người thật kiểm tra** (rủi ro lớn nhất + ai kiểm tra bằng cách nào) | |

### 6.3. Final decision

| Câu hỏi | Yes / Not Yet / No | Ghi chú (câu đầy đủ) |
|---|---|---|
| Actor + workflow rõ chưa? | | |
| Baseline + metric đo được chưa? | | |
| Data/input đủ dùng chưa? | | |
| AI sai, hậu quả chấp nhận được không? | | |
| Có người review/owner không? | | |
| Có cách non-AI đơn giản hơn không? | | |

**Decision:**

```text
[Go / Not Yet / No-Go]
```

**Lý do (3-4 câu dựa trên bằng chứng):**

```text

```

**Nếu Go — pilot nhỏ nhất (data nào, chạy tay ra sao, đo 3 số nào):**

```text

```

**Nếu Not Yet — cần validate gì trước:**

```text

```

**Nếu No-Go — làm gì thay AI:**

```text

```

**Exit / rollback (khi nào dừng AI, quay về cách cũ):**

```text

```

---

### Self-check nộp phần 02 (nhóm)
- [ ] Có nhật ký hội tụ 9-12 → 1 (cluster + shortlist + score)
- [ ] Có validation (quote thật) + research (link kiểm được)
- [ ] Có workflow trước/sau đủ thời gian, handoff, bottleneck, boundary, fallback
- [ ] Có PS v0 → v1, metric có trước/sau + cách đo, boundary có làm/không làm
- [ ] Có so sánh Rule/Workflow/Agent + Decision Go/Not Yet/No-Go có lý do
