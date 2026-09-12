# 01 — Individual Problem Scan

> Điền theo Phase 1 + Phase 2 trong `01-worksheet.md`. Tự scan trước, dùng AI sau để phản biện. Không copy ví dụ Weekly Report.

## Thông tin cá nhân

- Họ và tên:
- Mã học viên:
- Vai trò / bối cảnh (VD: sinh viên năm X, intern PM, ...):
- Công việc hằng tuần (3-5 gạch đầu dòng để soi problem):

---

## Phase 1 — Scan 5+ problems (tối thiểu 5, khuyến khích 8-10)

**Cách điền:** mỗi dòng = việc gì + ai chịu + đo bằng gì. Cột `Dấu hiệu thật` bắt buộc có số: mất bao lâu (bấm giờ mấy lần), mấy lần/tuần, bao nhiêu người gặp, log/ticket/quote nào.

| # | Lăng kính (Lặp lại / Tốn thời gian / AI có thể tốt hơn / Pain từ người khác) | Problem quan sát được | Ai chịu ảnh hưởng? | Dấu hiệu thật (số + bằng chứng) |
|---|---|---|---|---|
| 1 | Tốn thời gian | Viết báo cáo kinh doanh hàng tuần | Trưởng phòng Kinh doanh | Mỗi tuần, phòng KD dành ra 30 phút để gom nhặt dữ liệu phù hợp, tổng hợp vào Google Sheets |
| 2 | Tốn thời gian | Quản lý tồn kho và dự trù hàng ngày | Nhân viên bán hàng, Khách hàng | Nhân viên bán hàng dành ra 1 tiếng đầu ngày để kiểm tra tồn kho, đối chiếu với threshold để đặt hàng |
| 3 | Tốn thời gian | Kiểm kê hàng hóa hàng tháng | Nhân viên bán hàng | Một cửa hàng có thể mất nửa ngày (không bán hàng) để kiểm kê toàn bộ hàng hóa trong tủ |
| 4 | Tốn thời gian | Quản lý công nợ & Đối soát | Kế toán | Kế toán mất nhiều giờ để đối soát từng sao kê, lịch sử giao dịch trên nhiều phương tiện giao dịch |
| 5 | AI làm tốt hơn | Hỏi lưu trữ thông tin cá nhân khách hàng | Nhân viên bán hàng | Nhân viên chỉ tập trung vào hỏi thông tin khách hàng, bỏ quên nghiệp vụ bán hàng |

> Gợi ý tự soi: tuần trước mất nhiều thời gian nhất vào việc gì? Việc gì hay trì hoãn? Người khác hay hỏi lại câu gì? Workflow nào ai cũng biết là chậm?

**AI đã dùng ở Phase 1 (nếu có):**
- Prompt đã hỏi: 
- Ý dùng được:
- Ý bỏ vì không phải pain thật:

**Self-check Phase 1:**
- [ ] Đủ 5+ dòng, mỗi dòng có actor + số đo cụ thể
- [ ] Dùng ít nhất 3/4 lăng kính
- [ ] Không có dòng chung chung kiểu "mất nhiều thời gian"

---

## Phase 2 — Top 3 Problem Cards

### 2.1. Chọn top 3

Giữ bài nào: actor cụ thể, workflow vẽ được 3-7 bước, bottleneck ở 1 bước, impact đo được. Loại bài quá rộng.

| Rank | Problem (copy từ bảng scan) | Vì sao chọn (2-3 ý) | Điều còn chưa chắc |
|---|---|---|---|
| 1 | Đối soát thanh toán | Actor cụ thể (Kế toán), vẽ được workflow, impact đo được: Thời gian đối soát | Thông số nào để đánh giá hiệu quả trước và sau khi có giải pháp |
| 2 | Chăm sóc, lưu trữ thông tin khách hàng | | |
| 3 | Quản lý tồn kho và dự trù hàng ngày | | |

### 2.2. Problem Cards chi tiết (lặp lại cho cả 3 cards)

---

#### Problem Card #1 — [Đối soát thanh toán]

```text
Problem 1 câu:

Actor: Nhân viên kế toán nội bộ

Thời điểm / bối cảnh: Kế toán mất quá nhiều thời gian dò đối chiếu thủ công từng khoản tiền gửi ngân hàng với đơn hàng trên hệ thống do khách hàng thường ghi chú chuyển khoản sai cú pháp, dẫn đến chậm trễ tiến độ giao hàng.

Current workflow 3-7 bước:
1. Xuất danh sách đơn hàng chờ thanh toán
2. Tải file sao kê ngân hàng định kỳ
3. Phát hiện có chênh lệch
4. Dò tìm thủ công (match) mã giao dịch/số tiền gây chênh lệch
5. Báo cáo với phòng Kinh doanh

Bottleneck: Bước 4 (dò tìm thủ công). Do có quá nhiều hóa đơn, Kế toán phải đối soát từng hóa đơn/thanh toán một

Impact: Kế toán mát 3 giờ/ngày để đối soát từng sao kê, lịch sử giao dịch trên nhiều phương tiện giao dịch

Success metric: Số giờ làm thủ công giảm từ 3 giờ còn 1 giờ

Non-AI alternative: Sử dụng code cứng để đối chiếu hóa đơn vs. thanh toán/Sử dụng QR code để hóa đơn có invoice ID

AI hypothesis: AI hỗ trợ sắp xếp dữ liệu

Quick gut:
[ ] No AI / process fix
[X] Rule
[X] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #1** (ASCII / Mermaid / ảnh đính kèm):

#### Problem Card #2 — [Chăm sóc, lưu trữ dữ liệu khách hàng]

```text
Problem 1 câu: Nhân viên bán hàng bị giảm hiệu suất và sự kết nối khi phải vật lộn giữa việc duy trì mạch giao tiếp tư vấn với khách hàng và việc ghi chép thủ công thông tin cá nhân, nhu cầu của họ.

Actor: Nhân viên bán hàng trực tiếp

Thời điểm / bối cảnh: Tại không gian cửa hàng vật lý, trong quá trình khách hàng đang xem sản phẩm, đặc biệt là vào các khung giờ cao điểm hoặc trong các phiên tư vấn sản phẩm giá trị cao cần khai thác nhiều thông tin.

Current workflow 3-7 bước:
1. Nhân viên tiếp đón và bắt đầu trò chuyện để tìm hiểu nhu cầu của khách hàng.
2. Khách hàng chia sẻ các thông tin (Tên, số điện thoại, bệnh lý, ngân sách, vấn đề đang gặp phải).
3. Nhân viên xin phép ngắt nhịp giao tiếp để thiết bị ra ghi chép, hoặc chọn cách ghi nhớ trong đầu để tiếp tục nói chuyện.
4. Nhân viên đưa khách đi xem sản phẩm và chốt sale.
5. Sau khi khách hàng thanh toán hoặc rời đi, nhân viên mới ngồi nhớ lại hoặc nhìn sổ nháp để nhập dữ liệu lên hệ thống CRM/phần mềm quản lý.

Bottleneck: Bước 3, 5. Việc cặm cụi ghi chép (bước 3) làm đứt gãy tương tác mắt (eye-contact) và cảm xúc của khách hàng. Nếu để đến cuối mới nhập liệu (bước 5), nhân viên dễ bị quên, nhớ nhầm số điện thoại hoặc sót các chi tiết quan trọng về nhu cầu của khách (nhất là khi phải tiếp nhiều khách liên tục).

Impact: Trải nghiệm khách hàng bị suy giảm (cảm thấy không được chú ý lắng nghe); Thất thoát hoặc sai lệch dữ liệu khách hàng tiềm năng (lead); Giảm hiệu suất phục vụ trong giờ cao điểm.

Success metric: Thời gian thao tác nhập liệu của nhân viên (giảm từ vài phút xuống 0); Tỷ lệ hồ sơ khách hàng bị điền thiếu/sai thông tin (Missing/Error rate); Tỷ lệ chuyển đổi khách hàng tại cửa hàng (Conversion rate).

Non-AI alternative: In sẵn các phiếu điền thông tin (Form) cứng hoặc cung cấp một mã QR để khách hàng tự quét và tự điền thông tin trên điện thoại của họ trong lúc chờ đợi; Hoặc ghép cặp 2 nhân viên cho 1 lượt khách (1 người chuyên tư vấn, 1 người chuyên ghi chép).

AI hypothesis: Trang bị cho nhân viên ứng dụng AI (có khả năng Voice-to-Text và trích xuất thực thể - NER) chạy ngầm để thu thập thông tin (dưới )

Quick gut:
[ ] No AI / process fix
[ ] Rule
[X] Workflow
[ ] Agent
[ ] Chưa biết
```

```text
CURRENT STATE — ___ phút

[1 ...: __'] → [2 ...: __'] → [3 ...: __'] → [4 ...: __']  <-- bottleneck

FUTURE STATE — ___ phút

[1 ...: __'] → [2 ...: __'] → [3 ... review: __']  <-- human boundary

Fallback: nếu AI sai thì ...
```

File đính kèm (nếu vẽ riêng): `01-individual-problem-scan-workflow-card-1.png`

---

#### Problem Card #2 — [Tên problem]

```text
Problem 1 câu:

Actor:

Thời điểm / bối cảnh:

Current workflow 3-7 bước:
1.
2.
3.
4.
5.

Bottleneck:

Impact:

Success metric:

Non-AI alternative:

AI hypothesis:

Quick gut:
[ ] No AI / process fix
[ ] Rule
[ ] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #2:**

```text
CURRENT STATE — ___ phút

[1 ...] → [2 ...] → [3 ...]  <-- bottleneck

FUTURE STATE — ___ phút

[1 ...] → [2 ...] → [3 ... review]  <-- human boundary

Fallback: ...
```

File đính kèm: `01-individual-problem-scan-workflow-card-2.png`

---

#### Problem Card #3 — [Tên problem]

```text
Problem 1 câu:

Actor:

Thời điểm / bối cảnh:

Current workflow 3-7 bước:
1.
2.
3.
4.
5.

Bottleneck:

Impact:

Success metric:

Non-AI alternative:

AI hypothesis:

Quick gut:
[ ] No AI / process fix
[ ] Rule
[ ] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #3:**

```text
CURRENT STATE — ___ phút

[1 ...] → [2 ...] → [3 ...]  <-- bottleneck

FUTURE STATE — ___ phút

[1 ...] → [2 ...] → [3 ... review]  <-- human boundary

Fallback: ...
```

File đính kèm: `01-individual-problem-scan-workflow-card-3.png`

---

### 2.3. Card muốn pitch nhất (chuẩn bị 2 phút)

**Card tôi muốn pitch nhất:**

```text

```

**Vì sao (2-3 câu: workflow gì, số đo gì, impact gì):**

```text

```

**Câu hỏi tôi muốn nhóm challenge (1-2 câu hỏi đúng chỗ yếu):**

```text

```

**AI phản biện Card (nếu có):**
- Điểm yếu AI chỉ ra:
- Tôi sửa gì:

### Self-check nộp phần 01
- [ ] Có 5+ problems + top 3 Cards đủ field
- [ ] Mỗi Card có workflow trước/sau + bottleneck + metric + fallback
- [ ] Đã chọn 1 card pitch + câu hỏi challenge
