---
lang: vi
lang_alt: reference-manuals/geotechnical-engineers-handbook/chapter-08-retaining-walls/
---
# Chương 8 — Phân tích tường chắn

Chương VIII bàn về áp lực đất và các kết cấu chống lại nó. Chương mở đầu bằng lý thuyết
áp lực chủ động và bị động cổ điển, rồi xử lý **tường chắn cứng** (trọng lực và
công-xôn) và **tường chắn mềm** (tường cừ và tường vữa), kể cả tường có neo và hố đào
chống xà.

## 8.1 Áp lực chủ động và bị động

### 8.1.1 Trường hợp đất dính ($\varphi = 0$, $c \neq 0$)

Với tường chắn đứng, mặt đất sau tường nằm ngang và bỏ qua ma sát tường–đất, **áp lực
chủ động** là giá trị *nhỏ nhất* của áp lực ngang mà khối đất tác dụng lên tường — trạng
thái mà tường đã dịch ra đủ xa để đất huy động sức kháng cắt dọc mặt phá hoại:

$$\sigma_a = K_a\,\sigma'_z - 2c\sqrt{K_a}$$

trong đó $\sigma'_z$ là áp lực cột đất hữu hiệu, $c$ là lực dính kết, và $K_a$ là **hệ
số áp lực chủ động**.

**1. Xác định hệ số $K_a$** theo biểu thức:

$$K_a = \tan^2\!\left(45^\circ - \frac{\varphi}{2}\right) = \frac{1 - \sin\varphi}{1 + \sin\varphi}$$

**2. Lực chủ động $Q_a$** với tường cao $H$:

$$Q_a = \tfrac{1}{2}H\,\sigma_a = \tfrac{1}{2}K_a\,\gamma\,H^2$$

và điểm tác dụng của lực ở $\tfrac{1}{3}H$ tính từ chân tường.

### 8.1.2 Trường hợp đất rời

Cùng khung lý thuyết với $c = 0$, kể thêm ảnh hưởng của ma sát tường và mặt đất dốc.

![Figure: foundation-retaining-wall-forces](../../../assets/figures/foundation-retaining-wall-forces.svg)

**Hình.** Áp lực đất tác dụng lên tường chắn.

## 8.2 Phân tích tường chắn cứng

### 8.2.1 Định nghĩa và phân loại
Tường trọng lực, bán trọng lực và tường công-xôn.

### 8.2.2 Phân tích tường chắn cứng
Kiểm tra ổn định chống **lật**, **trượt** và **phá hoại nền**, cùng thiết kế kết cấu
thân tường.

### 8.2.3 Một số dạng tường chắn cứng – thấp

## 8.3 Phân tích tường chắn mềm

### 8.3.1 Định nghĩa, phân loại
Tường cừ và tường vữa (slurry wall).

### 8.3.2 Phân tích dải tường chắn ngàm chân
### 8.3.3 Phân tích dải tường chắn có neo
### 8.3.4 Phân tích hố đào với tường chống xà

Hố đào chống xà — trường hợp gần nhất với hố đào sâu trong đô thị và với phần quan trắc
trên trang [Móng & Đào đất](../../applications/foundations.md) của trang web này.

### 8.3.5 Ổn định đáy hố đào và biến dạng thành hố đào

## 8.4 Thuật ngữ

| Tiếng Anh | Tiếng Việt (sách dùng) |
| --- | --- |
| retaining wall | tường chắn |
| active earth pressure | áp lực chủ động |
| passive earth pressure | áp lực bị động |
| earth pressure at rest | áp lực tĩnh (nghỉ) |
| coefficient of active earth pressure | hệ số áp lực chủ động |
| active thrust | lực chủ động |
| rigid wall | tường chắn cứng |
| flexible wall | tường chắn mềm |
| cantilever wall | tường công-xôn |
| sheet pile | tường cừ |
| anchored wall | tường chắn có neo |
| braced excavation | hố đào chống xà |

## 8.5 Các điểm then chốt

- **Chủ động** là áp lực nhỏ nhất; **bị động** là lớn nhất; **tĩnh** nằm ở giữa.
- Với đất dính, $\sigma_a = K_a\sigma'_z - 2c\sqrt{K_a}$ và
  $K_a = \tan^2(45^\circ - \varphi/2)$.
- Lực chủ động lên tường cao $H$ là $Q_a = \tfrac{1}{2}K_a\gamma H^2$, tác dụng ở
  $\tfrac{1}{3}H$ trên chân tường.
- Tường cứng được kiểm tra **lật, trượt và phá hoại nền**.
- Tường mềm (cừ, vữa) và **hố đào chống xà** là trường hợp then chốt cho quan trắc hố
  đào sâu trong đô thị.
