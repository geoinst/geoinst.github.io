---
lang: vi
lang_alt: reference-manuals/fhwa-mse-walls/chapter-07-design-rss/
---
# Chương 7 — Thiết kế Mái dốc Đất có cốt

## 7.1 Giới thiệu

Thiết kế mái dốc có cốt nâng hệ số an toàn của một mái dốc bằng cách thêm cốt gia cường
xuyên qua các mặt trượt tiềm tàng. Lực cốt được đưa vào một **phân tích cân bằng giới
hạn cải tiến**: mô men chống của cốt (lực kéo nhân cánh tay đòn quanh tâm quay) được
cộng vào mô men chống của đất, và chiều dài cốt phía sau mặt trượt phải đủ để huy động
lực kéo đó bằng sức kháng nhổ.

Vì mặt trượt tới hạn không biết trước, thiết kế mang tính lặp: chọn một mặt trượt, tính
cốt cần thiết, kiểm tra rằng cốt huy động được lực của nó bằng sức kháng nhổ, rồi tìm
lại mặt trượt tới hạn với cốt đã đưa vào.

![Figure: rss-slope-anatomy](../../../assets/figures/rss-slope-anatomy.svg)

**Hình.** Mặt cắt ngang điển hình của mái dốc đất có cốt: các lớp cốt gia cường kéo dài
từ mặt dốc phủ thực vật vào tận đất ổn định phía sau mặt trượt tới hạn, với mặt dốc
đứng ở góc β (theo FHWA-NHI-00-043, Ch. 6–7).

## 7.2 Hướng dẫn thiết kế mái dốc có cốt

Sổ tay đặt ra một **quy trình chín bước**:

**Bước 1 — Thiết lập yêu cầu hình học, tải trọng và hiệu năng.** Hình học mái dốc, tải
ngoài (giao thông, kết cấu), hệ số an toàn yêu cầu và tiêu chí hiệu năng.

**Bước 2 — Xác định thông số kỹ thuật của đất nguyên trạng.** Trọng lượng đơn vị, cường
độ kháng cắt (thoát nước và không thoát nước) và chế độ áp lực lỗ rỗng của nền hiện hữu
và đất nền.

**Bước 3 — Xác định thông số của đất đắp có cốt (và, nếu khác, đất lưng tường).** Trọng
lượng đơn vị, góc ma sát và giới hạn độ hạt/độ dẻo cho đất đắp có cốt.

**Bước 4 — Đánh giá thông số thiết kế cho cốt gia cường.** Cường độ cho phép dài hạn —
sau khi giảm do từ biến, hư hại khi thi công và độ bền với vật liệu địa kỹ thuật tổng
hợp, hoặc sau tổn thất ăn mòn với thép — cùng hệ số ma sát nhổ $F^{*}$ và hệ số tỷ lệ
$\alpha$ cho cặp đất–cốt.

**Bước 5 — Kiểm tra ổn định khi chưa có cốt.** Phân tích mái dốc không có cốt để xác
lập hệ số an toàn nền tảng và định vị mặt trượt tới hạn. Bước này cho biết cần bao nhiêu
cốt.

**Bước 6 — Thiết kế cốt để đảm bảo mái dốc ổn định.** Chọn bố trí cốt (khoảng cách, chiều
dài, cường độ) sao cho mái dốc có cốt đạt hệ số an toàn yêu cầu. **Lực cốt yêu cầu** được
tìm từ hiệu giữa mô men chống yêu cầu và mô men chống sẵn có:

$$T_{yc} = \frac{FS_{yc}\ \cdot\ M_{gây\ trượt} - M_{chống}}{\sum (\text{cánh tay đòn}_i)}$$

Cốt được phân bố trên chiều cao mái dốc, thường gần nhau hơn ở chân dốc nơi ứng suất gây
trượt lớn nhất, và mỗi lớp được kiểm tra **nhổ** phía sau mặt trượt tới hạn.

**Bước 7 — Kiểm tra ổn định ngoài.** Xác nhận mái dốc có cốt không trượt dọc một lớp nền
yếu, không làm nền quá tải về sức chịu tải, và không phá hoại trên một mặt trượt sâu đi
qua bên dưới vùng có cốt.

**Bước 8 — Ổn định động đất.** Áp dụng lực quán tính giả tĩnh và kiểm tra lại mái dốc có
cốt, cộng gia số động đất vào lực cốt.

**Bước 9 — Đánh giá yêu cầu kiểm soát nước ngầm và dòng chảy mặt.** Thiết kế thoát nước
sao cho áp lực lỗ rỗng trong vùng có cốt giữ ở giá trị thiết kế và nước mặt được chặn
lại và dẫn đi.

## 7.3 Thiết kế có hỗ trợ máy tính

Vì Bước 6 đòi hỏi tìm mặt trượt tới hạn khi đã có cốt, thiết kế RSS thường được thực
hiện bằng chương trình ổn định mái dốc có hỗ trợ phần tử cốt. Các ví dụ đã giải của sổ
tay gồm cả tính tay và lời giải máy tính tương ứng, để hai cách đối chiếu nhau.

## 7.4 Các ví dụ thiết kế

- **Ví dụ 1 — Thiết kế mái dốc có cốt, mở rộng đường.** Một mái dốc được mở rộng bằng
  cách dựng dốc mặt, thiết kế với các lớp cốt.
- **Ví dụ 2 — Thiết kế mái dốc có cốt, xây dựng đường mới.** Một mái dốc nền đắp mới
  được xây có cốt ngay từ đầu.
- **Ví dụ 3 — Lời giải có hỗ trợ máy tính.** Cùng bài toán được giải bằng chương trình
  ổn định mái dốc.
- **Ví dụ 4 — Tính ổn định mặt dốc.** Kiểm tra ổn định của mặt dốc (đoạn quấn và đất mặt)
  dưới chính lực của cốt.

## 7.5 Ước tính chi phí dự án

Sổ tay khép lại bằng một **quy trình ước tính chi phí** cho mái dốc có cốt — bóc tách
khối lượng cốt, đất đắp, xử lý mặt dốc và thoát nước — cũng là dữ liệu tham khảo đã cũ,
phải quy đổi về giá tại địa phương.

## 7.6 Các điểm then chốt cần ghi nhớ

- Thiết kế RSS là **cân bằng giới hạn có cốt mang tính lặp**: định vị mặt trượt tới hạn,
  cộng lực cốt, kiểm tra lại.
- **Bước 5 (ổn định khi chưa có cốt) cho biết cần bao nhiêu cốt**; không được bỏ qua.
- Phân bố cốt **gần nhau hơn ở chân dốc** nơi ứng suất gây trượt đạt đỉnh, và kiểm tra
  **nhổ** phía sau mặt trượt tới hạn cho mọi lớp.
- Kiểm tra **ổn định ngoài** độc lập — mái dốc có cốt vẫn có thể trượt trên nền yếu.
- **Thiết kế thoát nước (Bước 9)** là một phần của thiết kế ổn định, không phải chi tiết.
