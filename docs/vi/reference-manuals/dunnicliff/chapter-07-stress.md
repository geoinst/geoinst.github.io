---
lang: vi
lang_alt: reference-manuals/dunnicliff/chapter-07-stress/
---

# Chương 7 — Đo ứng suất trong đất và đá

## 7.1 Hai bài toán ứng suất riêng biệt

Quan trắc ứng suất trong công trình địa kỹ thuật được phân thành hai nhóm nhiệm vụ cơ bản với các đặc tính cơ học và thiết bị hoàn toàn khác nhau:

1. **Ứng suất toàn phần trong đất (Total Stress in Soil)**: Áp lực do khối đất hoặc tải trọng công trình tác dụng lên một mặt phẳng (áp lực đất chủ động lên tường vây, áp lực tiếp xúc dưới đáy móng bè, ứng suất pháp bên trong khối đắp đập).
2. **Biến thiên ứng suất trong khối đá (Stress Change in Rock)**: Sự tái phân bố trường ứng suất tự nhiên trong khối đá nứt nẻ do hoạt động đào hầm, nổ mìn hoặc gia tải kết cấu.

## 7.2 Tế bào đo áp lực đất (Earth Pressure Cells - EPC)

### Cấu tạo và nguyên lý
Tế bào đo áp lực đất gồm hai đĩa thép không gỉ mỏng hàn mép kín, kẹp giữa một màng chất lỏng thủy lực truyền áp cực mỏng, nối liền với một cảm biến áp suất dây rung hoặc khí nén.

### Hai dạng lắp đặt chính
- **Tế bào tiếp xúc ranh giới (Boundary / Contact Cells)**: Mặt sau là tấm thép dày phẳng cứng, mặt trước mỏng linh hoạt. Được gắn phẳng mặt với bề mặt bê tông của tường vây, mố cầu hoặc đáy đài móng để đo áp lực đất trực tiếp tác dụng lên kết cấu.
- **Tế bào chôn trong khối đất (Embedment Cells)**: Hai mặt đối xứng linh hoạt mỏng, được chôn chìm trực tiếp vào khối đắp đập hoặc nền đất đắp để đo ứng suất pháp theo phương đứng hoặc ngang.

## 7.3 Hệ số tác động của tế bào (Cell Action Factor - CAF)

Do độ cứng của bản thân tế bào bằng thép khác biệt so với độ cứng của khối đất xung quanh, đường truyền ứng suất sẽ bị hội tụ hoặc phân tán cục bộ:

$$\text{CAF} = \frac{\sigma_{\text{đo được}}}{\sigma_{\text{thực tế của đất}}}$$

Nếu tế bào quá cứng, $\text{CAF} > 1.0$ (tập trung ứng suất giả tạo, số đo bị vọt cao). Nếu tế bào quá mềm, $\text{CAF} < 1.0$ (phân tán ứng suất, số đo bị thấp).

### Yêu cầu thiết kế của Dunnicliff để $\text{CAF} \approx 1.0$:
- **Tỷ số kích thước (Aspect ratio)**: Tỷ số giữa độ dày tế bào ($B$) và đường kính ($D$) phải nhỏ hơn $1/10$ (tốt nhất là $B/D \le 1/12$).
- **Đường kính tế bào đủ lớn**: Đường kính tối thiểu phải gấp ít nhất 10–20 lần kích thước hạt đất lớn nhất tiếp xúc.
- **Kỹ thuật đầm nén**: Đất đắp xung quanh tế bào phải được sàng loại bỏ đá cuội sắc nhọn và đầm nén thủ công cẩn trọng để đạt khối lượng thể tích đồng nhất với khối đắp xung quanh.

## 7.4 Đo thay đổi ứng suất trong khối đá

Khối đá nứt nẻ và công trình ngầm đòi hỏi các phương pháp đo ứng suất đặc thù:

- **Tế bào đo áp lực hố khoan (Borehole Pressure Cells - BPC)**: Thiết bị gồm tế bào phẳng chèn chặt vào hố khoan bằng nêm cơ học hoặc vữa trương nở, theo dõi sự gia tăng áp lực khi khối đá xung quanh chịu tải.
- **Phương pháp kích phẳng (Flat Jacks)**: Cắt một khe hẹp trên vách đá hầm để giải phóng ứng suất (hai mốc biến dạng co lại), sau đó chèn kích phẳng thủy lực và bơm dầu cho đến khi hai mốc dãn về vị trí ban đầu. Áp lực dầu lúc này tương đương với ứng suất ban đầu của vách đá.
- **Phương pháp khoan giải ứng suất (Overcoring Technique)**: Dán đầu đo biến dạng đa trục (USBM gauge hoặc CSIR/CSIRO hollow inclusion cell) vào đáy một hố khoan nhỏ, sau đó dùng mũi khoan lấy lõi đường kính lớn hơn khoan bao xung quanh để giải phóng hoàn toàn khối đá lõi khỏi trường ứng suất. Dựa trên biến dạng đàn hồi hồi phục, kỹ sư tính toán ngược lại tenxơ ứng suất nguyên sinh 3D của khối đá.

![Figure: dunnicliff-earth-pressure-cell](../../../assets/figures/dunnicliff-earth-pressure-cell.svg)

**Hình.** Tế bào áp lực đất. Tế bào ứng suất tiếp xúc đo áp lực lên kết cấu; tế bào ứng suất toàn phần được chôn trong đất đắp. Cần khớp độ cứng tế bào với nền đất (Dunnicliff, Ch. 10).

## 7.5 Các điểm then chốt cần ghi nhớ

- Đo ứng suất đất khó hơn đo biến dạng hay đo áp lực nước vì sự bất đồng nhất của độ cứng vật liệu.
- Thiết kế tế bào áp lực đất phải đảm bảo tỷ số độ dày / đường kính $B/D \le 1/10$ để đạt $\text{CAF} \approx 1.0$.
- Cẩn trọng tuyệt đối khi đầm nén đất xung quanh tế bào để tránh tập trung ứng suất giả tạo.
- Trong khối đá, phương pháp kích phẳng và khoan giải ứng suất (overcoring) là công cụ chủ lực để xác định trường ứng suất nguyên sinh.
