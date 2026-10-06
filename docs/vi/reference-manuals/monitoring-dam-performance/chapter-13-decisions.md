---
lang: vi
lang_alt: reference-manuals/monitoring-dam-performance/chapter-13-decisions/
---
# Chương 13 — Đánh giá vận hành và ra quyết định

## 13.1 Giám sát tồn tại để hỗ trợ ra quyết định

Mục đích của tất cả công việc trước đó là một câu trả lời có thể bảo vệ được cho
một câu hỏi: **dựa trên những gì giám sát cho thấy, chúng ta nên làm gì?** Chương
này kết nối đo lường với hành động.

## 13.2 Phản ứng có cấu trúc trước bất thường

Khi một ngưỡng bị vượt quá hoặc một đánh giá tìm thấy một sai lệch thực sự:

1. **Xác minh** — xác nhận rằng đó không phải là lỗi cảm biến hay dữ liệu.
2. **Đánh giá** — so sánh với mode hư hỏng mà nó bảo vệ; xếp hạng mức độ nghiêm trọng.
3. **Tăng cường** — tăng tần suất đọc và điều động kiểm tra
   ([Chương 3](chapter-03-philosophy.md)).
4. **Quyết định** — tiếp tục bình thường, điều tra, hạn chế vận hành hồ, hoặc
   hành động khắc phục.
5. **Tài liệu hóa** — ghi lại quyết định và cơ sở của nó.

## 13.3 Các mức hành động

Nhiều chương trình xác định các **mức hành động** theo bậc gắn với ngưỡng:

| Mức | Ý nghĩa | Phản ứng |
|-----|---------|----------|
| Bình thường (Normal) | Trong đường cơ sở | Giám sát định kỳ |
| Cảnh báo (Alert) | Vượt dải đường cơ sở | Xem xét, xác minh, theo dõi |
| Báo động (Alarm) | Vượt ngưỡng nguy hiểm | Tăng cường, hạn chế vận hành, thông báo |

Các mức này chuyển những con số thô thành một phản ứng chia sẻ, đã được thỏa thuận
trước — nhanh hơn và bớt cảm xúc hơn trong một tình huống khẩn cấp.

## 13.4 Vận hành hồ như một đòn bẩy

Thường thì hành động tức thời nhất là vận hành: **hạ mực nước hồ** để giảm tải
trọng và thấm trong khi tìm nguyên nhân. Dữ liệu giám sát biện minh và hướng dẫn
quyết định đó theo thời gian thực.

## 13.5 Phán đoán có căn cứ rủi ro

Các quyết định cân nhắc **hậu quả** của hư hỏng so với **mức độ tin cậy** của xu
hướng quan sát được. Một thay đổi nhỏ, được giải thích rõ trên một hạng mục hậu
quả thấp có thể chỉ cần giám sát; cùng thay đổi đó trên một mode hư hỏng hậu quả
cao đòi hỏi hành động khẩn cấp. Không có quy tắc phổ quát nào — phán đoán, được
thông tin bởi giám sát, là cần thiết.

## 13.6 Khép kín vòng lặp

Một chương trình tốt biết học hỏi. Mỗi bất thường, dù lành tính hay nghiêm trọng,
đều cập nhật đường cơ sở, các ngưỡng và kế hoạch. Trong suốt tuổi thọ của đập, bản
thân chương trình giám sát được cải thiện.

## 13.7 Điểm mấu chốt

- Mục đích của giám sát là một quyết định có thể bảo vệ: chúng ta nên làm gì?
- Phản ứng theo xác minh → đánh giá → tăng cường → quyết định → tài liệu hóa.
- Các mức hành động đã thỏa thuận trước giúp tình huống khẩn cấp nhanh hơn và bình tĩnh hơn.
- Vận hành hồ thường là đòn bẩy đầu tiên; phán đoán cân nhắc hậu quả so với mức độ tin cậy.
