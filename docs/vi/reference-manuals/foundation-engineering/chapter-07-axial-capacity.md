---
lang: vi
lang_alt: reference-manuals/foundation-engineering/chapter-07-axial-capacity/
---
# Chương 7 — Móng sâu: Sức chịu tải dọc trục

## 7.1 Phương trình sức chịu tải

**Sức chịu tải dọc trục cực hạn** của một cọc đơn là tổng sức kháng thành bên và sức kháng
mũi:

$$Q_{ult} = Q_s + Q_p - W$$

trong đó $Q_s$ là **sức kháng thành bên (ma sát)**, $Q_p$ là **sức kháng mũi**, và $W$ là
trọng lượng cọc (thường bỏ qua). **Sức chịu tải cho phép** là $Q_{ult}$ chia cho hệ số an
toàn, và cũng phải thỏa mãn tiêu chí lún.

## 7.2 Sức kháng thành bên trong sét

Trong sét, sức kháng thành bên thường được tính bằng **phương pháp ứng suất tổng (α)**:

$$Q_s = \alpha \, c_u \, A_s$$

trong đó $c_u$ là sức kháng cắt không thoát nước, $A_s$ là diện tích thành bên, và $\alpha$
là hệ số dính bám (thường ~0,5, giảm khi $c_u$ tăng). **Phương pháp ứng suất hữu hiệu (β)**
cũng được dùng, đặc biệt cho điều kiện dài hạn.

## 7.3 Sức kháng thành bên trong cát

Trong cát, sức kháng thành bên được tính bằng **phương pháp ứng suất hữu hiệu (β)**:

$$Q_s = \beta \, \sigma'_v \, A_s = K \tan\delta \, \sigma'_v \, A_s$$

trong đó $\sigma'_v$ là ứng suất hữu hiệu thẳng đứng, $K$ là hệ số áp lực đất ngang, và
$\delta$ là góc ma sát cọc–đất. **Phương pháp λ** và **α** là các lựa chọn thay thế cho điều
kiện cụ thể.

## 7.4 Sức kháng mũi

Sức kháng mũi phụ thuộc việc mũi cọc tựa trên đá, cát chặt hay sét:

- **Trong sét:** $Q_p = 9 \, c_u \, A_p$ (với $c_u$ ở mũi).
- **Trong cát:** $Q_p = q'N_q A_p$ (hoặc tương quan SPT/CPT), có giới hạn để kể tới độ sâu
  hữu hạn mà áp lực mũi huy động.
- **Trên đá:** sức chịu tải từ cường độ nén một trục của đá với các hệ số giảm.

## 7.5 Sức chịu tải từ thí nghiệm tại chỗ

Phân tích tĩnh được kiểm tra và thường hiệu chuẩn theo thí nghiệm hiện trường:

- **Tương quan SPT và CPT** — sức chịu tải ước lượng từ sức kháng xuyên.
- **Thử tải cọc tĩnh** — phép đo xác định nhất, tải gia tăng theo cấp và ghi lún.
- **Thử động (PDA)** — thử động biến dạng cao trong khi đóng cho sức chịu tải và tính
  toàn vẹn.
- **Thử tải Statnamic và tải nhanh** — thay thế khi thử tĩnh bất khả thi.

## 7.6 Thử tải có lắp thiết bị

Các thử tải nhiều thông tin nhất là **có lắp thiết bị**: cảm biến đo biến dạng (strain gauge) hoặc **thanh thép đo biến dạng phụ (sister bar)** dọc
thân cọc và **thanh truyền chuyển vị (telltale)** hay **thiết bị đo biến dạng sâu (extensometer)** đo phân bố tải giữa thành bên và mũi, tách
trực tiếp hai thành phần (xem tài liệu [FHWA](../fhwa/index.md), Chương 8, và ví dụ
**Phụ lục D**).

## 7.7 Hệ số an toàn và LRFD

Thiết kế theo ứng suất cho phép dùng hệ số an toàn trên sức chịu tải cực hạn (thường
2,5–4 cho tải làm việc). **LRFD** thay vào đó áp **hệ số sức kháng** riêng cho thành bên và
mũi, phản ánh độ tin cậy khác nhau của chúng.

## 7.8 Các điểm then chốt cần ghi nhớ

- **$Q_{ult} = Q_s + Q_p$** — ma sát thành bên cộng sức kháng mũi.
- Dùng **phương pháp α/β/λ** cho thành bên, và **9$c_u$ / $q'N_q$** cho mũi.
- **Hiệu chuẩn** phân tích tĩnh bằng **thử tải, tương quan SPT/CPT và thử động**.
- **Thử tải có lắp thiết bị** tách thành bên khỏi mũi — chuẩn vàng.
- Ứng suất cho phép dùng **hệ số an toàn**; LRFD dùng **hệ số sức kháng**.
