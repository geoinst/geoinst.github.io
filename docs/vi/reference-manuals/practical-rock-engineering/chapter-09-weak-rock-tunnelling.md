---
lang: vi
lang_alt: reference-manuals/practical-rock-engineering/chapter-09-weak-rock-tunnelling/
---

# Chương 9 — Thi Công Hầm Trong Đá Yếu & Đất Đá Ép Lún

## 9.1 Cơ Học Đất Đá Ép Lún (Squeezing Ground)

Khi các đường hầm thi công ở độ sâu lớn xuyên qua các tầng đá yếu nứt nẻ hoặc biến chất (đá phiến sét, đá phyllite, đá phiến kết, hoặc đới dập vỡ đứt gãy chứa sét), ứng suất tiếp tuyến kích ứng quanh chu vi hầm ($\sigma_\theta$) vượt xa cường độ kháng nén của khối đá ($\sigma_{cm}$).

Trong điều kiện này, khối đá không bị phá hủy giòn thành từng mảnh sắc. Thay vào đó, nó trải qua quá trình **biến dạng dẻo ép lún theo thời gian (ductile squeezing)**—toàn bộ khối đá xung quanh thành vách bị biến dạng dẻo trồi ép vào khoảng không trong hầm, gây ra sự co hẹp thể tích nghiêm trọng ($> 5\% - 20\%$ đường kính hầm), làm oằn cong các vì chống thép và phá hủy nén nứt vỡ lớp vỏ bê tông cứng.

### Chỉ Số Ép Lún Của Hoek:
Hoek và Marinos (2000) đã thiết lập tương quan giữa tỷ số cường độ khối đá trên ứng suất tầng phủ nguyên sinh ($\sigma_{cm} / \gamma H$) với mức độ biến dạng co hẹp đường kính hầm dự báo ($\epsilon = \Delta D / D$):

$$\frac{\sigma_{cm}}{\gamma H} = \frac{\sigma_{ci} \cdot s^a}{\gamma H}$$

| Tỷ Số $\sigma_{cm} / \gamma H$ | Biến Dạng Hầm $\Delta D / D$ | Mức Độ Nghiêm Trọng & Tác Động Vận Hành |
|--------------------------------|------------------------------|-----------------------------------------|
| $> 1,0$ | $< 1\%$ | Rất ít vấn đề chống giữ; dùng neo đá và lưới thép tiêu chuẩn |
| $0,5 - 1,0$ | $1\% - 2,5\%$ | Ép lún nhẹ; vì thép nhẹ hoặc neo đá kết hợp bê tông phun |
| $0,3 - 0,5$ | $2,5\% - 5\%$ | Ép lún trung bình; vì chống nặng lắp đặt ngay sát gương đào |
| $0,15 - 0,3$ | $5\% - 10\%$ | Ép lún nặng; khung vòm thép trượt dẻo, thi công ô dù ống thép cọc vòm |
| $< 0,15$ | $> 10\%$ | Ép lún cực kỳ nghiêm trọng; sập gương lò, để khe co dãn trong bê tông phun |

---

## 9.2 Phương Pháp Đường Cong Phản Ứng Nền (Convergence-Confinement Method - CCM)

Phương pháp Đường cong Phản ứng Nền là khung lý thuyết giải tích chuẩn mực kết hợp tương tác giữa ba đường cong căn bản:

```
Áp Lực Chống Giữ Bên Trong pi
      ^
  p_0 |  \ Đường Cong Phản Ứng Nền (GRC)
      |    \
      |      \        Đường Đặc Tính Kết Cấu Chống Giữ (SCC)
 p_eq |------- \-----/
      |         \   /
      |          \ / (Điểm Cân Bằng: u_eq, p_eq)
      |           v
      +-------------------------> Chuyển Vị Hướng Tâm u_r
                 u_0  u_eq
```

1. **Đường Cong Phản Ứng Nền (Ground Reaction Curve - GRC)**: Biểu diễn sự suy giảm áp lực giam giữ bên trong $p_i$ cần thiết để duy trì cân bằng khi chuyển vị hướng tâm thành vách $u_r$ tăng dần từ trạng thái ban đầu ($p_i = p_0, u_r = 0$) đến trạng thái không chống giữ ($p_i = 0, u_r = u_{\max}$).
2. **Biểu Đồ Biến Dạng Theo Trục Dọc (Longitudinal Deformation Profile - LDP)**: Thể hiện độ dịch chuyển thành hầm $u_r(x)$ theo khoảng cách đến gương đào $x$. Khoảng $25 - 35\%$ tổng chuyển vị đã phát sinh *trước* khi gương đào tiến tới vị trí lắp đặt vì chống.
3. **Đường Đặc Tính Vì Chống (Support Characteristic Curve - SCC)**: Phản ánh quan hệ tải trọng - biến dạng đàn dẻo của hệ kết cấu chống giữ (neo đá, bê tông phun, khung chống thép). Hệ vì chống phải được lắp đặt tại thời điểm độ co hẹp ban đầu $u_0$ tương ứng với khoảng cách bước đào.

---

## 9.3 Triết Lý Kết Cấu Chống Giữ Cứng Đối Chiếu Kết Cấu Chống Giữ Dẻo

Cố gắng ngăn chặn hiện tượng đất đá ép lún nặng bằng các kết cấu vỏ hầm siêu cứng, tuyệt đối không biến dạng là điều bất khả thi; áp lực ép khổng lồ của tầng đá nguyên ($p_0 = \gamma H$) sẽ nghiền nát bất kỳ kết cấu bê tông dày nào.

### Chiến Lược Chống Giữ Dẻo Hiện Đại:
1. **Các Khớp Trượt Nối Dẻo Hấp Thu Năng Lượng**: Sử dụng các vì vòm thép có khớp nối ma sát trượt (vì thép TH) hoặc ống thép biến dạng dẻo (hộp trụ LSC) cho phép khung chống co lại một cách có kiểm soát dưới lực cản định trước ($200 - 400\text{ kN}$).
2. **Xẻ Khe Co Dãn Dọc Trên Vỏ Bê Tông Phun**: Để lại các khe hở dọc theo phương trục hầm trên lớp bê tông phun, cho phép chu vi đường hầm co hẹp tự nhiên mà không làm vỡ nát bê tông phun do nén cục bộ. Khi biến dạng hầm đã tiệm cận ổn định, các khe này mới được phun bù bê tông bịt kín.
3. **Neo Đá Chịu Biến Dạng Lớn (Swellex, D-Bolt)**: Cho phép dãn dài $15 - 20\%$ mà không bị đứt gãy, duy trì liên tục áp lực nén giam hãm lên vành khăn đá dẻo đã nứt nẻ quanh hầm.

---

## 9.4 Thuật ngữ Đối chiếu Chuẩn hóa

| Thuật ngữ Tiếng Anh | Thuật ngữ Tiếng Việt Chuẩn hóa | Định nghĩa Kỹ thuật |
|---------------------|--------------------------------|----------------------|
| Squeezing ground | Đất đá ép lún | Hiện tượng đá bị biến dạng dẻo trồi ép vào trong hầm theo thời gian |
| Convergence-Confinement Method (CCM) | Phương pháp đường cong phản ứng nền (CCM) | Khung giải tích cân bằng giữa sự hội tụ đất đá và phản lực vì chống |
| Ground Reaction Curve (GRC) | Đường cong phản ứng nền (GRC) | Quan hệ giữa áp lực chống giữ bên trong và chuyển vị hướng tâm thành hầm |
| Longitudinal Deformation Profile (LDP) | Biểu đồ biến dạng theo trục dọc hầm (LDP) | Chuyển vị thành hầm biểu diễn theo khoảng cách tới gương đào |
| Yielding support | Kết cấu chống giữ dẻo hấp thu biến dạng | Hệ vì chống dẻo được thiết kế để co biến dạng dẻo mà không bị phá hoại |
