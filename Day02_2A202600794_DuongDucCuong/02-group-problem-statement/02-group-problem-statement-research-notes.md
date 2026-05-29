# 02 — Group Problem Statement Research Notes

## Research goal

Nhóm research để trả lời 3 câu hỏi:

1. Với problem "sinh viên ở trọ mất thời gian nghĩ hôm nay ăn gì và mua đồ ăn thiếu/thừa", hiện đã có những cách giải nào?
2. Cách nào chỉ cần Rule/checklist, cách nào cần Workflow có AI hỗ trợ?
3. Có nên làm Agent tự lập kế hoạch hoặc tự mua đồ không?

## Problem scope sau khi thu hẹp

```text
Không làm "trợ lý ăn uống toàn diện".
Chỉ tập trung vào một workflow nhỏ:
Sinh viên nhập đồ đang có + ngân sách + thời gian nấu + món không ăn
→ AI gợi ý 3 món
→ AI tạo danh sách mua đồ
→ sinh viên review trước khi đi mua.
```

## Research questions

| Câu hỏi | Vì sao cần hỏi? |
|---|---|
| Người dùng có thật sự cần AI để nghĩ món không? | Nếu thực đơn cố định đã đủ thì không nên dùng AI quá sớm. |
| Người dùng có chịu nhập đồ đang có không? | Nếu input quá phiền, workflow sẽ bị bỏ. |
| Danh sách mua đồ nên tự động đến mức nào? | Nếu tự mua hoặc tự đặt hàng thì rủi ro cao. |
| Có thể đo thành công bằng gì? | Cần metric rõ: thời gian, số lần mua thiếu/thừa, mức độ vượt ngân sách. |

## Sources scanned

| Nguồn / tool / pattern | Link | Họ giải quyết phần nào? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| Google Keep | https://support.google.com/keep/answer/2888240 | Ghi note, tạo list, reminder | Nhanh, dễ dùng, phù hợp checklist mua đồ | Không tự gợi ý món theo đồ đang có/ngân sách | Checklist là baseline tốt cho non-AI / Rule |
| Apple Notes | https://support.apple.com/en-ie/118442 | Ghi note, checklist, bảng, lưu thông tin cá nhân | Có sẵn trên iPhone, ít friction | Không cá nhân hóa món ăn, không tự tạo danh sách mua thông minh | Dùng được cho danh sách mua thủ công |
| Notion | https://www.notion.com/notes | Note, task, template, tổ chức thông tin | Có thể làm meal plan/table theo tuần | Setup hơi nặng với sinh viên chỉ cần chuẩn bị một bữa | Hợp cho người thích quản lý có cấu trúc, chưa chắc hợp pilot nhẹ |
| Cookpad | https://cookpad.com/eng | Tìm và chia sẻ công thức nấu ăn | Nhiều công thức, cộng đồng người nấu thật | Người dùng vẫn phải tự search, tự lọc theo nguyên liệu và ngân sách | AI nên giảm số lựa chọn xuống còn vài món phù hợp |
| YouTube search/filter | https://support.google.com/youtube/answer/111997 | Tìm video hướng dẫn nấu ăn | Dễ xem cách làm trực quan | Có quá nhiều kết quả, mất thời gian chọn | Video/công thức là input tham khảo, không phải workflow chính |
| ChatGPT | https://help.openai.com/en/articles/9125172 | AI hội thoại có thể gợi ý món từ input tự nhiên | Linh hoạt, dễ thử nhanh bằng prompt | Có thể gợi ý món không hợp khẩu vị, nguyên liệu khó mua hoặc giá không đúng thực tế | Chỉ nên dùng để draft/gợi ý, cần người dùng review |

## Pattern rút ra

### 1. Checklist giải quyết được một phần

Google Keep, Apple Notes hoặc Notion có thể giúp người dùng ghi danh sách mua đồ. Đây là giải pháp đơn giản, không cần AI.

Điểm thiếu:

- Không giúp người dùng nghĩ món mới.
- Không tự nối các yếu tố: đồ đang có, ngân sách, thời gian nấu, món không ăn.
- Nếu danh sách ban đầu sai thì checklist chỉ giúp mua sai một cách có tổ chức hơn.

### 2. Recipe apps giải quyết phần công thức, không giải quyết phần quyết định

Cookpad, YouTube hoặc blog nấu ăn có nhiều công thức. Nhưng người dùng vẫn phải tự tìm, tự lọc và tự quyết định món nào hợp với tình huống hiện tại.

Điểm thiếu:

- Quá nhiều lựa chọn.
- Không tối ưu cho sinh viên có ngân sách thấp và thời gian ít.
- Không tự tạo danh sách mua đồ ngắn gọn từ nguyên liệu đang có.

### 3. AI chat phù hợp với bước mơ hồ nhất

AI có ích nhất ở bước:

```text
Đồ đang có + ngân sách + thời gian nấu + món không ăn
→ gợi ý vài món phù hợp
→ tạo danh sách mua tối giản.
```

Nhưng AI không nên tự quyết định toàn bộ, vì:

- Khẩu vị thay đổi theo ngày.
- Giá thực tế ở cửa hàng có thể khác.
- AI không biết chính xác tủ lạnh/phòng đang có gì nếu người dùng không nhập.
- Dị ứng, kiêng ăn, món ghét phải do người dùng kiểm tra.

## Rule / Workflow / Agent implication

| Mức | Kết luận từ research |
|---|---|
| No AI / Process fix | Dùng thực đơn cố định 5-7 món và checklist mua đồ. Hợp làm fallback. |
| Rule | Lọc món theo rule như dưới 30 phút, dưới 50.000đ, ít nguyên liệu. Hợp để giới hạn lựa chọn. |
| Workflow | Phù hợp nhất cho pilot: người dùng nhập input ngắn, AI gợi ý món và danh sách mua, người dùng review. |
| Agent | Chưa nên chọn. Tự lập kế hoạch cả tuần hoặc tự đặt hàng/mua đồ quá rủi ro và vượt scope lab. |

## Proposed pilot based on research

```text
Thời gian: 1 tuần
Người thử: 1-3 sinh viên ở trọ
Tần suất: mỗi lần chuẩn bị bữa ăn

Input:
- Đồ đang có
- Ngân sách dự kiến
- Thời gian nấu
- Món không ăn / dị ứng nếu có

Output AI:
- 3 món gợi ý
- Lý do chọn từng món
- Danh sách mua đồ tối giản

Người dùng:
- Chọn 1 món
- Sửa danh sách mua
- Ghi lại thời gian và lỗi nếu có
```

## Metrics to track

| Metric | Baseline | Target |
|---|---:|---:|
| Thời gian nghĩ món + lập danh sách | Khoảng 35 phút/lần | Dưới 10 phút/lần |
| Số lần mua thiếu/thừa nguyên liệu | 2-3 lần/tuần | 0-1 lần/tuần |
| Số lần phải đổi món vì thiếu đồ | Chưa đo | Giảm sau pilot |
| Tỷ lệ danh sách AI cần sửa nhiều | Chưa đo | Dưới 30% nội dung phải sửa |
| Mức độ phiền khi nhập input | Chưa đo | Người dùng thấy chấp nhận được |

## Risks and mitigations

| Risk | Vì sao xảy ra | Mitigation |
|---|---|---|
| AI gợi ý món không hợp khẩu vị | Input chưa đủ hoặc khẩu vị thay đổi | Luôn hỏi món không ăn và để người dùng chọn/sửa |
| Danh sách mua thiếu nguyên liệu | AI không biết đồ thật đang có | Người dùng review danh sách trước khi mua |
| Giá thực tế vượt ngân sách | Giá cửa hàng thay đổi | Dùng ngân sách như constraint mềm, người dùng kiểm lại giá |
| Người dùng lười nhập input | Workflow quá nặng | Chỉ yêu cầu 4 input ngắn, cho phép bỏ qua mục không biết |
| Solution quá rộng | Dễ biến thành app ăn uống toàn diện | Giữ scope một lần chuẩn bị bữa, không lập kế hoạch cả tuần trong pilot |

## Research takeaway

```text
Hướng tốt nhất không phải Agent, mà là Workflow nhẹ.
Rule/checklist đủ làm fallback, recipe apps đủ làm nguồn tham khảo,
còn AI hữu ích nhất ở bước gợi ý món + tạo danh sách mua từ input ngắn.
Người dùng vẫn là người kiểm tra và quyết định cuối.
```
