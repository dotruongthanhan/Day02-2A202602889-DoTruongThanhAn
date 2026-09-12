# 01 — Individual Problem Scan

> Điền theo Phase 1 + Phase 2 trong `01-worksheet.md`. Tự scan trước, dùng AI sau để phản biện. Không copy ví dụ Weekly Report.

## Thông tin cá nhân

- Họ và tên: Đỗ Trương Thành Ân
- Mã học viên: 2A202602889
- Vai trò / bối cảnh (VD: sinh viên năm X, intern PM, ...): Phụ trách hệ thống công nghệ cho doanh nghiệp bán hàng
- Công việc hằng tuần (3-5 gạch đầu dòng để soi problem): Quan sát quy trình, phỏng vấn các phòng ban (Kinh doanh, Kế toán, Cung ứng, etc.) về công việc hàng ngày của họ, tìm ra những điểm painpoint làm giảm hiệu quả công việc và phát triển sản phẩm công nghệ nội bộ để tăng hiệu quả công việc cho nhân viên. Ví dụ hoạt động:
    - Bán hàng tại điểm
    - Xuất nhập hàng tại kho
    - Đối soát tài chính
    - Báo cáo kinh doanh

---

## Phase 1 — Scan 5+ problems (tối thiểu 5, khuyến khích 8-10)

**Cách điền:** mỗi dòng = việc gì + ai chịu + đo bằng gì. Cột `Dấu hiệu thật` bắt buộc có số: mất bao lâu (bấm giờ mấy lần), mấy lần/tuần, bao nhiêu người gặp, log/ticket/quote nào.

| # | Lăng kính (Lặp lại / Tốn thời gian / AI có thể tốt hơn / Pain từ người khác) | Problem quan sát được | Ai chịu ảnh hưởng? | Dấu hiệu thật (số + bằng chứng) |
|---|---|---|---|---|
| 1 | Tốn thời gian | Viết báo cáo kinh doanh hàng tuần | Trưởng phòng Kinh doanh | Mỗi tuần, phòng KD dành ra 1 tiếng cho mỗi chi nhánh để gom nhặt dữ liệu phù hợp, tổng hợp vào Google Sheets |
| 2 | Tốn thời gian | Quản lý tồn kho và dự trù hàng ngày | Nhân viên bán hàng, Khách hàng | Nhân viên bán hàng dành ra 1 tiếng đầu ngày để kiểm tra tồn kho, đối chiếu với threshold để đặt hàng |
| 3 | Tốn thời gian | Kiểm kê hàng hóa hàng tháng | Nhân viên bán hàng | Một cửa hàng có thể mất nửa ngày (không bán hàng) để kiểm kê toàn bộ hàng hóa trong tủ |
| 4 | Lặp lại | Quản lý công nợ & Đối soát | Kế toán | Khối lượng hóa đơn và thanh toán cần đối chiếu từ hệ thống bán lẻ sang sao kê quá lớn (~700 hóa đơn/ngày), dễ gây nhầm lẫn. |
| 5 | AI làm tốt hơn | Hỏi lưu trữ thông tin cá nhân khách hàng | Nhân viên bán hàng | Nhân viên phải tự ghi nhớ thông tin khách hàng, tự điền lại sau khi bán hàng chỉ còn 70% thông tin |

> Gợi ý tự soi: tuần trước mất nhiều thời gian nhất vào việc gì? Việc gì hay trì hoãn? Người khác hay hỏi lại câu gì? Workflow nào ai cũng biết là chậm?

**AI đã dùng ở Phase 1 (nếu có):**
- Prompt đã hỏi: Hãy gợi ý cho tôi nhũng công việc trong các doanh nghiệp bán hàng vừa và nhỏ thường gặp phải, xoay quanh các công việc lặp lại, tốn thời gian.
- Ý dùng được: Chăm sóc khách hàng, quản lý tồn kho, tài chính & đối soát
- Ý bỏ vì không phải pain thật: Marketing & vận hành truyền thông. Các doanh nghiệp vừa và nhỏ thường không bỏ nhiều chi phí/thu thập nhiều dữ liệu truyền thông --> Không phải pain thật

**Self-check Phase 1:**
- [X] Đủ 5+ dòng, mỗi dòng có actor + số đo cụ thể
- [X] Dùng ít nhất 3/4 lăng kính
- [X] Không có dòng chung chung kiểu "mất nhiều thời gian"

---

## Phase 2 — Top 3 Problem Cards

### 2.1. Chọn top 3

Giữ bài nào: actor cụ thể, workflow vẽ được 3-7 bước, bottleneck ở 1 bước, impact đo được. Loại bài quá rộng.

| Rank | Problem (copy từ bảng scan) | Vì sao chọn (2-3 ý) | Điều còn chưa chắc |
|---|---|---|---|
| 1 | Đối soát thanh toán | Actor cụ thể (Kế toán), vẽ được workflow, impact đo được: Thời gian đối soát | Thông số nào để đánh giá hiệu quả trước và sau khi có giải pháp |
| 2 | Chăm sóc, lưu trữ thông tin khách hàng | Actor cụ thể (Nhân viên bán hàng/CSKH), luồng trích xuất dữ liệu rõ ràng, đo được impact trực tiếp (thời gian nhập liệu, tỷ lệ sai/sót data). | Chưa rõ luồng người dùng để duyệt lại dữ liệu do AI bóc tách (human-in-the-loop) sẽ như thế nào để không làm phát sinh thao tác thừa. |
| 3 | Quản lý tồn kho và dự trù hàng ngày | Actor cụ thể (Quản lý cửa hàng/Thủ kho), giải quyết đúng "điểm mù" độ trễ nhập liệu, metric đo lường rõ ràng (tỷ lệ overselling, thời gian chốt sổ). | Khả năng mở/tích hợp API với các kênh bán (Shopee, TikTok) có thực sự ổn định hay không, giải pháp có bị trùng lặp với các SaaS hiện hành không. |

### 2.2. Problem Cards chi tiết (lặp lại cho cả 3 cards)

---

#### Problem Card #1 — [Đối soát thanh toán]

```text
Problem 1 câu: Kế toán mất quá nhiều thời gian dò đối chiếu thủ công từng khoản tiền gửi ngân hàng với đơn hàng trên hệ thống.

Actor: Nhân viên kế toán nội bộ

Thời điểm / bối cảnh: Kế toán mất quá nhiều thời gian dò đối chiếu thủ công từng khoản tiền gửi ngân hàng với đơn hàng trên hệ thống do khách hàng thường ghi chú chuyển khoản sai cú pháp, dẫn đến chậm trễ tiến độ giao hàng.

Current workflow 3-7 bước:
1. Xuất danh sách đơn hàng chờ thanh toán (10')
2. Tải file sao kê ngân hàng định kỳ (10')
3. Phát hiện có chênh lệch (10')
4. Dò tìm thủ công (match) mã giao dịch/số tiền gây chênh lệch (180-210')
5. Báo cáo với phòng Kinh doanh (10')

- Bottleneck: Bước 4 (dò tìm thủ công). Do có quá nhiều hóa đơn, Kế toán phải đối soát từng hóa đơn/thanh toán một
- Impact: Kế toán mát 3 giờ/ngày để đối soát từng sao kê, lịch sử giao dịch trên nhiều phương tiện giao dịch
- Success metric: Số giờ làm thủ công giảm từ 3 giờ còn 1 giờ
- Non-AI alternative: Sử dụng code cứng để đối chiếu hóa đơn vs. thanh toán/Sử dụng QR code để hóa đơn có invoice ID

AI hypothesis: AI hỗ trợ sắp xếp dữ liệu

Quick gut:
[X] No AI / process fix
[X] Rule
[ ] Workflow
[ ] Agent
[ ] Chưa biết
```

```text
CURRENT STATE — 220 - 250 phút

[1 Xuất danh sách đơn hàng chờ thanh toán: 10'] → [2 Tải file sao kê ngân hàng định kỳ: 10'] → [3 Phát hiện có chênh lệch: 10'] → [4 Dò tìm thủ công mã giao dịch/số tiền gây chênh lệch: 180-210'] <-- bottleneck → [5 Báo cáo với phòng Kinh doanh: 10']

FUTURE STATE — 85 phút

[1 Xuất dữ liệu đơn hàng & sao kê: 10'] → [2 Hệ thống tự đối chiếu (Rule-based: map theo QR code/ID chuẩn + AI: phân tích ngôn ngữ tự nhiên đối với nội dung sai cú pháp để tìm ra khách hàng): 5'] → [3 Kế toán review và xác nhận các giao dịch do AI gợi ý: 60'] <-- human boundary → [4 Báo cáo với phòng Kinh doanh: 10']

Fallback: Nếu AI sai hoặc độ tự tin thấp (không thể suy luận ra người chuyển khoản từ nội dung sai cú pháp) thì giao dịch sẽ được gắn cờ "Ngoại lệ" (Unmatched). Kế toán sẽ chỉ cần dò tìm thủ công cho một nhóm nhỏ các giao dịch này hoặc trực tiếp yêu cầu Sale liên hệ khách hàng để gửi bill xác nhận.
```

---

#### Problem Card #2 — [Chăm sóc, lưu trữ dữ liệu khách hàng]

```text
Problem 1 câu: Nhân viên bán hàng bị giảm hiệu suất và sự kết nối khi phải vật lộn giữa việc duy trì mạch giao tiếp tư vấn với khách hàng và việc ghi chép thủ công thông tin cá nhân, nhu cầu của họ.

Actor: Nhân viên bán hàng trực tiếp

Thời điểm / bối cảnh: Tại không gian cửa hàng vật lý, trong quá trình khách hàng đang xem sản phẩm, đặc biệt là vào các khung giờ cao điểm hoặc trong các phiên tư vấn sản phẩm giá trị cao cần khai thác nhiều thông tin.

Current workflow 3-7 bước:
1. Nhân viên tiếp đón và bắt đầu trò chuyện để tìm hiểu nhu cầu của khách hàng. (1')
2. Khách hàng chia sẻ các thông tin (Tên, số điện thoại, bệnh lý, ngân sách, vấn đề đang gặp phải). (5')
3. Nhân viên xin phép ngắt nhịp giao tiếp để thiết bị ra ghi chép. (3')
4. Nhân viên đưa khách đi xem sản phẩm và chốt sale (5').
5. Sau khi khách hàng thanh toán hoặc rời đi, nhân viên mới ngồi nhớ lại hoặc nhìn sổ nháp để nhập dữ liệu lên hệ thống CRM/phần mềm quản lý (5').

- Bottleneck: Bước 3, 5. Việc cặm cụi ghi chép (bước 3) làm đứt gãy tương tác mắt (eye-contact) và cảm xúc của khách hàng. Nếu để đến cuối mới nhập liệu (bước 5), nhân viên dễ bị quên, nhớ nhầm số điện thoại hoặc sót các chi tiết quan trọng về nhu cầu của khách (nhất là khi phải tiếp nhiều khách liên tục).
- Impact: Trải nghiệm khách hàng bị suy giảm (cảm thấy không được chú ý lắng nghe); Thất thoát hoặc sai lệch dữ liệu khách hàng tiềm năng (lead); Giảm hiệu suất phục vụ trong giờ cao điểm.
- Success metric: Thời gian nhập liệu của nhân viên (giảm từ vài phút xuống 0); Tỷ lệ hồ sơ khách hàng bị điền thiếu/sai thông tin (Missing/Error rate); Tỷ lệ chuyển đổi khách hàng tại cửa hàng (Conversion rate).
- Non-AI alternative: In sẵn các phiếu điền thông tin (Form) cứng hoặc cung cấp một mã QR để khách hàng tự quét và tự điền thông tin trên điện thoại của họ trong lúc chờ đợi; Hoặc ghép cặp 2 nhân viên cho 1 lượt khách (1 người chuyên tư vấn, 1 người chuyên ghi chép).
- AI hypothesis: Trang bị cho nhân viên ứng dụng AI (có khả năng Voice-to-Text và trích xuất thực thể - Named Entity Recognition) chạy ngầm để thu thập thông tin

Quick gut:
[ ] No AI / process fix
[ ] Rule
[X] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #2:**

```text
CURRENT STATE — 19 phút

[1 Tiếp đón và trò chuyện tìm hiểu nhu cầu: 1'] → [2 Khách hàng chia sẻ thông tin cá nhân và vấn đề: 5'] → [3 Ngắt nhịp giao tiếp để ghi chép thủ công: 3'] <-- bottleneck → [4 Đưa đi xem sản phẩm và chốt sale: 5'] → [5 Nhớ lại/nhìn sổ nháp để nhập liệu lên hệ thống CRM: 5'] <-- bottleneck

FUTURE STATE — 12 phút

[1 Tiếp đón & trò chuyện (Bật app AI chạy ngầm): 1'] → [2 Khách chia sẻ thông tin (AI tự động thu âm, chuyển đổi giọng nói thành văn bản và trích xuất thực thể vào các trường dữ liệu): 5'] → [3 Đưa khách xem sản phẩm và chốt sale: 5'] → [4 Nhân viên review và xác nhận hồ sơ khách hàng trên CRM: 1'] <-- human boundary

Fallback: Nếu AI sai (do môi trường cửa hàng quá ồn, khách nói giọng địa phương khó nghe hoặc AI nhận diện nhầm số điện thoại/tên bệnh lý), nhân viên sẽ trực tiếp chỉnh sửa thủ công các trường dữ liệu bị điền sai trên form trong bước review (bước 4). Hệ thống cũng lưu lại bản ghi âm gốc để nhân viên có thể bấm nghe lại ngay đoạn thông tin bị nghi ngờ mà không cần phải gọi điện hỏi lại khách hàng.
```

File đính kèm: `01-individual-problem-scan-workflow-card-2.png`

---

#### Problem Card #3 — [Tên problem]

```text
Problem 1 câu: Quản lý cửa hàng mất nhiều thời gian chốt sổ và thường xuyên gặp tình trạng bán vượt mức (overselling) do độ trễ trong việc tổng hợp và cập nhật tồn kho thủ công từ nhiều kênh bán hàng (Shopee, TikTok, offline).

Actor: Quản lý cửa hàng / Thủ kho

Thời điểm / bối cảnh: Cuối ngày làm việc khi cần chốt sổ kho hoặc trong các đợt flash sale/chiến dịch khuyến mãi khi lượng đơn hàng tăng đột biến trên đa kênh.

Current workflow 3-7 bước:
1. Đăng nhập vào từng kênh bán (Shopee, TikTok, phần mềm POS) để xuất file báo cáo đơn hàng. (15')
2. Tải và gom các file Excel dữ liệu về một máy tính. (5')
3. Tổng hợp số liệu, đối chiếu số lượng đã bán với số lượng tồn thực tế trên file Excel tổng. (45')
4. Chỉnh sửa và cập nhật lại số lượng tồn kho mới lên từng kênh bán hàng để tránh overselling. (30')
5. Lập dự trù nhập hàng cho ngày tiếp theo dựa trên cảm tính hoặc số bán trung bình. (20')

- Bottleneck: Bước 3 và Bước 4. Việc gom file và đối chiếu thủ công tạo ra độ trễ nhập liệu lớn, khiến tồn kho trên sàn không khớp với thực tế, gây ra overselling.
- Impact: Gây mất uy tín với khách hàng, shop bị phạt/tắt hiển thị do hủy đơn trên sàn TMĐT; thủ kho tốn gần 2 tiếng mỗi ngày cho việc chốt sổ.
- Success metric: Tỷ lệ overselling giảm xuống < 1%; Thời gian chốt sổ và lập dự trù giảm từ 115 phút xuống < 15 phút.
- Non-AI alternative: Thuê/mua các phần mềm quản lý bán hàng (SaaS) có sẵn tính năng đồng bộ API đa kênh (tuy nhiên phụ thuộc vào độ ổn định API của sàn).
- AI hypothesis: Ứng dụng RPA kết hợp AI để tự động đọc/trích xuất dữ liệu từ các báo cáo đa kênh (khắc phục điểm yếu API không ổn định), tự động đối chiếu tồn kho và dùng AI dự báo nhu cầu (demand forecasting) để đề xuất lượng hàng cần dự trù chính xác thay vì dự đoán cảm tính.

Quick gut:
[ ] No AI / process fix
[X] Rule
[X] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #3:**

```text
CURRENT STATE — 115 phút

[1 Xuất và tải báo cáo từ các kênh (Shopee, TikTok, POS): 20'] → [2 Đối chiếu tổng hợp tồn kho thủ công trên Excel: 45'] <-- bottleneck → [3 Cập nhật tồn kho ngược lên sàn & dự trù nhập hàng: 50'] <-- bottleneck

FUTURE STATE — 15 phút

[1 RPA tự động lấy dữ liệu và hợp nhất số liệu bán hàng đa kênh: 5'] → [2 AI tự động tính toán tồn kho hiện tại và lập bảng dự trù nhập hàng cho ngày mai: 5'] → [3 Quản lý review bảng tồn kho & số lượng dự trù nhập hàng do AI đề xuất để duyệt: 5' review] <-- human boundary

Fallback: Nếu hệ thống đồng bộ lỗi (do giao diện sàn thay đổi hoặc API hỏng) hoặc AI đưa ra dự báo số lượng nhập hàng bất thường, hệ thống sẽ phát cảnh báo. Thủ kho sẽ tải file Excel thủ công đưa vào hệ thống xử lý (Rule-based) và tự quyết định số lượng dự trù theo kinh nghiệm.
```

---

### 2.3. Card muốn pitch nhất (chuẩn bị 2 phút)

**Card tôi muốn pitch nhất:**

```text
Chăm sóc, lưu trữ dữ liệu khách hàng
```

**Vì sao (2-3 câu: workflow gì, số đo gì, impact gì):**

```text
Workflow: [1 Tiếp đón & trò chuyện (Bật app AI chạy ngầm): 1'] → [2 Khách chia sẻ thông tin (AI tự động thu âm, chuyển đổi giọng nói thành văn bản và trích xuất thực thể vào các trường dữ liệu): 5'] → [3 Đưa khách xem sản phẩm và chốt sale: 5'] → [4 Nhân viên review và xác nhận hồ sơ khách hàng trên CRM: 1'] <-- human boundary

Số đo: Thời gian nhập liệu của nhân viên (giảm từ vài phút xuống 0); Tỷ lệ hồ sơ khách hàng bị điền thiếu/sai thông tin (Missing/Error rate); Tỷ lệ chuyển đổi khách hàng tại cửa hàng (Conversion rate).
```

**Câu hỏi tôi muốn nhóm challenge (1-2 câu hỏi đúng chỗ yếu):**

```text
1. Khách hàng từ chối ghi âm thì phải xử lý như thế nào?
2. Phải xử lý ra sao với giọng địa phương?
```

**AI phản biện Card (nếu có):**
- Điểm yếu AI chỉ ra: Nhiều khách hàng sẽ từ chối nếu sales yêu cầu bật ghi âm toàn bộ cuộc trò chuyện.
- Tôi sửa gì: Tôi và nhóm đã thống nhất 1 phương án: Hệ thống hỗ trợ 2 chế độ:
    - Mode 1: Ghi âm trực tiếp khi khách đồng ý
    - Mode 2: Sales dành 60 giây ngay sau khi tiễn khách để thu một Voice Note tóm tắt nhanh bằng lời của chính mình — AI sẽ trích xuất từ voice note này vào CRM.

### Self-check nộp phần 01
- [X] Có 5+ problems + top 3 Cards đủ field
- [X] Mỗi Card có workflow trước/sau + bottleneck + metric + fallback
- [X] Đã chọn 1 card pitch + câu hỏi challenge
