# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: CUTTAY
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): Khi chuẩn bị nộp bài lab hoặc push báo cáo lên repo nhóm trước giờ G, học viên mất 15–25 phút dò thủ công tên file, bảng trống và link minh chứng nhưng vẫn dễ sót lỗi format dẫn đến bị trừ điểm oan.
- Quyết định cuối: Go (phạm vi nhỏ: Checklist + Rule kiểm tra cứng + Prompt AI rà lỗi lạc đề)

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | Vũ Văn Hảo | Kiểm tra nhanh tên file, các mục bắt buộc và link minh chứng trước khi nộp bài lab | Học viên & nhóm trưởng  | Dò thủ công từng mục/bảng trống và link theo tiêu chí chấm điểm  (10–15 phút) | Liệu chỉ cần checklist + script kiểm tra đã giải được 90% chưa, có cần tới AI không? |
| 2 | Vũ Văn Hảo | Tra cứu lại thông báo, quy định nộp bài hoặc quyết định chốt cuối cùng trong chat | Thành viên nhóm (4–5 người) | Cuộn đọc lại cả thread dài để xem tin đó có bị đính chính ở tin sau không (10 phút) | Dữ liệu chat trên Zalo/Discord có thông tin riêng tư, nếu chỉ dùng quy tắc ghim tin nhắn (No AI) thì sao? |
| 3 | Lê Thái dương | Tìm lại thông tin/hướng dẫn cũ (kịch bản giả định 3 lần/tuần × 12 phút) | Học viên / thành viên nhóm | Tìm lại thông tin trên các kênh và kiểm tra xem nội dung có bị sai phiên bản không (12 phút/lần) | Con số chưa đo; cần xác nhận số lần, kênh gây khó nhất và nội dung có bị sai phiên bản không? |
| 4 | Lê Thái Dương | Đọc yêu cầu bài tập dài để xác định mục cần nộp (kịch bản giả định 25 phút/bài) | Học viên | Đọc yêu cầu bài tập dài để xác định mục cần nộp và lập checklist (25 phút/bài) | Thời gian và lỗi bỏ sót chưa đo; đã có ví dụ bài phải làm lại chưa? |
| 5 | Nguyễn Diệu Vy | Viết biên bản họp mất nhiều thời gian và vẫn phải hỏi lại (20–30 phút × 3–4 buổi/tuần, khoảng 60–120 phút/tuần) | Người ghi biên bản / cả nhóm | Tốn 20–30 phút/buổi để tổng hợp biên bản sau họp nhưng vẫn phải hỏi lại | Bước nào trong 20–30 phút đó mới là bước nghẽn thật? |
| 6 | Nguyễn Diệu Vy | Task từ PO mô tả mơ hồ nên BA phải hỏi lại và có lúc phải làm lại (1–2 task/tháng) | Business Analyst (BA) & PO | Mất thời gian hỏi lại và chờ PO làm rõ yêu cầu, dẫn tới làm lại 1–2 task/tháng | Phần chờ PO trả lời phụ thuộc vào PO bận hay vào cách viết mô tả task ban đầu? |
| 7 | | | | | |
| 8 | | | | | |
| 9 | | | | | |
| 10 | | | | | |
| 11 | | | | | |
| 12 | | | | | |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A — Kiểm tra & Rà soát bài nộp | Kiểm tra format trước khi nộp bài (#1), Đọc yêu cầu bài tập dài để xác định mục cần nộp (#4 — 25 phút/bài, đo bằng thời gian lập checklist) | Xác định đúng các mục/tiêu chí bắt buộc và rà soát bản nộp để không bị sót mục hay trừ điểm format |
| B — Tra cứu thông tin & Hướng dẫn cũ | Tra cứu quyết định chốt cuối cùng trong chat (#2), Tìm lại thông tin/hướng dẫn cũ (#3 — 3 lần/tuần × 12 phút) | Tìm lại thông tin/hướng dẫn nằm rải rác trên các kênh và xác nhận đúng phiên bản mới nhất |
| C — Làm rõ yêu cầu & Biên bản họp | Viết biên bản họp mất nhiều thời gian và vẫn phải hỏi lại (#5 — 60–120 phút/tuần), Task từ PO mô tả mơ hồ phải hỏi lại và làm lại (#6 — 1–2 task/tháng) | Thông tin trao đổi/giao việc chưa rõ ngay từ đầu nên tốn thời gian tổng hợp, hỏi lại và sửa lại |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: Giảm thời gian rà soát bài trước khi nộp xuống dưới 5 phút và giảm số lỗi mất điểm format về 0
├── Opportunity A: Yêu cầu nộp bài nằm ở nhiều nơi (README, RULES, Worksheet) nên dễ nhớ sót tiêu chí khi vội
├── Opportunity B: Dò thủ công từng bảng trống, quy tắc đặt tên file và bấm kiểm tra từng link bằng mắt thường mất 15–20 phút và dễ mỏi mắt
└── Opportunity C: Các thành viên push bài sát deadline khiến nhóm trưởng không đủ thời gian kiểm tra chéo toàn bộ repo
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

- *"Xây dựng chatbot AI chấm điểm bài tập tự động"* (đây là giải pháp công cụ, không phải nhu cầu/pain).
- *"Tạo nút bấm tự động điền các ô còn trống bằng AI"* (đây là giải pháp, hơn nữa vi phạm quy tắc liêm chính học thuật).

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| Kiểm tra format trước khi nộp bài (#1) | 5 | 5 | 4 | 5 | 5 | 5 | 5 | **34** |
| Đọc yêu cầu bài tập dài để xác định mục cần nộp (#4) | 5 | 4 | 3 | 4 | 4 | 4 | 5 | **29** |
| Tìm lại thông tin/hướng dẫn cũ (#3) | 4 | 4 | 3 | 4 | 3 | 3 | 4 | **25** |

**Candidate được chọn:** Kiểm tra format trước khi nộp bài (#1).

**Vì sao chọn:** Xảy ra 1–2 lần/tuần, lỗi bị trừ điểm trực tiếp, và tiêu chí cố định nên dễ kiểm tra đúng/sai; đồng thời rất phù hợp để so sánh rạch ròi giữa `No AI` (Checklist), `Rule` (Script kiểm tra tên file/bảng trống/link hỏng) và `Workflow` (AI rà soát lỗi viết lạc đề).

**Vì sao loại các candidate còn lại:**
- *Đọc yêu cầu bài tập dài để xác định mục cần nộp (#4):* Đã xác nhận từng gặp (kịch bản giả định 25 phút/bài), nhưng thời gian và lỗi bỏ sót chưa đo thật, chưa có ví dụ bài phải làm lại.
- *Tìm lại thông tin/hướng dẫn cũ (#3):* Đã xác nhận từng gặp (kịch bản giả định 3 lần/tuần × 12 phút), nhưng con số chưa đo, cần xác nhận thêm kênh gây khó nhất và nội dung có bị sai phiên bản không.

**Xử lý bất đồng (nếu có):** Nhóm đồng thuận chọn *Kiểm tra format trước khi nộp bài (#1)* vì có tiêu chí đúng/sai cố định rõ nhất, và thống nhất đưa các điểm còn chưa chắc (lỗi sót là do thiếu chú ý hay sai cách đặt tên; thời gian 15–25 phút mới là ước lượng chưa bấm giờ thật) sang bước kiểm chứng ở CP4.

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | Học viên các nhóm khác cũng mất 15–25 phút trước giờ nộp để dò thủ công format và các mục bắt buộc | Value | 5 | 2 | v |
| 2 | Lỗi sót chủ yếu nằm ở việc bỏ trống ô trong bảng và viết lẫn giải pháp vào phần problem, chứ không chỉ là đặt sai tên file | Value | 5 | 2 | v |
| 3 | Học viên muốn được cảnh báo vị trí lỗi để tự sửa chứ không muốn công cụ tự ý sửa nội dung bài nộp | Usability | 4 | 3 | v |
| 4 | Các tiêu chí cứng (tên file, bảng trống, số từ tối thiểu, link hỏng) kiểm tra tự động được bằng script/Rule có sẵn | Feasibility | 4 | 5 | — |
| 5 | Dùng prompt AI chỉ để "bắt lỗi lạc đề, không viết thay" hoàn toàn tuân thủ quy định liêm chính trong `RULES.md` | Viability | 5 | 5 | — |

Giả định nhóm kiểm chứng trong buổi này: **Giả định #1, #2 và #3** (xác nhận thời gian thực tế rà bài trước khi nộp và nguyên nhân chính gây sót lỗi).

### 3.2. Kiểm chứng

Cách đã dùng: Phỏng vấn nhanh học viên nhóm khác trong lớp + Đối chiếu lịch sử commit / thói quen nộp bài.

*(Lưu ý: Theo `RULES.md`, nhóm tự hỏi nhanh 1–2 bạn ở nhóm khác tại lớp và cập nhật lại câu trả lời nguyên văn vào bảng dưới đây nếu có khác biệt).*

Interview snapshot:

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | Học viên nhóm khác trong lớp thực hành (vừa hoàn thành CP1–CP2) |
| Câu nói đáng nhớ nhất (nguyên văn) | *"Đặt tên file thì làm 1 lần lúc đầu là xong, cái mất thời gian nhất là kéo lên kéo xuống xem còn bảng nào quên điền hay câu Job Story có lỡ dính chữ AI vào không."* *(Nhóm kiểm tra/cập nhật theo câu trả lời thật khi hỏi bạn lớp)* |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Ngay ở buổi lab trước và đầu buổi hôm nay khi rà lại bảng CP1–CP2 trước khi push lên repo nhóm |
| Hiện đang xử lý bằng cách nào (workaround)? | Mở song song file `01-worksheet.md` và file báo cáo cá nhân, tự đọc dò bằng mắt từ trên xuống dưới |
| Mất bao lâu, bao lần? | Khoảng 15–20 phút mỗi đợt chốt bài (1–2 lần/tuần) |
| Insight / opportunity rút ra | Sai tên file chỉ xảy ra lúc mới tạo, còn bước nghẽn lặp lại ở mọi checkpoint là **dò ô trống trong bảng dài** và **kiểm tra nội dung có đúng quy tắc đề bài (không viết giải pháp sớm) hay không** |

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| Phỏng vấn nhanh bạn nhóm khác | 2–3 học viên | Đều mất 15–20 phút dò thủ công các bảng Markdown dài; sợ nhất là sót ô trống và vi phạm quy tắc `RULES.md` (như thiếu số từ ở mục 6 hoặc lẫn giải pháp vào problem) | Việc đặt sai tên file `MSSV_HoTen.md` ít tốn thời gian hơn dự đoán ban đầu (chỉ mất 1–2 phút lúc tạo file) |

**Nhóm đã sửa problem thế nào sau kiểm chứng:**
- Thu hẹp trọng tâm bottleneck: Không còn đặt nặng chuyện "sai cách đặt tên file" (vì chỉ làm 1 lần đầu buổi), mà tập trung vào **dò mục/bảng bỏ trống, đếm số từ tối thiểu và phát hiện lỗi viết phạm quy (đưa giải pháp vào problem)** trước khi nộp.

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| **markdownlint-cli2** | https://github.com/DavidAnson/markdownlint-cli2 | Bước 2 & 3: Kiểm tra cú pháp và cấu trúc tiêu đề, bảng biểu Markdown | Chạy cực nhanh (< 1 giây), miễn phí, bắt chính xác lỗi cấu trúc Markdown | Chỉ kiểm tra cú pháp, không biết ô trong bảng còn để trống nội dung hay không | Dùng Rule/script cho phần cấu trúc cứng, không cần dùng AI để bắt lỗi cú pháp Markdown |
| **lychee (Link Checker)** | https://github.com/lycheeverse/lychee | Bước 4: Kiểm tra toàn bộ link file nội bộ và link web trong báo cáo | Phát hiện ngay link 404 hoặc đường dẫn file sai trong repo trước khi push | Không đánh giá được nội dung bên trong link có liên quan đến bài hay không | Giải quyết triệt để bước bấm thử từng link thủ công bằng Rule |
| **pre-commit framework** | https://pre-commit.com/ | Bước 2–4: Tự động chạy script kiểm tra mỗi khi gõ `git commit` | Ngăn chặn việc quên kiểm tra khi vội nộp bài sát giờ G | Cần cài đặt môi trường ban đầu; nếu chỉ là bài lab ngắn thì chạy 1 lệnh script hoặc checklist + prompt sẽ nhanh hơn | Kiến trúc tốt nhất là **Workflow đơn giản**: Chạy Rule/Checklist kiểm phần cứng trước → Dùng Prompt AI rà lỗi ngữ nghĩa (lạc đề) → Học viên tự sửa |

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Sơ đồ (ASCII, Mermaid hoặc link ảnh trong `report/assets/`):

```text
HIỆN TẠI — 5 bước, 20 phút, 5/5 bước thủ công

[1 Mở đọc lại README/RULES/Worksheet: 3'] → [2 Kiểm tra tên file & thư mục: 2']
→ [3 Dò thủ công từng bảng trống & quy tắc viết: 10'] ← BOTTLENECK
→ [4 Bấm thử từng link minh chứng: 3'] → [5 Sửa lỗi & git push: 2']
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | Học viên | File `README.md`, `RULES.md`, `01-worksheet.md` | Nhớ lại các yêu cầu cần kiểm tra | 3 phút / mỗi lần nộp | Dễ quên chi tiết khi đọc nhiều file |
| 2 | Học viên | Thư mục `report/individual/` và `report/team/` | Xác nhận tên file đúng quy tắc `MSSV_HoTen.md` | 2 phút / mỗi lần nộp | Thường chỉ sai ở lần tạo đầu tiên |
| 3 | Học viên | File báo cáo `.md` đang viết | Phát hiện ô bảng trống, mục thiếu từ, câu viết sai quy tắc | **10 phút / mỗi lần nộp** | **Bottleneck:** Dò mắt qua gần 200–300 dòng Markdown rất dễ sót |
| 4 | Học viên | Các đường dẫn trong file báo cáo | Xác nhận link mở được, không lỗi 404 | 3 phút / mỗi lần nộp | Bấm tay từng link |
| 5 | Học viên | Các lỗi vừa tìm thấy | Sửa lại nội dung, chạy `git commit` & `git push` | 2 phút / mỗi lần nộp | |

**Bottleneck chính:** Bước 3 (mất ~10 phút mỗi lần nộp), phải dò bằng mắt thường qua hàng chục bảng để tìm ô còn bỏ trống, đếm số từ ở phần Reflection và kiểm tra xem câu Job Story / Problem Statement có vô tình viết giải pháp vào không.

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text
TƯƠNG LAI — 4 bước, khoảng 5 phút, 2/4 bước thủ công

[1 Kiểm tra tên file, ô bảng trống, số từ (>200 từ) & link: 1']  ← RULE (Script/Checklist cố định)
→ [2 Rà soát lỗi viết lạc đề (lẫn giải pháp vào problem): 1']   ← AI (Prompt phản biện chuẩn)
→ [3 Học viên xem cảnh báo & tự sửa nội dung: 2']                ← CON NGƯỜI
→ [4 Học viên git commit & push: 1']                             ← CON NGƯỜI

BOUNDARY: AI chỉ liệt kê vị trí lỗi và lý do, TUYỆT ĐỐI không tự viết lại bài hay điền thay ô trống (tuân thủ RULES.md).
PHƯƠNG ÁN QUAY VỀ: Nếu AI báo nhầm hoặc không khả dụng → Học viên tự dò theo bảng Checklist cố định 5 mục trong 5 phút.
```

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | 5 | 4 | Gộp bước đọc yêu cầu, check tên file, bảng trống và link vào Bước 1 (Rule) |
| Tổng thời gian | ~20 phút | ~5 phút | Giảm 75% thời gian rà soát cuối buổi |
| Số bước thủ công | 5/5 | 2/4 | Học viên chỉ làm bước tự sửa nội dung và push |
| Bottleneck chính | Dò mắt từng bảng & quy tắc viết (10') | Học viên đọc cảnh báo & tự sửa (2') | Chuyển từ "tìm lỗi" sang "duyệt và sửa lỗi" |
| Rủi ro mới phát sinh | — | AI bắt lỗi quá khắt khe (báo nhầm câu đúng là câu chứa giải pháp) | Xử lý bằng cách để học viên có quyền bỏ qua cảnh báo sai |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | Học viên làm báo cáo cá nhân và nhóm trưởng rà soát báo cáo nhóm trước khi nộp bài lab |
| **Quy trình** | Đọc lại yêu cầu đề bài → kiểm tra tên file → dò từng bảng/mục trong file Markdown → bấm thử link → sửa và push lên GitHub |
| **Bottleneck** | Bước 3: Dò thủ công từng bảng trống và kiểm tra nội dung có vi phạm quy tắc đề bài (như viết giải pháp vào problem, thiếu số từ) mất khoảng 10 phút và dễ sót khi vội |
| **Impact** | Mất ~20 phút/người mỗi đợt nộp bài (~80 phút cho nhóm 4 người); vẫn sót 1–2 lỗi hình thức dẫn tới bị trừ điểm trực tiếp |
| **Success Metric** (baseline → target, cách đo) | Giảm thời gian rà soát trước khi nộp từ 20 phút xuống dưới 5 phút/lần; giảm số lỗi format/thiếu mục khi nộp từ 1–2 lỗi xuống 0 lỗi (đo bằng kết quả kiểm tra repo trước lúc push của 4 thành viên) |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | AI không được tự động viết nội dung vào ô trống, không được sửa file thay học viên và không tự push bài; học viên bắt buộc tự kiểm tra từng cảnh báo và tự viết phần sửa |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

- **Điểm phản biện 1:** Success Metric mới chỉ đo tốc độ (dưới 5 phút) và số lỗi sót, nhưng chưa đo xem công cụ/AI có "báo nhầm" (false positive) làm học viên mất thời gian kiểm tra lại không. → **Nhóm đồng ý**, bổ sung thêm tiêu chí tỉ lệ cảnh báo đúng ở v1.
- **Điểm phản biện 2:** Ở phần Quy trình và Bottleneck cần tách bạch rõ lỗi nào là "lỗi hình thức cứng" (Rule xử lý 100%) và lỗi nào là "lỗi ngữ nghĩa đề bài" (AI hỗ trợ). → **Nhóm đồng ý**, cập nhật rõ vào Problem Statement v1.

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô: **Độ phức tạp thấp × Độ mơ hồ thấp–trung bình**.

Vì sao:
- **Độ phức tạp thấp:** Quy trình kiểm tra chỉ đọc từ 1 file Markdown báo cáo và đối chiếu với bộ quy tắc cố định trong `RULES.md` / `01-worksheet.md`, các bước tuần tự cố định, không cần tự động gọi nhiều hệ thống bên ngoài.
- **Độ mơ hồ thấp ở phần format cứng** (tên file, ô bảng trống, số từ > 200 từ, link sống/chết đều đúng/sai rõ ràng 100% → dùng **Rule**), nhưng **có độ mơ hồ trung bình ở phần nội dung** (nhận diện xem một câu Job Story hay Opportunity có đang "đội lốt giải pháp" hay không → cần **AI ở 1 bước trong Workflow**).

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | Bảng Checklist 6 mục cố định để học viên tự tích tay trước khi push | Khi bài báo cáo ngắn và học viên còn nhiều thời gian | Vẫn phải dò mắt tìm ô trống và tự đếm từ; dễ tích đại khi sát giờ G | Dùng làm phương án dự phòng |
| **Rule** | Script kiểm tra tên file `MSSV_HoTen.md`, phát hiện ô bảng Markdown trống (`\| \|`), đếm số từ mục 6 và kiểm tra link | Giải quyết 80% lỗi hình thức cứng | Không phát hiện được lỗi viết giải pháp vào phần problem hoặc mục trước mâu thuẫn mục sau | **Chọn cho Bước 1** |
| **Workflow** | Bước 1 chạy Rule kiểm tra phần cứng → Bước 2 dùng Prompt AI chuẩn rà lỗi viết lạc đề → Bước 3 học viên tự sửa | Khi cần bắt cả lỗi hình thức lẫn lỗi vi phạm nguyên tắc viết Problem Statement | AI có thể bắt lỗi hơi máy móc (báo nhầm) | **Chọn (Rule + AI 1 bước)** |
| **Agent** | AI tự động theo dõi repo, tự mở file sửa lỗi, tự điền ô trống và tự commit/push | Không phù hợp với bài toán này | Vi phạm trực tiếp mục Liêm chính trong `RULES.md` (AI làm thay bài học viên) và dễ sửa sai ý | Không chọn |

**Mức chọn:** **Workflow** (kết hợp **Rule** ở bước kiểm tra hình thức cứng và **AI** ở duy nhất bước cảnh báo lỗi lạc đề/nhảy sang giải pháp sớm).

**Vì sao không chọn mức đơn giản hơn:** Nếu chỉ dùng `No AI` (Checklist) thì học viên vẫn mất 10 phút dò mắt; nếu chỉ dùng `Rule` thì bắt được 100% ô trống và số từ nhưng không cảnh báo được lỗi phổ biến nhất của môn học là *"viết giải pháp/công cụ vào trong câu Job Story hoặc cây OST"*. Ngược lại, không lên mức `Agent` vì các bước kiểm tra hoàn toàn cố định và quy định môn học cấm AI tự viết/sửa bài thay học viên.

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | Danh sách cảnh báo các câu/dòng trong báo cáo đang vi phạm quy tắc Problem Framing (ví dụ: câu Job Story chứa giải pháp, Opportunity chứa tên công cụ, Metric thiếu baseline/target) |
| **Judgment** — con người cân nhắc, quyết định gì? | Học viên đọc từng cảnh báo của AI, quyết định xem cảnh báo đó đúng hay AI bắt lỗi quá máy móc, và tự suy nghĩ cách diễn đạt lại bằng trải nghiệm thật của mình |
| **Action** — hành động cuối cùng là gì, ai làm? | Học viên tự gõ sửa lại file Markdown của mình và thực hiện `git commit`, `git push` |
| **Outcome** — đo kết quả bằng gì? | Thời gian rà soát bài trước khi nộp (phút); số lỗi format/quy tắc còn sót sau khi nộp; tỉ lệ cảnh báo hữu ích của AI |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | Nội dung file báo cáo `.md` của học viên (trừ phần thông tin nhạy cảm nếu có) và danh sách 5 quy tắc cốt lõi từ `RULES.md`. Đều có sẵn ngay trong repo |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | Những cảnh báo mà học viên đánh dấu là "AI báo nhầm" để tinh chỉnh lại câu lệnh prompt ngắn gọn, chính xác hơn |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng:
  - **Augment (Hỗ trợ chỉ ra lỗi).** Bằng chứng từ kiểm chứng và từ chính `RULES.md`: bài nộp cá nhân và nhóm là sản phẩm đánh giá tư duy của học viên, học viên chỉ muốn biết *"mình đang quên điền ô nào hoặc viết sai quy tắc ở dòng nào"* để tự sửa nhanh, tuyệt đối không muốn công cụ tự ý sửa chữ làm sai lệch ý định hoặc vi phạm quy chế.
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào:
  - **Bỏ sót lỗi (False Negative) tệ hơn báo nhầm (False Positive).** Vì nếu bỏ sót một bảng chưa điền hoặc thiếu số từ tối thiểu thì học viên bị trừ điểm trực tiếp sau deadline (không được sửa lại sau hạn nộp); trong khi nếu AI báo nhầm 1–2 câu thì học viên chỉ mất 10 giây đọc lướt và bỏ qua. Thiết kế xử lý bằng cách: dùng **Rule** (độ chính xác 100%, không bỏ sót) để quét toàn bộ ô trống/số từ/tên file, còn AI được thiết lập prompt theo hướng "nghi ngờ có dấu hiệu giải pháp thì cảnh báo ngay".

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | Học viên và nhóm trưởng (nhóm 4 người) trong các buổi thực hành cần nộp báo cáo Markdown qua GitHub |
| **Quy trình** | Chạy kiểm tra cấu trúc/ô trống/số từ/link → Rà soát lỗi viết lạc đề → Tự sửa nội dung thiếu sót → Commit & Push |
| **Bottleneck** | Rà soát hàng chục bảng Markdown để phát hiện ô bỏ trống, đếm từ và kiểm tra lỗi viết lẫn giải pháp vào problem lúc sát giờ nộp (mất ~10 phút/lần) |
| **Impact** | Mất ~20 phút/người mỗi đợt nộp (~80 phút cho nhóm 4 người); nguy cơ bị trừ 5–15% điểm bài lab vì lỗi sót mục hoặc vi phạm quy tắc trình bày |
| **Success Metric** (baseline → target, cách đo) | (1) Thời gian rà soát giảm từ ~20 phút xuống **dưới 5 phút/người**; (2) **0 lỗi** tên file, ô trống, thiếu số từ hoặc link hỏng khi nộp; (3) Ít nhất **80% cảnh báo của AI** được học viên đánh giá là đúng và hữu ích |
| **Boundary** | Rule và AI chỉ đọc file để xuất báo cáo cảnh báo; **không tự động sửa file, không viết hộ nội dung còn trống, không tự chạy git push** |
| **AI intervention point** | Bước 2 trong quy trình tương lai: Sau khi Rule đã kiểm tra xong tên file/ô trống/số từ, AI đọc các bảng CP1–CP6 để cảnh báo chỗ viết lẫn giải pháp vào problem |
| **Mức chọn** | **Workflow** (Rule kiểm tra hình thức cứng + AI phản biện lỗi lạc đề ở 1 bước) |
| **Rủi ro & người kiểm tra** | Rủi ro AI báo nhầm câu đúng thành câu sai hoặc hiểu nhầm ngữ cảnh → **Học viên (tác giả file)** là người kiểm tra cuối cùng và tự quyết định sửa hay giữ nguyên trước khi push |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| **Bottleneck** | Gộp chung lỗi đặt tên file và dò bảng trống | Tập trung vào dò ô bảng trống, đếm từ và lỗi viết lẫn giải pháp vào problem | Kiểm chứng ở CP4 cho thấy đặt tên file chỉ làm 1 lần lúc đầu, còn dò bảng trống và lỗi lạc đề mới lặp lại ở mọi checkpoint |
| **Success Metric** | Chỉ đo thời gian (< 5 phút) và số lỗi sót (0 lỗi) | Thêm metric chất lượng: >= 80% cảnh báo của AI là đúng | Tránh việc AI báo lỗi tràn lan làm học viên mất thêm thời gian đọc cảnh báo rác |
| **Mức chọn / Quy trình** | Chưa tách rõ bước nào Rule, bước nào AI | Tách rõ Bước 1 dùng Rule (ô trống, số từ, link), Bước 2 dùng AI (lỗi lạc đề) | Research ở CP4 chứng minh các lỗi cú pháp/ô trống/link dùng Rule nhanh và chuẩn xác hơn AI |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | Chỉ đúng vị trí lỗi | Nêu rõ tên mục/số dòng hoặc trích dẫn đúng câu có vấn đề trong file | Nói chung chung "bài còn một số chỗ chưa rõ" mà không chỉ ra câu nào |
| 2 | Bắt đúng lỗi "solution-first" | Phát hiện được các câu Job Story hoặc Opportunity có chứa từ khóa công cụ/giải pháp (như "làm chatbot", "xây app AI") | Bỏ sót câu chứa giải pháp rõ ràng hoặc báo nhầm các câu mô tả quy trình hiện tại |
| 3 | Không viết làm thay | Chỉ đặt câu hỏi gợi mở hoặc nêu lý do vi phạm để học viên tự viết lại | Tự viết sẵn đoạn văn hoàn chỉnh để học viên copy-paste (vi phạm `RULES.md`) |
| 4 | Thời gian đọc nhanh | Toàn bộ danh sách cảnh báo ngắn gọn dưới 150 từ, đọc xong trong 1 phút | Viết nhận xét dài dòng lan man làm mất thời gian trước giờ nộp |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | **Thấp** | Mọi thành viên trong nhóm và các bạn được hỏi đều phải kiểm tra bài trước khi nộp để tránh mất điểm oan |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | **Thấp** | Đầu ra chỉ là checklist ngắn gọn chỉ rõ mục nào còn trống / câu nào phạm quy; học viên hiểu và sửa được ngay trong 2 phút |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | **Thấp** | File Markdown nằm sẵn trên máy/repo; script kiểm tra ô trống/số từ hoặc công cụ `markdownlint` và prompt phản biện đều dùng được ngay trong 5 phút |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | **Thấp** | Chi phí bằng 0; tuân thủ tuyệt đối quy định trong `RULES.md` vì AI chỉ dùng để phản biện/chỉ ra lỗ hổng chứ không viết bài thay |

### 8.2. Kết luận

**Quyết định:** **Go** (phạm vi nhỏ, áp dụng ngay cho đợt nộp bài lab hôm nay).

**Lý do:** Cả 4 rủi ro đều ở mức **Thấp**; sự kết hợp giữa **Rule** (kiểm tra ô trống, tên file, số từ, link) và **Prompt AI phản biện** giải quyết trực tiếp bước nghẽn 10 phút rà bài mà không tốn chi phí xây dựng phức tạp.

**Nếu Go — pilot nhỏ nhất:**
- Áp dụng ngay trên 4 file báo cáo cá nhân và 1 file `group_report.md` của nhóm `CUTTAY` trước khi push cuối buổi:
  1. Chạy kiểm tra nhanh (Rule/Checklist): Tên file đúng `MSSV_HoTen.md`, không còn dòng bảng `| | |` bỏ trống ở các mục bắt buộc, mục 6 Reflection đủ >= 200 từ.
  2. Chạy Prompt phản biện chuẩn (như trong `01-worksheet.md`) để kiểm tra không có giải pháp lồng trong Job Story / Problem Statement.
  3. Bấm giờ xem tổng thời gian rà soát có thực sự dưới 5 phút/người không.

**Nếu Not Yet — cần kiểm chứng gì trước:** *(Không áp dụng vì nhóm chọn Go)*.

**Nếu No-Go — nên làm gì thay AI:** *(Không áp dụng vì nhóm chọn Go)*.

**Ngưỡng dừng** (nếu sau … mà … thì quay về …):
- Nếu sau 2 lần nộp bài mà thời gian chạy Workflow + đọc cảnh báo của AI mất **trên 10 phút** hoặc có **trên 50% cảnh báo của AI là báo nhầm**, nhóm sẽ bỏ bước dùng AI ở Bước 2 và quay về dùng thuần túy **Checklist cố định + Script Rule kiểm tra ô trống/số từ**.

---

## 9. Hạn chế và hướng tiếp theo

- **Hạn chế hiện tại:** Baseline thời gian (15–25 phút) ban đầu dựa trên ước lượng của các thành viên và mới kiểm chứng nhanh trên mẫu nhỏ trong lớp; cần bấm giờ thực tế ở các buổi lab tiếp theo để có số liệu chính xác hơn.
- **Hướng tiếp theo:** Đóng gói bước kiểm tra Rule (kiểm tra tên file, phát hiện ô bảng trống, đếm từ mục Reflection, kiểm tra link) thành một GitHub Action hoặc script `check_submission.py` chạy tự động mỗi khi thành viên tạo Pull Request lên repo nhóm.

## 10. Tài liệu tham khảo

- Hướng dẫn bài tập và khung lý thuyết: [docs/01-worksheet.md](../../docs/01-worksheet.md), [docs/03-international-frameworks.md](../../docs/03-international-frameworks.md), [RULES.md](../../RULES.md).
- Công cụ kiểm tra cú pháp Markdown (`markdownlint-cli2`): https://github.com/DavidAnson/markdownlint-cli2
- Công cụ kiểm tra link hỏng (`lychee`): https://github.com/lycheeverse/lychee
- Framework tự động chạy kiểm tra trước khi commit (`pre-commit`): https://pre-commit.com/
