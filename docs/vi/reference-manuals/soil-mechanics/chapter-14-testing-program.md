---
lang: vi
lang_alt: reference-manuals/soil-mechanics/chapter-14-testing-program/
---
# Chương 14 — Chương trình thí nghiệm phòng & hiện trường

## 14.1 Bắt đầu từ câu hỏi

Chương trình thí nghiệm không phải danh sách mua sắm — nó **do các câu hỏi thiết kế dẫn
dắt**. Trước khi định thí nghiệm nào, hãy hỏi:

- Thí nghiệm này phục vụ quyết định nào?
- Cần thông số nào, với độ chính xác nào?
- Phân tích nào sẽ dùng nó (lún, ổn định, sức chịu tải, thấm)?

Đây chính là kỷ luật **"không câu hỏi, không thiết bị"** như trong quan trắc (xem tài liệu
[FHWA](../fhwa/index.md)).

## 14.2 Khớp thí nghiệm với thông số

| Thông số | Thí nghiệm thường dùng |
|----------|------------------------|
| Chỉ tiêu cơ lý, phân loại | Rây, tỷ trọng kế, giới hạn Atterberg, độ ẩm |
| Đầm chặt | Proctor (tiêu chuẩn/cải tiến), dung trọng hiện trường |
| Tính thấm | Cột nước không đổi/giảm dần, bơm hút hiện trường |
| Cố kết ($C_c$, $c_v$, $\sigma'_p$) | Oedometer |
| Sức kháng cắt ($c'$, $\phi'$, $c_u$) | Cắt trực tiếp, ba trục (UU/CU/CD), cắt cánh |
| Độ cứng ($E$, $G$) | Ba trục, pressuremeter, địa chấn, bàn nén |
| Sức kháng hóa lỏng | SPT/CPT với tương quan chu kỳ |

## 14.3 Chương trình phòng thí nghiệm

- **Thí nghiệm chỉ tiêu** — rẻ, nhanh, chạy trên nhiều mẫu để mô tả tính biến đổi.
- **Phân loại** — tối thiểu một mẫu mỗi tầng.
- **Cường độ và cố kết** — nhắm vào các **tầng tới hạn** xác định từ mô hình nền.
- **Chất lượng mẫu quan trọng** — xáo trộn làm thay đổi cường độ và độ cứng; dùng mẫu nguyên
  dạng chất lượng cao cho thông số then chốt.

## 14.4 Chương trình hiện trường

- **Thí nghiệm tại chỗ** ([Chương 12](chapter-12-in-situ-testing.md)) cho thông số nơi khó
  lấy mẫu hoặc xáo trộn là vấn đề.
- **Quan trắc nước ngầm** bằng piezometer, theo thời gian để nắm dải theo mùa.
- **Thử tải** nơi sức chịu tải then chốt và sai sót tốn kém.

## 14.5 Báo cáo và diễn giải

Kết quả thí nghiệm phải được **rút gọn thành thông số thiết kế** với cơ sở được ghi lại:

- báo cáo **dải giá trị**, không chỉ giá trị trung bình;
- nêu **giả định** trong diễn giải;
- **đối chiếu** giá trị phòng và hiện trường — khác biệt lớn cho thấy vấn đề;
- **so sánh** với kinh nghiệm địa phương và tương quan công bố.

## 14.6 Các điểm then chốt cần ghi nhớ

- Để **câu hỏi thiết kế** dẫn dắt chương trình thí nghiệm.
- Khớp **mỗi thí nghiệm với một thông số** và phân tích dùng nó.
- Dùng **thí nghiệm chỉ tiêu** rộng rãi và **cường độ/cố kết** trên tầng tới hạn.
- **Chất lượng mẫu** quyết định với cường độ và độ cứng.
- Báo cáo **dải và cơ sở**, và **đối chiếu** phòng với hiện trường.
