---
lang: vi
lang_alt: reference-manuals/practical-rock-engineering/chapter-04-rock-mass-properties/
---

# Chương 4 — Tính Chất Khối Đá & Chỉ Số Cường Độ Địa Chất (GSI)

## 4.1 Tiêu Chuẩn Bền Phá Hoại Hoek-Brown Tổng Quát (Ấn Bản 2002)

Đối với các khối đá bị nứt nẻ mạnh, nơi mà kích thước của từng khối đá con là rất nhỏ so với quy mô hình học của công trình đào ngầm hay bờ moong, khối đá ứng xử tương đương như một môi trường tựa liên tục đẳng hướng. Hoek, Carranza-Torres và Corkum (2002) đã hoàn thiện phương trình đường bao phá hoại Hoek-Brown tổng quát:

$$\sigma_1' = \sigma_3' + \sigma_{ci} \left( m_b \frac{\sigma_3'}{\sigma_{ci}} + s \right)^a$$

Trong đó:
- $\sigma_{ci}$ = cường độ nén đơn trục của mẫu đá nguyên vẹn
- $m_b$ = giá trị suy giảm của hằng số vật liệu $m_i$ áp dụng cho khối đá:

$$m_b = m_i \exp \left( \frac{\text{GSI} - 100}{28 - 14D} \right)$$

- $s$ và $a$ là các hằng số thực nghiệm mô tả mức độ nứt nẻ và độ cài răng lược của khối đá:

$$s = \exp \left( \frac{\text{GSI} - 100}{9 - 3D} \right)$$

$$a = \frac{1}{2} + \frac{1}{6} \left( e^{-\text{GSI}/15} - e^{-20/3} \right)$$

- $D$ là **hệ số tổn thương do nổ mìn** ($0,0 \le D \le 1,0$) phản ánh mức độ vi nứt nẻ do chấn động sóng nổ và giải phóng ứng suất trong quá trình đào bới.

---

## 4.2 Hệ Thống Chỉ Số Cường Độ Địa Chất (GSI)

Chỉ số Cường độ Địa chất (GSI - Geological Strength Index) được phát triển nhằm thay thế các hệ thống phân loại định lượng cổ điển (RMR, Q) vốn bộc lộ nhiều sai số khi áp dụng cho các khối đá rất yếu ($RMR < 25$). GSI dựa trên hai quan sát địa chất trực quan tại hiện trường:

1. **Cấu trúc Khối đá (Mức độ Cài răng lược Vĩ mô)**:
   - *Liền khối (Intact / Massive)*: Rất ít khe nứt, khoảng cách khe nứt rất lớn.
   - *Dạng khối (Blocky)*: Các khối đá dạng hộp lập phương cài chặt vào nhau tạo bởi 3 hệ khe nứt trực giao.
   - *Rất nhiều khối (Very blocky)*: Có từ 4 hệ khe nứt trở lên tạo thành các khối đá góc cạnh đa diện.
   - *Bị xáo động / Nếp uốn (Disturbed / Folded)*: Khối đá bị vò xát, uốn nếp hoặc trượt đứt gãy.
   - *Bị vỡ vụn (Disintegrated)*: Khối đá bị dập vỡ hoàn toàn thành các mảnh vụn kích thước sỏi sạn.
2. **Chất lượng Bề mặt Khe Nứt (Tình trạng Thành vách Khe nứt)**:
   - Đánh giá từ *Rất tốt* (mặt nhám, đá tươi không phong hóa) đến *Rất kém* (mặt trơn nhẵn có vết cào xước, có lớp sét mềm lấp nhét).

```
+-----------------------------------------------------------------------------------------+
|                          CHỈ SỐ CƯỜNG ĐỘ ĐỊA CHẤT (GSI)                                 |
+---------------------+-------------------+---------------------+-------------------------+
| CẤU TRÚC KHỐI ĐÁ    | Mặt vách Rất tốt  | Mặt vách Trung bình | Mặt vách Kém / Chứa sét |
+---------------------+-------------------+---------------------+-------------------------+
| DẠNG KHỐI           |   GSI = 60 - 80   |    GSI = 50 - 65    |      GSI = 35 - 50      |
| RẤT NHIỀU KHỐI      |   GSI = 50 - 65   |    GSI = 40 - 55    |      GSI = 25 - 40      |
| XÁO ĐỘNG / PHÂN LỚP |   GSI = 35 - 50   |    GSI = 25 - 40    |      GSI = 15 - 30      |
| VỠ VỤN HOÀN TOÀN    |   GSI = 20 - 35   |    GSI = 15 - 25    |      GSI < 15           |
+---------------------+-------------------+---------------------+-------------------------+
```

---

## 4.3 Các Thông Số Mohr-Coulomb Tương Đương ($c', \phi'$)

Do phần lớn các phần mềm tính toán địa kỹ thuật (FLAC, PLAXIS, RS2) sử dụng tiêu chuẩn Mohr-Coulomb, nhóm tác giả Hoek đã dẫn xuất công thức xác định lực dính kết ($c'$) và góc ma sát trong ($\phi'$) tương đương bằng cách tiếp xúc đường thẳng tuyến tính với đường cong phi tuyến Hoek-Brown trong dải ứng suất giới hạn $\sigma_{3,\max}'$:

$$\phi' = \arcsin \left[ \frac{6 a m_b (s + m_b \sigma_{3n}')^{a-1}}{2(1 + a)(2 + a) + 6 a m_b (s + m_b \sigma_{3n}')^{a-1}} \right]$$

$$c' = \frac{\sigma_{ci} \left[ (1 + 2a)s + (1 - a)m_b \sigma_{3n}' \right] (s + m_b \sigma_{3n}')^{a-1}}{(1 + a)(2 + a) \sqrt{1 + \left( 6 a m_b (s + m_b \sigma_{3n}')^{a-1} \right) / \left( (1 + a)(2 + a) \right)}}$$

---

## 4.4 Mô Đun Biến Dạng của Khối Đá ($E_{rm}$)

Xác định mô đun biến dạng của khối đá là yêu cầu bắt buộc để tính toán độ co hẹp hội tụ của thành vách hầm và độ lún của móng công trình ngầm. Phương trình thực nghiệm Hoek-Diederichs (2006) có dạng:

$$E_{rm} = E_i \left( 0,02 + \frac{1 - D/2}{1 + e^{(60 + 15D - \text{GSI})/11}} \right)$$

Trong đó $E_i$ là mô đun Young của đá nguyên vẹn ($\text{MPa}$). Nếu không có thí nghiệm nén đo biến dạng trong phòng, có thể ước tính thông qua Tỷ số Mô đun ($MR$): $E_i = MR \cdot \sigma_{ci}$.

---

## 4.5 Thuật ngữ Đối chiếu Chuẩn hóa

| Thuật ngữ Tiếng Anh | Thuật ngữ Tiếng Việt Chuẩn hóa | Định nghĩa Kỹ thuật |
|---------------------|--------------------------------|----------------------|
| Geological Strength Index (GSI) | Chỉ số Cường độ Địa chất (GSI) | Chỉ số (10–100) đánh giá cấu trúc khối đá và tình trạng mặt nứt |
| Disturbance factor $D$ | Hệ số tổn thương do nổ mìn $D$ | Hệ số (0–1) làm suy giảm độ bền khối đá do chấn động nổ mìn |
| Equivalent continuum | Môi trường tựa liên tục tương đương | Mô hình môi trường liên tục đại diện cho khối đá nứt nẻ nhiều hệ |
| Deformation modulus | Mô đun biến dạng khối đá | Mô đun đàn hồi phản ánh tổng biến dạng đàn hồi và dẻo của khối đá |
