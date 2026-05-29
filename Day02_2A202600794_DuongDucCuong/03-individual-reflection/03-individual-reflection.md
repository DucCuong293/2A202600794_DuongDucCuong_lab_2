# 03 — Individual Reflection

## Đóng góp của tôi trong nhóm

| Hoạt động | Tôi đã làm gì? | Kết quả |
|---|---|---|
| Scan cá nhân | Scan 10 problems đời thường quanh ăn uống, chi tiêu, đồ dùng cá nhân và việc học | Có nhiều candidate gần gũi để nhóm thảo luận |
| Pitch | Pitch problem "nghĩ hôm nay ăn gì và mua đồ ăn thiếu/thừa" | Problem được đưa vào shortlist vì actor rõ, workflow rõ và xảy ra thường xuyên |
| Challenge | Hỏi liệu bài theo dõi chi tiêu có cần AI không hay chỉ cần app ghi chi tiêu | Nhóm phân biệt rõ hơn giữa Rule, Workflow và Agent |
| Group convergence | Góp phần gom các candidate thành cluster: ăn uống, chuẩn bị trước khi ra khỏi nhà, việc nhóm/kế hoạch cá nhân, quản lý đồ cá nhân | Nhóm nhìn ra pattern chung thay vì vote theo cảm tính |
| Agent thành viên thứ 6 | Dùng Agent để tổng hợp 9-12 candidate problems, chấm điểm và đề xuất problem cuối | Nhóm có thêm góc nhìn khách quan nhưng vẫn tự kiểm tra lại kết luận |
| Workflow | Đóng góp current/future workflow cho bài toán ăn uống | Bottleneck chính được làm rõ: nghĩ món + lập danh sách mua |
| Research | Tìm và so sánh các hướng hiện có như thực đơn cố định, checklist, app ghi chú, app công thức, AI chat | Nhóm thấy không cần build agent từ đầu |
| Problem Statement | Góp ý để metric và boundary cụ thể hơn | Problem Statement v1 rõ hơn v0 |
| Rule / Workflow / Agent | Lập luận chọn Workflow, dùng Rule làm fallback và không chọn Agent | Nhóm thống nhất AI chỉ hỗ trợ gợi ý món + danh sách mua |
| Decision | Ủng hộ Go với scope nhỏ trong 1 tuần | Quyết định có pilot, cách đo và rollback rõ |

## Bảng dùng AI trong reflection

| Phase | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai/hời hợt ở đâu? | Tôi sửa gì |
|---|---|---|---|---|
| Scan | Gợi ý thêm problem đời thường sau khi tôi tự nghĩ trước | Giúp mở rộng từ ăn uống sang chi tiêu, quên đồ, việc phòng trọ | Một số ý quá chung như "quản lý cuộc sống cá nhân" | Chỉ giữ ý có actor và workflow rõ |
| Problem Card | Nhờ AI phản biện actor, bottleneck và metric | Giúp thấy cần đo thời gian nghĩ món và số lần mua thiếu/thừa | AI ban đầu kéo bài thành "trợ lý ăn uống toàn diện" | Thu hẹp scope về một lần chuẩn bị bữa hoặc pilot 1 tuần |
| Workflow | Nhờ AI sắp xếp workflow trước/sau thành các bước | Giúp nhìn rõ AI nên nằm trước bước đi mua đồ | AI có lúc bỏ qua bước người dùng review | Thêm bước sinh viên chọn/sửa danh sách trước khi mua |
| Research | Dùng AI để nghĩ các giải pháp/pattern hiện có | Nhắc đến thực đơn cố định, checklist, app công thức và AI chat | Một số gợi ý quá phức tạp như tích hợp đặt hàng | Chỉ giữ giải pháp phù hợp với lab nhỏ |
| Problem Statement | Nhờ AI chỉ ra field còn mơ hồ | Giúp sửa metric từ "ăn uống tiện hơn" thành "35 phút xuống dưới 10 phút" | AI viết lại hơi chung chung | Nhóm tự viết lại bằng ngôn ngữ của mình |
| Rule / Workflow / Agent | Nhờ AI hỏi ngược có thật sự cần Agent không | Giúp thấy Workflow đã đủ cho scope hiện tại | AI đề xuất tự động lập kế hoạch cả tuần hơi quá rộng | Hạ scope về gợi ý 3 món cho từng lần chuẩn bị bữa |
| Agent thành viên thứ 6 | Dùng Agent để tổng hợp candidates, gom cluster, chấm điểm | Giúp nhóm tránh chọn theo cảm tính, có bảng điểm và lý do rõ hơn | Agent vẫn có thể thiên về problem dễ đo | Nhóm đọc lại, phản biện và tự xác nhận problem cuối |
| Decision | Dùng AI kiểm tra logic Go / Not Yet / No-Go | Giúp thêm pilot 1 tuần và fallback | Nếu nghe AI quá nhiều dễ để AI quyết định thay nhóm | Nhóm tự chốt Go với scope nhỏ |

## Bài học của tôi

- Problem tốt không phải problem nghe "AI" nhất, mà là problem có actor, workflow, bottleneck và metric rõ.
- Một vấn đề đời thường như "không biết ăn gì" vẫn có thể phân tích như bài toán sản phẩm nếu tách thành các bước cụ thể.
- Vẽ workflow giúp nhóm thấy phần nào chỉ cần Rule/checklist, phần nào AI mới có ích.
- Agent không phải lựa chọn mặc định. Trong case này, Agent phù hợp để hỗ trợ nhóm hội tụ ý tưởng, nhưng solution cuối cho người dùng nên là Workflow.
- Human review rất quan trọng. AI có thể gợi ý món và danh sách mua, nhưng sinh viên vẫn phải kiểm tra khẩu vị, ngân sách, dị ứng, giá thực tế và đồ đang có.
- Research không phải để copy một tool có sẵn, mà để thấy pattern: nhiều giải pháp tốt bắt đầu từ workflow nhỏ, có fallback đơn giản và không tự động hóa quá sớm.

## Điều tôi học được khi nghe top 3 problems của các bạn khác

```text
Tôi nhận ra các problem nhỏ trong đời sống sinh viên đều có thể phân tích được nếu nhìn bằng actor, workflow, bottleneck và metric. Ví dụ "không biết ăn gì" nghe rất nhỏ, nhưng khi tách ra thì có nhiều bước: kiểm tra đồ đang có, cân nhắc tiền, chọn món, mua đồ và xử lý đồ thừa.

Tôi cũng thấy Agent thành viên thứ 6 có thể giúp nhóm tổng hợp và phản biện tốt hơn, nhưng nhóm vẫn phải tự kiểm tra xem kết luận của Agent có đúng với trải nghiệm thật không.
```

## Nhóm có lúc nào bị solution-first không?

```text
Có. Lúc đầu nhóm dễ nghĩ ngay đến một app AI gợi ý mọi thứ về ăn uống. Sau khi vẽ workflow, nhóm thấy không cần app lớn hay Agent tự hành động. Vấn đề chính chỉ là giảm thời gian nghĩ món và lập danh sách mua đồ, nên Workflow nhẹ là đủ.
```

## Tôi có thay đổi ý kiến sau khi bị challenge không?

```text
Có. Ban đầu tôi nghĩ AI nên tự lập thực đơn cả tuần. Sau khi bị challenge rằng người dùng có thể đổi khẩu vị mỗi ngày và không muốn nhập quá nhiều, tôi đồng ý giảm scope: chỉ gợi ý 3 món cho từng lần chuẩn bị bữa.
```

## Điều khó nhất khi viết Problem Statement

```text
Khó nhất là biến một vấn đề rất đời thường thành metric đo được. Nếu chỉ viết "giúp ăn uống dễ hơn" thì quá mơ hồ. Nhóm phải đổi thành: giảm thời gian nghĩ món + lập danh sách từ khoảng 35 phút xuống dưới 10 phút, và giảm số lần mua thiếu/thừa xuống 0-1 lần/tuần.
```

## Nếu làm lại

```text
Tôi sẽ hỏi nhanh nhiều bạn ở trọ hơn để biết họ thật sự đau ở bước nào: nghĩ món, đi mua đồ, nấu ăn hay quản lý đồ thừa. Tôi cũng sẽ thử pilot trong 1 tuần để có số liệu thật thay vì chỉ ước lượng.
```

## Tự kiểm cuối bài

- [x] Cá nhân có 5+ problems và top 3 Problem Cards.
- [x] Tôi đã pitch rõ và challenge nhóm đúng trọng tâm.
- [x] Nhóm có nhật ký hội tụ từ candidates về 1 bài.
- [x] Nhóm có workflow trước/sau.
- [x] Nhóm có Problem Statement v0/v1 với metric và boundary rõ.
- [x] Nhóm có so sánh No AI / Rule / Workflow / Agent.
- [x] Nhóm có Go / Not Yet / No-Go và lý do rõ.
- [x] Reflection cá nhân nói đúng với vai trò và đóng góp của tôi.
- [x] Tôi tự giải thích được mạch problem → workflow → metric → boundary → AI fit.
