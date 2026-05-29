# Day 02 Lab — Tìm Đúng Bài Toán Cho AI

## Chủ đề bài làm

Problem đời thường được chọn:

```text
Sinh viên ở trọ mất thời gian nghĩ hôm nay ăn gì, mua đồ ăn thiếu/thừa và khó giữ chi tiêu ăn uống ổn định.
```

Đây là một problem gần với đời sống hằng ngày, dễ quan sát và có workflow rõ: nghĩ món → kiểm tra đồ đang có → lập danh sách mua → đi mua → nấu/ăn → xử lý đồ thừa.

## Hướng tiếp cận

```text
Problem thật → workflow hiện tại → bottleneck → metric → boundary → chọn Rule / Workflow / Agent → quyết định Go / Not Yet / No-Go.
```

Quyết định cuối:

```text
Go với scope nhỏ: chọn Workflow có AI hỗ trợ gợi ý món và danh sách mua đồ, nhưng sinh viên vẫn tự kiểm tra ngân sách, khẩu vị, nguyên liệu và quyết định cuối.
```

Trong quá trình hội tụ nhóm, nhóm cũng dùng một **Agent thành viên thứ 6** để tổng hợp candidates, gom cluster, chấm điểm và đề xuất problem cuối cho buổi thuyết trình. Agent này hỗ trợ nhóm chọn bài, còn solution cuối cho problem ăn uống vẫn là Workflow chứ không phải Agent.

## Vì sao không chọn Agent làm solution cuối?

- Bài toán không cần AI tự chạy nhiều công cụ hoặc tự quyết định thay người dùng.
- Workflow khá rõ và lặp lại: kiểm tra đồ có sẵn, chọn món, lập danh sách mua, nấu/ăn.
- Nếu AI gợi ý món không hợp khẩu vị, sai ngân sách hoặc không biết đồ thật đang có, người dùng vẫn phải kiểm lại.
- Rule và Workflow đã đủ cho pilot nhỏ, ít rủi ro hơn Agent.

## Cấu trúc bài nộp

```text
Day02_2A202600794_DuongDucCuong/
├── README.md
├── 01-individual-problem-scan/
│   └── README.md
├── 02-group-problem-statement/
│   └── README.md
└── 03-individual-reflection/
    └── README.md
```

## Tóm tắt 3 phần

| Phần | Nội dung chính |
|---|---|
| 01 — Individual Problem Scan | Scan 10 problems, chọn top 3, viết Problem Card cho bài muốn pitch nhất. |
| 02 — Group Problem Statement | Hội tụ nhóm, shortlist/score, validation, research, workflow before/after, Problem Statement v0/v1, so sánh Rule / Workflow / Agent và quyết định Go. |
| 03 — Individual Reflection | Nêu đóng góp cá nhân, cách dùng AI, bài học, điểm thay đổi sau khi bị challenge và điều sẽ làm khác nếu làm lại. |
