---
lang: vi
lang_alt: reference-manuals/practical-rock-engineering/chapter-03-discontinuity-shear-strength/
---

# Chương 3 — Sức Kháng Cắt của Mặt Bất Liên Tục

## 3.1 Cơ học Cắt Trượt Dọc theo Bề mặt Khe Nứt

Trong các khối đá có các hệ khe nứt phát triển liên tục, các phá hoại mất ổn định kết cấu (trượt bờ tầng mỏ, sập nêm vòm hầm, lật đổ cột đá) diễn ra chủ yếu bằng cách trượt dọc theo các mặt bất liên tục có sẵn chứ không phải do cắt phá vỡ xuyên qua bản thân đá nguyên vẹn.

Sức kháng cắt ($\tau$) dọc theo một mặt khe nứt hở không có lực dính kết keo được kiểm soát bởi ba yếu tố cốt lõi:
1. **Ứng suất Pháp Hữu hiệu ($\sigma_n'$)**: Ứng suất nén ép chặt hai bờ vách khe nứt lại với nhau.
2. **Góc Ma sát Cơ bản ($\phi_b$)**: Góc ma sát giữa các hạt khoáng đo trên bề mặt đá cưa phẳng nhẵn lý tưởng của cùng loại đá đó (thường dao động từ $25^\circ - 35^\circ$).
3. **Độ Nhám Bề mặt & Hiện tượng Giãn nở Mấu nhám**: Các gờ lồi lõm mấp mô hình học (asperities) buộc hai thành vách khe nứt phải trồi cưỡng bức lên nhau (hiện tượng dãn nở thể tích cắt) khi dịch chuyển, hoặc cắt đứt xuyên qua mấu nhám khi áp lực pháp quá cao.

---

## 3.2 Mô hình Song Tuyến của Patton

Năm 1966, F.D. Patton đã chứng minh rằng các mấu nhám hình răng cưa đều đặn nghiêng một góc $i$ sẽ tạo ra một đường bao sức kháng cắt dạng song tuyến gãy khúc:

### Vùng Ứng suất Pháp Thấp ($\sigma_n' < \sigma_T$): Trượt Leo qua Mấu nhám
Dịch chuyển cắt buộc hai khối đá phải nâng trồi vuông góc vượt qua đỉnh các răng cưa nhám:

$$\tau = \sigma_n' \tan(\phi_b + i)$$

### Vùng Ứng suất Pháp Cao ($\sigma_n' \ge \sigma_T$): Cắt Đứt xuyên qua Chân Mấu nhám
Ứng suất pháp quá lớn triệt tiêu khả năng nâng trồi; toàn bộ các răng cưa mấu nhám bị cắt đứt ngang chân:

$$\tau = c_j + \sigma_n' \tan(\phi_r)$$

Trong đó $c_j$ là lực dính biểu kiến do lực kháng cắt của chân mấu nhám và $\phi_r$ là góc ma sát dư.

---

## 3.3 Tiêu chuẩn Kháng Cắt Phi Tuyến Barton-Bandis

Bởi vì các mặt khe nứt thực tế trong tự nhiên có độ nhám bất quy tắc đa quy mô chứ không phải hình răng cưa nhân tạo đều đặn, Nick Barton và S. Bandis (1976, 1982, 1990) đã xây dựng phương trình thực nghiệm phi tuyến kinh điển:

$$\tau = \sigma_n' \tan \left[ \text{JRC} \cdot \log_{10} \left( \frac{\text{JCS}}{\sigma_n'} \right) + \phi_b \right]$$

Trong đó:
- $\text{JRC}$ = Hệ số độ nhám khe nứt (Joint Roughness Coefficient), biến thiên từ $0$ (nhẵn bóng như gương) đến $20$ (rất gồ ghề, lượn sóng).
- $\text{JCS}$ = Cường độ nén thành vách khe nứt (Joint Wall Compressive Strength), đo đạc trực tiếp bằng búa nảy Schmidt trên bề mặt vách khe nứt tươi hoặc phong hóa.
- $\phi_b$ = Góc ma sát cơ bản của mặt đá phẳng không phong hóa.
- $\sigma_n'$ = Ứng suất pháp hữu hiệu tác dụng vuông góc lên mặt khe nứt.

### Hiệu chỉnh Quy mô cho Khe nứt Hiện trường
Thí nghiệm hộp cắt trong phòng ($L_0 = 100\text{ mm}$) luôn đánh giá độ nhám cao hơn so với các mặt đứt gãy khe nứt dài ở hiện trường ($L_n = 1 - 5\text{ m}$):

$$\text{JRC}_n = \text{JRC}_0 \left( \frac{L_n}{L_0} \right)^{-0,02 \text{JRC}_0}$$

$$\text{JCS}_n = \text{JCS}_0 \left( \frac{L_n}{L_0} \right)^{-0,03 \text{JRC}_0}$$

---

## 3.4 Khe Nứt Chứa Vật Liệu Lấp nhét & Sét Dập vỡ Đứt gãy

Khi quá trình phong hóa hoặc biến dạng trượt đứt gãy tạo ra một lớp vật liệu hạt mịn lấp nhét (sét dập vỡ, bột talc, clorit) giữa hai vách đá, sự cài răng lược của mấu nhám bị mất tác dụng.

- Nếu chiều dày lớp lấp nhét $t < \text{chiều cao mấu nhám } a$, sự tiếp xúc đá - đá vẫn tham gia đóng góp vào sức kháng cắt.
- Nếu chiều dày $t \ge 1,5 a$, sức kháng cắt tụt giảm hoàn toàn xuống bằng sức kháng cắt thoát nước hoặc không thoát nước của bản thân lớp sét lấp nhét ($\phi' \approx 8^\circ - 18^\circ$ đối với sét montmorillonite/smectite). Đây chính là cơ chế tạo nên các mặt trượt phá hoại lịch sử như tại sạt lở núi Vajont.

---

## 3.5 Thuật ngữ Đối chiếu Chuẩn hóa

| Thuật ngữ Tiếng Anh | Thuật ngữ Tiếng Việt Chuẩn hóa | Định nghĩa Kỹ thuật |
|---------------------|--------------------------------|----------------------|
| Discontinuity shear strength | Sức kháng cắt của mặt bất liên tục | Khả năng chống trượt dọc theo khe nứt, mặt lớp và đứt gãy |
| Basic friction angle $\phi_b$ | Góc ma sát cơ bản $\phi_b$ | Góc ma sát đo trên bề mặt cưa phẳng nhẵn lý tưởng |
| Asperity | Mấu nhám | Độ mấp mô hình học lồi lõm trên bề mặt vách khe nứt |
| Joint Roughness Coefficient (JRC) | Hệ số độ nhám khe nứt (JRC) | Chỉ số không thứ nguyên (0–20) định lượng độ gồ ghề của vách nứt |
| Joint Wall Compressive Strength (JCS) | Cường độ nén thành vách khe nứt (JCS) | Cường độ nén đơn trục của lớp đá bề mặt tạo nên thành vách khe nứt |
| Fault gouge | Sét dập vỡ đứt gãy / Vữa đứt gãy | Vật liệu sét mềm mịn, bị vò xát mạnh lấp đầy trong đới đứt gãy |
