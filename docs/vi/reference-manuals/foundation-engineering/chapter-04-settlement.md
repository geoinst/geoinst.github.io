---
lang: vi
lang_alt: reference-manuals/foundation-engineering/chapter-04-settlement/
---
# Chương 4 — Móng nông: Lún

## 4.1 Vì sao lún thường chi phối

Với hầu hết công trình trên nền tốt, **tiêu chí chi phối không phải sức chịu tải mà là
lún**. Một móng có thể còn xa phá hoại cắt mà vẫn lún đủ nhiều để làm nứt lớp hoàn
thiện, biến dạng khung hoặc lệch máy móc. Vì vậy thiết kế phải tính lún và so với **biến
dạng cho phép** của công trình.

## 4.2 Ba thành phần của lún

Tổng lún gồm ba phần:

1. **Lún tức thời (đàn hồi)** — xảy ra ngay khi đặt tải, do nén đàn hồi và biến dạng
   ngang của đất. Đáng kể ở cát và đất không bão hòa.
2. **Lún cố kết sơ cấp** — thoát nước và thay đổi thể tích theo thời gian ở đất hạt mịn
   bão hòa, chi phối bởi **lý thuyết cố kết một chiều Terzaghi**. Có thể mất hàng tháng
   đến hàng năm.
3. **Lún thứ cấp (từ biến)** — thay đổi thể tích tiếp diễn ở ứng suất hữu hiệu không
   đổi, đặc biệt ở sét hữu cơ và sét yếu.

![Figure: foundation-settlement](../../../assets/figures/foundation-settlement.svg)

**Hình.** Ba thành phần lún của móng — tức thời, cố kết sơ cấp và thứ cấp — tích lũy theo thời gian (theo USACE EM 1110-1-1904).

## 4.3 Lún tức thời

Lún tức thời được tính từ **lý thuyết đàn hồi**:

$$S_e = q B \frac{1-\nu^2}{E} I_s$$

trong đó $q$ là áp lực tác dụng, $B$ bề rộng móng, $E$ và $\nu$ mô đun đàn hồi và hệ số
Poisson của đất, và $I_s$ hệ số ảnh hưởng phụ thuộc hình dạng và độ cứng móng. Ở cát, $E$
thường được ước lượng từ tương quan **SPT hoặc CPT**.

## 4.4 Lún cố kết sơ cấp

Với sét cố kết thường:

$$S_c = \frac{C_c H}{1+e_0}\log\frac{\sigma'_{v0}+\Delta\sigma}{\sigma'_{v0}}$$

trong đó $C_c$ là chỉ số nén, $H$ chiều dày tầng, $e_0$ hệ số rỗng ban đầu,
$\sigma'_{v0}$ ứng suất hữu hiệu ban đầu, và $\Delta\sigma$ gia tăng ứng suất. Với sét
quá cố kết, dùng **chỉ số nén lại** $C_r$ cho tới áp lực tiền cố kết. **Tốc độ theo thời
gian** do hệ số cố kết $c_v$ chi phối.

## 4.5 Lún của đất hạt rời

Ở cát, cố kết hầu như tức thời, và lún được ước lượng từ **tương quan kinh nghiệm** với
SPT $N$, sức kháng mũi CPT hoặc **thí nghiệm bàn nén**, có hiệu chỉnh theo bề rộng móng và
mực nước ngầm. Vì cát rất biến đổi, các ước lượng này mang độ bất định lớn.

## 4.6 Biến dạng cho phép và lún lệch

Thiết kế không bị chi phối bởi lún tuyệt đối mà bởi:

- **tổng lún** — không được làm hỏng chức năng công trình;
- **lún lệch** — *chênh lệch* giữa các điểm kề nhau, gây biến dạng, thường là tiêu chí
  tới hạn;
- **độ nghiêng góc** — lún lệch chia cho nhịp giữa các điểm.

Giới hạn phụ thuộc loại công trình (nhà, cầu, máy móc) và được nêu trong sổ tay thiết kế
và tiêu chuẩn.

## 4.7 Các điểm then chốt cần ghi nhớ

- **Lún, chứ không phải sức chịu tải, thường chi phối** thiết kế móng nông.
- Tổng lún = **tức thời + cố kết sơ cấp + thứ cấp**.
- Dùng **lý thuyết đàn hồi** cho tức thời, **lý thuyết cố kết** cho sét, **tương quan
  kinh nghiệm** cho cát.
- **Lún lệch và độ nghiêng góc** là tiêu chí sử dụng thực sự.
- Quan trắc lún thực bằng **bàn lún và extensometer** (xem tài liệu [FHWA](../fhwa/index.md)).
