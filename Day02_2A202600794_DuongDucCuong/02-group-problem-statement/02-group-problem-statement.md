# 02 — Group Problem Statement

## Group convergence

Nhóm 5 người share các problem cá nhân. Tổng cộng nhóm có khoảng 12 candidate problems, sau đó gom lại thành các cluster để chọn problem cuối.

| Cluster | Candidate examples | Pattern chung |
|---|---|---|
| Ăn uống hằng ngày | Nghĩ hôm nay ăn gì, theo dõi chi tiêu ăn uống, quên đồ ăn trong tủ lạnh | Sinh viên muốn ăn uống tiện hơn, ít lãng phí hơn, giữ ngân sách tốt hơn |
| Chuẩn bị trước khi ra khỏi nhà | Quên mang thẻ xe/sạc/tai nghe, chọn quần áo buổi sáng, nhắc uống nước/ngủ đúng giờ | Cần checklist hoặc reminder đơn giản |
| Việc nhóm và kế hoạch cá nhân | Phân chia việc dọn phòng, ưu tiên deadline cá nhân, lên kế hoạch đi chơi nhóm | Cần sắp xếp ưu tiên hoặc thống nhất giữa nhiều người |
| Quản lý đồ cá nhân/dữ liệu | Mua đồ online quên so sánh giá, tìm lại ảnh/tài liệu cá nhân | Cần tìm, so sánh, phân loại nhưng có rủi ro dữ liệu |

## Shortlist và score

| Candidate | Actor rõ | Workflow rõ | Pain có evidence | Impact đo được | Làm trong lab | So sánh R/W/A được | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| Nghĩ hôm nay ăn gì và mua đồ ăn thiếu/thừa | 5 | 5 | 4 | 5 | 5 | 5 | 5 | 34 |
| Theo dõi chi tiêu ăn uống bằng trí nhớ | 5 | 4 | 4 | 5 | 4 | 4 | 5 | 31 |
| Quên đồ ăn trong tủ lạnh đến khi hỏng | 5 | 4 | 3 | 4 | 5 | 4 | 5 | 30 |

Nhóm chọn: **Nghĩ hôm nay ăn gì và mua đồ ăn thiếu/thừa**.

Vì sao chọn:

- Actor rất rõ: sinh viên ở trọ tự lo bữa ăn.
- Workflow lặp lại nhiều lần/tuần và dễ vẽ before/after.
- Bottleneck cụ thể nằm ở bước nghĩ món và lập danh sách mua.
- Có thể đo bằng thời gian, số lần mua thiếu/thừa và mức độ vượt ngân sách.
- Đủ đơn giản để làm pilot nhỏ trong lab.
- Có thể so sánh rõ No AI / Rule / Workflow / Agent.

Vì sao không chọn các bài khác:

- Theo dõi chi tiêu ăn uống: impact tài chính rõ nhưng có thể chỉ cần app ghi chi tiêu hoặc Google Sheets, AI chưa chắc là phần quan trọng nhất.
- Quên đồ ăn trong tủ lạnh: đáng giải quyết nhưng phụ thuộc việc người dùng có chịu nhập/chụp đồ ăn sau mỗi lần mua không.

## Quick validation

Nhóm kiểm chứng nhanh bằng quan sát cá nhân và hỏi miệng một vài bạn sinh viên ở trọ. Các số liệu dưới đây là ước lượng ban đầu, cần đo lại nếu làm pilot thật.

| Nguồn | Số người / mẫu | Tín hiệu xác nhận | Tín hiệu phản bác | Nhóm sửa problem thế nào |
|---|---:|---|---|---|
| Quick interview | 3 bạn sinh viên | 2/3 bạn nói thường mất thời gian nghĩ ăn gì, nhất là buổi tối | 1 bạn thường ăn ngoài nên ít tự nấu | Thu hẹp actor: sinh viên ở trọ có tự nấu hoặc mua đồ về ăn |
| Micro poll trong nhóm/lớp | 5-10 bạn dự kiến hỏi thêm | Nhiều bạn muốn có danh sách mua đồ đơn giản trước khi đi siêu thị | Một số bạn không muốn nhập quá nhiều thông tin | Giới hạn input còn 4 mục: đồ đang có, ngân sách, thời gian nấu, món không ăn |
| Quan sát cá nhân | 1 tuần sinh hoạt | Hay mua đồ theo cảm tính, có lúc thừa rau/trứng hoặc thiếu gia vị | Chưa đo chính xác tiền lãng phí | Dùng pilot 1 tuần để đo thật |

Insight sau validation:

```text
Pain thật không chỉ là "không biết ăn gì". Pain nằm ở việc phải nối nhiều yếu tố nhỏ: còn nguyên liệu gì, có bao nhiêu tiền, có bao nhiêu thời gian, món nào dễ nấu và có bị ngán không. Nếu solution bắt người dùng nhập quá nhiều thì họ sẽ bỏ, nên workflow phải thật nhẹ.
```

## Research giải pháp

Nhóm tìm các hướng đã có sẵn, không giả định phải tự build một agent lớn từ đầu.

| Nguồn / tool / case | Link | Họ giải quyết phần nào? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| Meal planner / thực đơn cố định | Có thể làm bằng Google Sheets | Lập thực đơn tuần và danh sách mua đồ | Đơn giản, dễ làm, ít rủi ro | Dễ chán, không linh hoạt theo đồ đang có | Dùng làm baseline non-AI |
| Google Keep / Apple Notes / Notion checklist | App ghi chú có sẵn | Ghi danh sách mua đồ | Rất nhanh, dễ dùng | Không tự gợi ý món, không biết ngân sách | Checklist giải quyết một phần, nhưng chưa giải quyết phần nghĩ món |
| Cookpad / YouTube / blog nấu ăn | Các nguồn công thức nấu ăn | Tìm công thức món ăn | Nhiều lựa chọn, dễ xem hướng dẫn | Tìm lâu, không cá nhân hóa theo đồ đang có | AI nên gợi ý ít món phù hợp thay vì đưa quá nhiều lựa chọn |
| ChatGPT / Gemini / Claude | Công cụ AI hội thoại | Gợi ý món từ nguyên liệu và ngân sách | Linh hoạt, hiểu input tự nhiên | Có thể gợi ý món không hợp khẩu vị hoặc nguyên liệu khó mua | Cần human review và fallback bằng món quen |

Research takeaway:

```text
Không nên build Agent tự lập kế hoạch ăn uống và tự mua đồ. Hướng hợp lý hơn là Workflow nhẹ: người dùng nhập vài thông tin chính, AI gợi ý 3 món và danh sách mua, người dùng sửa lại rồi mới đi mua.
```

## Workflow before/after

Nội dung workflow nhóm dùng trong bài:

```text
CURRENT STATE — 5 bước, khoảng 55 phút/lần

[1 Nghĩ hôm nay ăn gì: 15']
→ [2 Kiểm tra đồ đang có: 5']
→ [3 Tự đoán cần mua gì: 15']  <-- bottleneck
→ [4 Đi mua đồ: 15']
→ [5 Nấu/ăn hoặc đổi món nếu thiếu đồ: 5']

Rủi ro:
Mua thiếu nguyên liệu, mua thừa đồ tươi, vượt ngân sách hoặc đặt đồ ăn ngoài vì quá mệt để nghĩ.

FUTURE STATE — 6 bước, khoảng 30 phút/lần

[1 Nhập đồ đang có + ngân sách + thời gian nấu + món không ăn: 3']
→ [2 AI gợi ý 3 món phù hợp: 1']       -- Workflow step
→ [3 AI tạo danh sách mua tối giản: 1'] -- Workflow step
→ [4 Sinh viên chọn/sửa danh sách: 5']  -- Human boundary
→ [5 Đi mua đồ theo checklist: 15']
→ [6 Nấu/ăn: 5']

Fallback:
AI gợi ý không hợp → dùng danh sách 5-7 món quen và checklist mua đồ cố định.

Bottleneck mới:
Sinh viên review và sửa danh sách. Đây là bottleneck chấp nhận được vì đó là điểm kiểm soát khẩu vị, ngân sách và thực tế đồ đang có.
```

Before/after impact:

| Metric | Trước | Sau kỳ vọng | Ghi chú |
|---|---:|---:|---|
| Tổng thời gian trước khi có bữa ăn | Khoảng 55 phút | Khoảng 30 phút | Giảm chủ yếu ở bước nghĩ món và lập danh sách |
| Thời gian nghĩ món + lập danh sách | 30-40 phút | Dưới 10 phút | Target chính |
| Số lần mua thiếu/thừa | 2-3 lần/tuần | 0-1 lần/tuần | Cần đo trong pilot |
| Số bước thủ công | 5/5 | 4/6 | Người dùng vẫn chọn, sửa, mua, nấu |
| Risk mới | Mua theo cảm tính | AI gợi ý món không hợp | Cần fallback món quen |

## Problem Statement v0

| Field | Nội dung |
|---|---|
| **Actor** | Sinh viên ở trọ, tự lo bữa ăn hằng ngày hoặc vài lần mỗi tuần. |
| **Workflow** | Sinh viên nghĩ món, kiểm tra đồ đang có, đoán cần mua gì, đi mua đồ, rồi nấu/ăn. |
| **Bottleneck** | Bước nghĩ món và lập danh sách mua mất 25-40 phút vì phải cân bằng khẩu vị, ngân sách, thời gian nấu và nguyên liệu đang có. |
| **Impact** | Mất thời gian, dễ mua thiếu/thừa, dễ đặt đồ ăn ngoài, chi tiêu ăn uống khó kiểm soát. |
| **Success Metric** | Giảm thời gian nghĩ món + lập danh sách từ khoảng 35 phút xuống dưới 10 phút/lần; giảm số lần mua thiếu/thừa xuống 0-1 lần/tuần. |
| **Boundary** | AI không tự quyết định người dùng phải ăn gì, không tự mua đồ, không tự giả định dị ứng/khẩu vị nếu chưa có input; người dùng phải review danh sách trước khi mua. |

## Rule / Workflow / Agent

| Mức | Phương án | Khi nào đủ | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI / Process fix** | Tự lập 5-7 món quen và checklist mua đồ cố định | Đủ nếu người dùng không cần đổi món nhiều | Dễ chán, không linh hoạt theo đồ đang có | Dùng làm fallback |
| **Rule** | Lọc món theo rule: dưới 30 phút, dưới 50.000đ, ít nguyên liệu | Đủ để lọc món quen | Không gợi ý tốt khi đồ đang có thay đổi | Dùng một phần |
| **Workflow** | Nhập đồ đang có + ngân sách + thời gian → AI gợi ý món → AI tạo danh sách mua → người dùng sửa | Phù hợp vì AI hỗ trợ đúng bước mơ hồ nhất | Gợi ý món không hợp, danh sách thiếu nguyên liệu | Chọn |
| **Agent** | Agent tự lập kế hoạch ăn cả tuần, tự đặt hàng/mua đồ | Chỉ cần nếu có nhiều app tích hợp và người dùng muốn tự động hóa mạnh | Quá rủi ro, dễ mua sai, không phù hợp pilot nhỏ | Không chọn |

Mức chọn:

```text
Workflow.
```

Vì sao:

- Workflow hiện tại có các bước rõ và lặp lại.
- AI chỉ hỗ trợ phần mơ hồ nhất: gợi ý món và danh sách mua.
- Người dùng vẫn quyết định món cuối cùng, sửa danh sách và tự mua đồ.
- Chưa cần Agent vì không cần AI tự lập kế hoạch dài hạn hoặc tự hành động.

## Problem Statement v1

| Field | Nội dung |
|---|---|
| **Actor** | Sinh viên ở trọ tự lo bữa ăn 3-5 lần mỗi tuần. |
| **Workflow** | Nghĩ món → kiểm tra đồ đang có → lập danh sách mua → đi mua → nấu/ăn → xử lý đồ thừa. |
| **Bottleneck** | Nghĩ món và lập danh sách mua mất 25-40 phút/lần vì phải cân bằng khẩu vị, ngân sách, thời gian nấu và nguyên liệu đang có. |
| **Impact** | Mất thời gian, mua thiếu/thừa đồ ăn, có thể vượt ngân sách hoặc đặt đồ ăn ngoài vì không nghĩ ra món. |
| **Success Metric** | Giảm thời gian nghĩ món + lập danh sách xuống dưới 10 phút/lần; giảm mua thiếu/thừa xuống 0-1 lần/tuần; người dùng thấy danh sách mua đủ dùng trong pilot 1 tuần. |
| **Boundary** | AI không tự mua đồ, không ép người dùng ăn món cụ thể, không giả định dị ứng/kiêng ăn, không thay quyết định cuối của người dùng. |
| **AI intervention point** | Sau khi người dùng nhập đồ đang có, ngân sách, thời gian nấu và món không ăn; trước khi đi mua đồ. |
| **Mức chọn** | Workflow: input ngắn → AI gợi ý 3 món → AI tạo danh sách mua → người dùng review. |
| **Rủi ro & người thật kiểm tra** | Risk: món không hợp khẩu vị, thiếu nguyên liệu, giá thực tế khác dự đoán. Người thật review: sinh viên phải sửa danh sách trước khi mua. |

## Final decision

Decision:

```text
Go với scope nhỏ.
```

Pilot nhỏ nhất:

- Trong 1 tuần, mỗi lần chuẩn bị bữa ăn, sinh viên nhập 4 thông tin: đồ đang có, ngân sách, thời gian nấu, món không ăn.
- AI gợi ý 3 món và danh sách mua.
- Sinh viên đo thời gian nghĩ món, số lần phải mua bổ sung và số lần còn thừa đồ.
- Sau 1 tuần, so sánh với baseline hiện tại.

Exit / rollback:

- Nếu sinh viên vẫn phải sửa lại hơn 70% danh sách trong nhiều lần liên tiếp, hạ xuống thực đơn cố định + checklist.
- Nếu AI liên tục gợi ý món không hợp khẩu vị hoặc nguyên liệu khó mua, chỉ dùng AI như nguồn ý tưởng, không dùng làm danh sách mua trực tiếp.
- Nếu người dùng thấy việc nhập 4 thông tin quá phiền, giảm về Rule/checklist đơn giản.

Decision rationale:

- Problem rõ, workflow rõ, metric rõ.
- Có non-AI alternative làm fallback.
- AI nằm ở một bước cụ thể, không ôm toàn bộ việc ăn uống.
- Human review rõ trước khi mua đồ.
