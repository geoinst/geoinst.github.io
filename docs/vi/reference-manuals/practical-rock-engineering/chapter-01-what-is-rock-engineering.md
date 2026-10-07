---
lang: vi
lang_alt: reference-manuals/practical-rock-engineering/chapter-01-what-is-rock-engineering/
---

# Chương 1 — Nhập môn Kỹ thuật Cơ học Đá

## 1.1 Bối cảnh Lịch sử & Sự Phát triển của Bộ môn

Kỹ thuật cơ học đá chính thức hình thành như một phân ngành kỹ thuật độc lập vào giữa thế kỷ 20. Trước thời điểm này, hoạt động khai thác mỏ hầm lò và đào hầm giao thông chủ yếu được coi là những kỹ nghệ mang tính thực hành dựa trên kinh nghiệm truyền khẩu, trong khi các công trình đào bề mặt thì áp dụng máy móc các công thức của cơ học đất.

Hàng loạt thảm họa kinh hoàng xảy ra vào giữa thế kỷ 20 đã gióng lên hồi chuông cảnh tỉnh về sự nguy hiểm đến tính mạng khi đồng nhất khối đá nứt nẻ với môi trường đất đồng nhất:

1. **Thảm họa Vỡ đập vòm Malpasset (Pháp, 1959)**: Đập vòm bê tông mỏng Malpasset bị vỡ sụp hoàn toàn ngay trong lần tích nước đầu tiên, cướp đi sinh mạng của 423 người. Bản thân bê tông thân đập không hề bị phá hoại; nguyên nhân cốt tử là do một đới trượt phiến hóa chưa được khảo sát kỹ và các mặt phân phiến bất lợi bên dưới vai đập trái bị đẩy trồi dưới áp lực nước khe nứt của hồ chứa.
2. **Thảm họa Lở núi Vajont (Ý, 1963)**: Một khối đá vĩ đại thể tích 270 triệu $\text{m}^3$ bất ngờ tách rời dọc theo các lớp kẹp sét bên trong mặt lớp đá vôi, trượt thẳng xuống lòng hồ thủy điện với vận tốc lên tới 110 km/h. Sóng thần cao 250 m vượt qua đỉnh đập quét sạch các thung lũng hạ du, làm hơn 2.000 người thiệt mạng.
3. **Sụp đổ Mỏ than Coalbrook (Nam Phi, 1960)**: Thảm họa sụp đổ dây chuyền của hơn 4.000 trụ than trên diện tích 3 $\text{km}^2$ đã chôn vùi 437 thợ mỏ chỉ trong vài phút, minh chứng rằng việc tính toán kích thước trụ than thuần túy theo diện tích truyền tải mà bỏ qua điều kiện giam hãm sẽ dẫn đến sụp đổ dây chuyền thảm khốc.

Các bài học đắt giá này buộc giới kỹ sư xây dựng và khai mỏ phải thừa nhận một chân lý nền tảng: **Hành vi cơ học của một khối đá không được quyết định bởi cường độ của bản thân mẫu đá nguyên vẹn, mà bị chi phối áp đảo bởi hệ thống các mặt bất liên tục cấu trúc (khe nứt, đứt gãy, mặt lớp) phân cắt nó và áp lực chất lưu thủy lực tác động bên trong các khe hở đó.**

---

## 1.2 Đá Nguyên vẹn đối chiếu Khối đá

Bước chuyển biến tư duy then chốt do Tiến sĩ Evert Hoek đúc kết chính là sự phân biệt rạch ròi giữa:

- **Đá nguyên vẹn (Intact Rock / Rock Material)**: Phần vật liệu đá đồng chất nằm giữa các mặt bất liên tục cấu trúc, thường được lấy mẫu dưới dạng các thỏi lõi khoan hình trụ ($\approx 50\text{ mm}$ đường kính). Nó ứng xử như một chất rắn đàn hồi giòn liên tục mà cường độ chịu nén được quyết định bởi liên kết khoáng vật và các vi nứt tế vi.
- **Khối đá (Rock Mass)**: Môi trường cấu trúc tại hiện trường bao gồm tập hợp các khối đá nguyên vẹn bị chia cắt bởi mạng lưới các mặt bất liên tục giao cắt nhau (khe nứt, đứt gãy, thớ phân phiến, mặt lớp). Khối đá có bản chất **bất liên tục, dị hướng, không đồng nhất và phi đàn hồi**.

```
+--------------------------------------------------------------+
|                          KHỐI ĐÁ                             |
|                                                              |
|   +---------------+      / /      +---------------+          |
|   | Đá nguyên vẹn |     / /       | Đá nguyên vẹn |          |
|   |   (Khối con)  |    / / Khe    |   (Khối con)  |          |
|   +---------------+   / /  nứt    +---------------+          |
|          \ \         / /                 \ \                 |
|           \ \ Đứt   / /                   \ \ Mặt            |
|   +---------------+ gãy  / /      +---------------+ lớp      |
|   | Đá nguyên vẹn |     / /       | Đá nguyên vẹn |          |
|   |   (Khối con)  |    / /        |   (Khối con)  |          |
|   +---------------+   / /         +---------------+          |
+--------------------------------------------------------------+
```

---

## 1.3 Hiệu ứng Quy mô trong Cơ học Đá

Khi quy mô xem xét của bài toán kỹ thuật mở rộng từ các mẫu thí nghiệm nhỏ trong phòng thí nghiệm đến các tầng bờ moong khai thác hay các buồng ngầm gian máy khổng lồ, cường độ kháng nén và mô đun biến dạng đo được của môi trường đá suy giảm nghiêm trọng.

$$\text{Cường độ}_{\text{Khối đá}} \ll \text{Cường độ}_{\text{Mẫu đá nguyên vẹn trong phòng}}$$

- Ở quy mô $0,05\text{ m}$ (mẫu lõi khoan), cơ học vi nứt nẻ và liên kết tinh thể chi phối.
- Ở quy mô $1 - 5\text{ m}$ (chu vi đường hầm hoặc bờ tầng mỏ), các nêm đá đa diện có khả năng giải phóng động học quyết định sự mất ổn định.
- Ở quy mô $> 30\text{ m}$ (bờ dốc mỏ lộ thiên sâu hoặc buồng nghiền quặng ngầm), khối đá nứt nẻ chằng chịt ứng xử như một môi trường tựa liên tục tương đương tuân theo tiêu chuẩn bền phá hoại Hoek-Brown.

---

## 1.4 Phương pháp Quan trắc trong Kỹ thuật Đá

Bởi vì các lỗ khoan khảo sát trước thi công chỉ lấy mẫu được chưa tới $0,001\%$ thể tích thực của khối đá, việc nắm bắt tường minh $100\%$ địa chất dưới lòng đất là điều bất khả thi về mặt toán học. Do đó, kỹ thuật cơ học đá bắt buộc phải dựa vào **Phương pháp quan trắc (Observational Method)**:

1. Thiết lập phương án thiết kế ban đầu dựa trên mô hình địa chất và địa kỹ thuật khả dĩ nhất.
2. Đề ra các giả thuyết định lượng rõ ràng về ngưỡng chuyển vị cho phép.
3. Lắp đặt mạng lưới thiết bị quan trắc (áp kế, thiết bị đo biến dạng sâu, mốc đo hội tụ).
4. Đo đạc liên tục phản ứng của đất đá trong suốt quá trình đào hầm hoặc bóc tầng mở moong.
5. Triển khai kế hoạch ứng phó ngưỡng kích hoạt (TARP) đã chuẩn bị sẵn khi tốc độ biến dạng đo được vượt quá ngưỡng an toàn.

---

## 1.5 Thuật ngữ Đối chiếu Chuẩn hóa

| Thuật ngữ Tiếng Anh | Thuật ngữ Tiếng Việt Chuẩn hóa | Định nghĩa Kỹ thuật |
|---------------------|--------------------------------|----------------------|
| Intact rock | Đá nguyên vẹn | Vật liệu đá liền khối nằm giữa các mặt bất liên tục cấu trúc |
| Rock mass | Khối đá | Môi trường hiện trường gồm các khối đá nguyên vẹn và hệ thống khe nứt chia cắt |
| Discontinuity | Mặt bất liên tục | Thuật ngữ chung chỉ khe nứt, mặt lớp, đới dập vỡ và đứt gãy |
| Cleft water pressure | Áp lực nước khe nứt | Áp lực thủy tĩnh và thủy động lực học của chất lưu tác động trong khe hở khe nứt |
| Observational Method | Phương pháp quan trắc | Phương pháp thiết kế kết hợp thi công đồng hành với đo đạc hiện trường theo thời gian thực |
