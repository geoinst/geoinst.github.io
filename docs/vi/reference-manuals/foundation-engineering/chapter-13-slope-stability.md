---
lang: vi
lang_alt: reference-manuals/foundation-engineering/chapter-13-slope-stability/
---
# Chương 13 — Ổn định mái dốc

## 13.1 Vì sao mái dốc phá hoại

Mái dốc phá hoại khi **ứng suất cắt** dọc mặt trượt tiềm năng vượt **sức kháng cắt** của
đất. **Hệ số an toàn** là tỷ số giữa sức kháng khả dụng và ứng suất huy động:

$$F = \frac{\tau_{khả dụng}}{\tau_{huy động}}$$

Phá hoại có thể **đột ngột** (giòn, ở đất chặt hoặc đá) hoặc **tiến triển** (sét yếu, đá
phong hóa), và có thể do mưa, đào, chất tải hoặc động đất kích hoạt.

## 13.2 Mái dốc vô hạn

Với mái dốc dài, đồng nhất, nơi mặt trượt song song với mặt dốc, hệ số an toàn có lời giải
dạng kín. Hai trường hợp quan trọng:

- **Mái dốc khô hoặc thoát nước** — do góc ma sát và góc dốc chi phối.
- **Có thấm** — áp lực nước lỗ rỗng làm giảm ứng suất hữu hiệu và hệ số an toàn, thường rất
  mạnh. Đây là lý do **thoát nước** là biện pháp ổn định chính.

## 13.3 Mái dốc hữu hạn và phương pháp phân mảnh

Mái dốc thực được phân tích bằng **phương pháp cân bằng giới hạn**, chia khối trượt tiềm
năng thành các **mảnh thẳng đứng**:

- **Phương pháp phân mảnh thông thường (Fellenius)** — đơn giản, thiên an toàn.
- **Phương pháp đơn giản hóa Bishop** — kể đến lực giữa các mảnh, là công cụ chủ lực trong
  thực hành.
- **Spencer** và **Morgenstern–Price** — nghiêm ngặt, thỏa mãn mọi điều kiện cân bằng.

Phân tích tìm **mặt trượt tới hạn** — mặt cho hệ số an toàn nhỏ nhất. Phương pháp máy tính
(ví dụ **STABL**, **SLOPE/W**) tự động hóa việc tìm kiếm.

![Figure: foundation-slope-stability](../../../assets/figures/foundation-slope-stability.svg)

**Hình.** Ổn định mái dốc bằng phương pháp phân mảnh: lực gây trượt và lực kháng trên mỗi mảnh, và việc tìm mặt trượt tới hạn (theo USACE EM 1110-2-1902).

## 13.4 Điều kiện ngắn hạn và dài hạn

- **Ngắn hạn (không thoát nước)** — ngay sau thi công hoặc đào, dùng **sức kháng cắt không
  thoát nước** $c_u$; tới hạn với sét yếu.
- **Dài hạn (thoát nước)** — sau khi áp lực nước lỗ rỗng cân bằng, dùng thông số **ứng suất
  hữu hiệu** $c', \phi'$; thường tới hạn ở sét cứng và mái dốc có thấm.

Phải kiểm tra cả hai, và **hệ số an toàn nhỏ hơn** chi phối.

## 13.5 Biện pháp ổn định

Khi mái dốc mất ổn định, các lựa chọn gồm:

- **Thoát nước** — mặt và ngầm; hiệu quả và kinh tế nhất.
- **Sửa dốc** — làm thoải mái dốc hoặc thêm bệ chân.
- **Kết cấu chắn** — tường, cừ hoặc đất có cốt ở chân.
- **Gia cố nền** — neo đất, neo hoặc cốt gia cường
  ([Chương 14](chapter-14-ground-improvement.md)).
- **Gia cường** — neo đất, tie-back hoặc vải địa kỹ thuật.

## 13.6 Các điểm then chốt cần ghi nhớ

- Mái dốc phá hoại khi **ứng suất cắt vượt sức kháng cắt**; hệ số an toàn là tỷ số.
- **Thấm** làm giảm hệ số an toàn — **thoát nước** là biện pháp chính.
- Dùng **phương pháp phân mảnh** (Bishop cho thực hành) và tìm **mặt trượt tới hạn**.
- Kiểm tra **ngắn hạn và dài hạn**; $F$ nhỏ hơn chi phối.
- Ổn định bằng **thoát nước, sửa dốc, kết cấu chắn hoặc gia cường**.
