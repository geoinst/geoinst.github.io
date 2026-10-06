---
lang: vi
lang_alt: reference-manuals/foundation-engineering/chapter-03-bearing-capacity/
---
# Chương 3 — Móng nông: Sức chịu tải

## 3.1 Bài toán sức chịu tải

Móng nông (thường là móng có độ sâu $D_f$ nhỏ hơn bề rộng $B$) phải truyền tải công
trình xuống nền mà **không gây phá hoại cắt** cho đất đỡ. **Sức chịu tải cực hạn**
$q_{ult}$ là áp lực mà tại đó đất phá hoại; **áp lực chịu tải cho phép** là $q_{ult}$
chia cho hệ số an toàn, đồng thời phải kiểm tra theo lún
([Chương 4](chapter-04-settlement.md)).

## 3.2 Cơ chế phá hoại

Phá hoại sức chịu tải xảy ra theo một trong ba cách, tùy mật độ và tính nén của đất:

- **Cắt tổng thể** — nêm và mặt trượt rõ ràng; phá hoại giòn, đột ngột. Điển hình ở cát
  chặt và sét cứng.
- **Cắt cục bộ** — mặt trượt kém phát triển, lún đáng kể trước khi phá hoại. Điển hình
  ở đất mật độ trung bình.
- **Cắt xuyên (punching)** — móng xuyên vào đất, ít trồi mặt. Điển hình ở cát rời và sét
  yếu.

![Figure: foundation-bearing-failure](../../../assets/figures/foundation-bearing-failure.svg)

**Hình.** Các cơ chế phá hoại sức chịu tải: cắt tổng thể (giòn), cắt cục bộ và cắt xuyên (dẻo) (theo USACE EM 1110-1-1905).

## 3.3 Phương trình sức chịu tải

Lời giải cổ điển biểu diễn $q_{ult}$ thành tổng ba thành phần:

$$q_{ult} = c N_c s_c + q N_q s_q + \tfrac{1}{2} \gamma B N_\gamma s_\gamma$$

trong đó $c$ là lực dính, $q$ là tải tác dụng ở cao độ đáy móng, $\gamma$ là dung trọng,
$B$ là bề rộng móng, $N_c, N_q, N_\gamma$ là **hệ số sức chịu tải** (hàm của góc ma sát),
và các số hạng $s$ là **hệ số hình dạng**. Có nhiều công thức đang dùng — **Terzaghi**,
**Meyerhof**, **Hansen** và **Vesić** — khác nhau ở các hệ số và cách xử lý hình dạng, độ
sâu, độ nghiêng và độ lệch tâm.

## 3.4 Mực nước ngầm

Nước ngầm làm giảm ứng suất hữu hiệu trong vùng phá hoại, hạ thấp sức chịu tải. Hai
trường hợp cực trị:

- mực nước ngầm **ở đáy móng**, và
- mực nước ngầm **ở mặt đất**.

Ở khoảng giữa, các số hạng dung trọng được giảm theo một hệ số phụ thuộc độ sâu mực nước
so với $B$. Thiết kế phải dùng **mực nước cao nhất dự kiến** cho sức chịu tải tới hạn
(nhỏ nhất).

## 3.5 Tải lệch tâm và nghiêng

Móng thực tế chịu tải **lệch tâm** (mô men) và đôi khi **nghiêng**. Cách chuẩn là thay
móng thực bằng một **diện tích hữu hiệu** $B' \times L'$ (Meyerhof), đặt dưới hợp lực
tải, và áp các hệ số nghiêng. Độ lệch tâm làm giảm cả diện tích chịu tải hữu hiệu lẫn
sức chịu tải.

## 3.6 Sức chịu tải từ thí nghiệm tại chỗ

Nơi khó lấy mẫu, sức chịu tải được ước lượng từ thí nghiệm hiện trường:

- **SPT** — tương quan giữa $N$ và áp lực cho phép, hiệu chỉnh theo mực nước ngầm và
  tải trên.
- **CPT** — sức chịu tải từ sức kháng mũi côn.
- **Thí nghiệm bàn nén** — đo trực tiếp tại chỗ phản ứng tải–lún của đất thực, ngoại
  suy cho móng nguyên mẫu một cách cẩn thận.

## 3.7 Các điểm then chốt cần ghi nhớ

- **Sức chịu tải cực hạn ÷ hệ số an toàn = áp lực cho phép** — nhưng lún thường chi phối.
- Nắm **cơ chế phá hoại**: cắt tổng thể, cục bộ hay xuyên.
- Phương trình sức chịu tải gồm **ba số hạng** (lực dính, tải trên, trọng lượng bản thân)
  cùng hệ số hình dạng/độ sâu/độ nghiêng.
- Dùng **mực nước ngầm cao nhất** trong thiết kế.
- Chuyển **tải lệch tâm** thành diện tích hữu hiệu.
- **Thí nghiệm bàn nén** đo phản ứng đất thực; dùng kèm phán đoán.
