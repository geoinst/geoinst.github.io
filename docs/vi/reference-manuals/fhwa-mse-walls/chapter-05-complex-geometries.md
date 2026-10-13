---
lang: vi
lang_alt: reference-manuals/fhwa-mse-walls/chapter-05-complex-geometries/
---
# Chương 5 — Tường MSE với Hình học Phức tạp

## 5.1 Mố cầu

Một **mố cầu MSE** chịu tải gối cầu ngoài áp lực đất, và các tải đó đi vào khối đất
có cốt ở phía trên — nơi cốt ít có khả năng phân phối lại nhất. Đây là ứng dụng MSE
khắt khe nhất, và sổ tay xử lý nó rất kỹ.

**Mố cầu MSE trên móng nông.** Móng chịu trên đất đắp có cốt (hoặc trên nền phía sau),
và tải của nó (thẳng đứng, ngang và mô men) được truyền vào khối đất có cốt và đất
nền. Thiết kế phải kiểm tra:

- **Sức chịu tải** dưới móng, kể cả độ lệch tâm do tải cầu.
- **Ổn định trong** khi cộng tải móng như một tải chất lớn — lực kéo trong các lớp cốt
  phía trên tăng mạnh.
- **Trượt** của khối đất có cốt dưới tải ngang của cầu.
- **Ổn định tổng thể** xuyên qua mố và nền của nó.
- **Lún** của móng và đường đầu cầu, cùng **dung sai** cho chuyển vị không đều giữa
  gối cầu và bản quá độ.

**Mố cầu MSE trên móng cọc.** Khi nền quá yếu cho móng nông, mố được đỡ trên **cọc**,
và tường MSE được xây quanh chúng. Cách này tách lún của cầu khỏi lún của tường nhưng
sinh ra vấn đề riêng: cọc làm gián đoạn cốt, đài cọc tạo tải tập trung, và thiết kế
phải đảm bảo cốt không bị hư hại do đóng cọc hoặc do chuyển vị của đài cọc.

## 5.2 Tường xếp lớp (nhiều bậc)

Khi hai hay nhiều tường MSE xếp chồng với một cơ giữa chúng, tường dưới chịu tải chất
của tường trên. Sổ tay đưa **quy tắc thiết kế** cho tường xếp lớp: khoảng cách lệch
giữa các tường, chiều dài cốt trong mỗi tường, và cách tải của tường trên được trải
lên tường dưới. Bỏ qua tương tác — thiết kế mỗi tường như thể nó đứng riêng — là một
lỗi kinh điển.

## 5.3 Tường có chiều dài cốt không đều

Khi chiều dài cốt phải thay đổi dọc theo tường (do vật cản, hình học hoặc tải thay
đổi), thiết kế vẫn phải đảm bảo một khối đất có cốt **liên tục** và kiểm tra các vùng
chuyển tiếp nơi chiều dài thay đổi, vì các đoạn ngắn hơn huy động sức kháng nhổ ít hơn
và có thể trở thành điểm yếu.

## 5.4 Tường lưng tựa lưng

Khi hai tường đối mặt nhau với một khối đất hẹp ở giữa, các vùng có cốt có thể **chồng
lấn**. Sổ tay phân biệt các trường hợp theo tỷ số giữa khoảng cách và chiều cao tường:

- **Khoảng cách rộng** — mỗi tường được thiết kế độc lập.
- **Khoảng cách hẹp** — các vùng có cốt chồng lấn và hai tường ứng xử như một khối hỗn
  hợp; thiết kế phải xem khối đó là một.
- **Khoảng cách rất hẹp** — hai mặt tường thực chất tạo thành một tường đơn với cốt
  xuyên suốt toàn bộ chiều rộng.

## 5.5 Chi tiết

Các chi tiết riêng cho mố gồm **gối cầu**, mối nối **bản quá độ**, cách bố trí **gối
đỡ** và **thoát nước** phía sau và xuyên qua mố — tất cả đều phải chấp nhận được biến
dạng ra ngoài của tường mà không bị hư hại.

## 5.6 Ví dụ thiết kế, mố cầu

Sổ tay giải trọn một mố cầu — hình học, tải cầu, ổn định ngoài, ổn định trong với tải
chất của móng, và bố trí cốt kết quả — bằng tính tay và bằng chương trình máy tính.

## 5.7 Các điểm then chốt cần ghi nhớ

- **Mố cầu là một bức tường cộng một tải tập trung ở đỉnh** — đường truyền tải vào cốt
  và vào nền phải được nêu rõ.
- **Mố trên cọc** tách lún nhưng làm gián đoạn cốt; phải cấu tạo mặt tiếp giáp cẩn thận.
- **Tường xếp lớp và lưng tựa lưng tương tác** — thiết kế cả hệ thống, không thiết kế
  từng tường riêng lẻ.
- **Chiều dài cốt không đều** tạo các vùng chuyển tiếp phải được kiểm tra.
- Phải chấp nhận **biến dạng và lún không đều** tại gối cầu, nếu không đường đầu cầu
  sẽ nứt.
