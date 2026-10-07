---
lang: vi
lang_alt: reference-manuals/practical-rock-engineering/chapter-05-in-situ-stresses/
---

# Chương 5 — Ứng Suất Nguyên Sinh & Ứng Suất Kích Ứng Quanh Công Trình Ngầm

## 5.1 Trường Ứng Suất Nguyên Sinh Dưới Lòng Đất

Trước khi bất kỳ một lỗ khoan hay đường hầm nào được đào bới, khối đá nằm sâu trong lòng đất đã tồn tại ở một trạng thái cân bằng tự nhiên được gọi là **trường ứng suất nguyên sinh (virgin / in-situ stress field)**.

### Ứng Suất Thẳng Đứng ($\sigma_v$)
Ứng suất thẳng đứng phát sinh do trọng lượng bản thân của toàn bộ cột đá nằm phía trên (chiều sâu tầng phủ $z$, dung trọng trung bình của đá $\gamma \approx 0,027\text{ MN/m}^3$):

$$\sigma_v = \int_0^z \gamma(z)\, dz \approx \gamma z \approx 0,027 z \quad (\text{MPa với } z \text{ tính bằng mét})$$

### Tỷ Số Ứng Suất Ngang ($k_0$)
Do tác động của các chuyển động kiến tạo mảng thạch quyển, co ngót nhiệt và lịch sử bóc mòn địa chất, các ứng suất chính nằm ngang ($\sigma_h, \sigma_H$) sai lệch rất lớn so với giả định thủy tĩnh:

$$k_0 = \frac{\sigma_h}{\sigma_v}$$

Dựa trên hàng ngàn dữ liệu đo đạc thực địa toàn cầu được tổng hợp bởi Hoek và Brown, ở độ sâu nông ($< 500\text{ m}$), $k_0$ thường xuyên vượt quá $1,5$ đến $3,5$ do ứng suất kiến tạo còn tồn lưu:

$$\frac{100}{z} + 0,3 \le k_0 \le \frac{1500}{z} + 0,5$$

---

## 5.2 Lời Giải Giải Tích Kirsch Cho Hầm Tiết Diện Tròn

Khi đào một lỗ rỗng ngầm, lực kéo mặt biên bên trong bị triệt tiêu về 0, buộc các đường truyền ứng suất phải uốn cong đi vòng qua biên lỗ khoét. Đối với hầm tròn bán kính $a$ trong môi trường đàn hồi đồng nhất chịu ứng suất đứng $p$ và ứng suất ngang $k p$:

### Ứng Suất Tiếp Vòng Biên ($\sigma_\theta$)

$$\sigma_\theta = \frac{p}{2} \left[ (1 + k)\left(1 + \frac{a^2}{r^2}\right) - (1 - k)\left(1 + 3\frac{a^4}{r^4}\right)\cos 2\theta \right]$$

### Ứng Suất Pháp Hướng Tâm ($\sigma_r$)

$$\sigma_r = \frac{p}{2} \left[ (1 + k)\left(1 - \frac{a^2}{r^2}\right) + (1 - k)\left(1 - 4\frac{a^2}{r^2} + 3\frac{a^4}{r^4}\right)\cos 2\theta \right]$$

### Tại Ngay Biên Thành Vách Hầm ($r = a$):
- Ứng suất hướng tâm bằng không: $\sigma_r = 0$.
- Đỉnh vòm / Đáy hầm ($\theta = \pi/2$): $\sigma_{\theta,\text{đỉnh}} = p (3k - 1)$.
- Hai bên hông lò ($\theta = 0$): $\sigma_{\theta,\text{hông}} = p (3 - k)$.

```
Trường hợp A: Trạng thái thủy tĩnh (k = 1,0)
Ứng suất tiếp biên hầm: sigma_theta = 2p ở mọi điểm (tập trung gấp 2 lần).

Trường hợp B: Ứng suất ngang kiến tạo rất cao (k = 2,0)
Ứng suất đỉnh vòm: sigma_theta = p(3(2) - 1) = 5p  (Nén ép rất mạnh gây nổ đá, tróc vỡ).
Ứng suất hai bên hông: sigma_theta = p(3 - 2) = 1p.

Trường hợp C: Ứng suất ngang nhỏ (k = 0,25)
Ứng suất đỉnh vòm: sigma_theta = p(3(0,25) - 1) = -0,25p (Xuất hiện vùng kéo -> nêm đá rơi tự do).
Ứng suất hai bên hông: sigma_theta = p(3 - 0,25) = 2,75p.
```

---

## 5.3 Sự Tập Trung Ứng Suất & Các Dạng Phá Hoại Quanh Buồng Ngầm

Khi ứng suất tiếp vòng biên $\sigma_\theta$ vượt quá cường độ kháng nén của khối đá ($\sigma_{cm}$):
1. **Bong tróc Giòn (Spalling / Slabbing)**: Các phiến đá mỏng sắc nhọn bị tách rời song song với biên hang đào trong các khối đá cứng liền khối ($UCS > 100\text{ MPa}$).
2. **Hình thành Vùng Dẻo (Plastic Yielding Zone)**: Một vành khăn dẻo bán kính $r_p > a$ phát triển xung quanh biên hầm, đẩy đỉnh ứng suất tập trung lùi sâu vào bên trong khối đá nguyên.
3. **Giải phóng Ứng suất Gây Kéo**: Tại các vùng xuất hiện ứng suất kéo ở đỉnh nóc hầm, ma sát trên các mặt khe nứt bị triệt tiêu hoàn toàn ($\sigma_n' \le 0$), khiến các khối nêm đá rơi tự do dưới tác dụng của trọng lực nếu không được chống giữ kịp thời bằng neo đá.

---

## 5.4 Các Phương Pháp Đo Đạc Ứng Suất Hiện Trường

| Phương Pháp | Nguyên Lý Hoạt Động | Chiều Sâu Ứng Dụng |
|-------------|---------------------|-------------------|
| **Khoan chụp đo biến dạng giải phóng (Overcoring - CSIRO HI Cell)** | Đo các biến dạng đàn hồi hồi phục khi một lỗ khoan dẫn đường được khoan chụp tách rời bởi ống khoan kim cương lớn hơn | Khoảng cách $30 - 50\text{ m}$ từ gương đào |
| **Thủy lực nứt nẻ (Hydraulic Fracturing)** | Dùng nút cao su cô lập một đoạn lỗ khoan sâu, bơm nước áp lực cao đến khi thành vách bị nứt vuông góc với $\sigma_3$ | Từ mặt đất xuống độ sâu $> 1.000\text{ m}$ |
| **Phân tích Vỡ mép Lỗ khoan (Borehole Breakouts)** | Dùng đầu đo siêu âm televiewer phát hiện các vùng bong tróc mép lỗ khoan định hướng theo phương ứng suất ngang nhỏ nhất | Các lỗ khoan thăm dò sâu |

---

## 5.5 Thuật ngữ Đối chiếu Chuẩn hóa

| Thuật ngữ Tiếng Anh | Thuật ngữ Tiếng Việt Chuẩn hóa | Định nghĩa Kỹ thuật |
|---------------------|--------------------------------|----------------------|
| In-situ stress / Virgin stress | Ứng suất nguyên sinh | Trường ứng suất tự nhiên tồn tại trước khi đào công trình |
| Induced stress | Ứng suất kích ứng | Trường ứng suất bị phân bố lại xung quanh không gian ngầm |
| Kirsch solution | Lời giải Kirsch | Hệ phương trình giải tích đàn hồi tính ứng suất quanh lỗ tròn |
| Tangential stress / Hoop stress | Ứng suất tiếp vòng biên | Ứng suất tác dụng tiếp tuyến với chu vi biên hang đào |
| Overcoring | Khoan chụp đo biến dạng giải phóng | Kỹ thuật đo ứng suất bằng cách khoan bao ngoài để giải phóng biến dạng |
