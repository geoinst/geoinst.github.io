---
lang: vi
lang_alt: reference-manuals/practical-rock-engineering/chapter-12-blasting-damage-controlled-excavation/
---

# Chương 12 — Tổn Thương Do Nổ Mìn & Kỹ Thuật Đào Kiểm Soát

## 12.1 Vật Lý Quá Trình Phá Hủy Đá Do Sóng Nổ

Nổ mìn phá vỡ đất đá thông qua hai cơ chế vật lý liên hoàn nối tiếp nhau:

1. **Sóng Xung Kích Vận Tốc Cực Cao**: Một xung nén tức thời truyền ra từ tâm lỗ mìn với tốc độ siêu thanh ($V_p \approx 3.000 - 6.000\text{ m/s}$). Khi sóng nén này phản xạ tại các mặt tự do biến thành sóng kéo, nó gây ra mạng lưới vi nứt nẻ tỏa tròn xung quanh thành lỗ khoan.
2. **Áp Suất Khí Nổ Giãn Nở**: Lượng khí nổ áp suất cực cao và nhiệt độ lớn ($P_{\text{khí nổ}} \approx 1.000 - 5.000\text{ MPa}$) chen lấn thâm nhập sâu vào các vết nứt do sóng xung kích tạo ra, tách banh các khe nứt và đẩy văng khối đá vỡ vụn về phía mặt thoáng tự do.

### Vùng Tổn Thương Do Nổ Mìn (Blast Damage Zone):
Trong nổ mìn khai thác thông thường, việc nhồi thuốc quá mức sẽ làm khối đá phía sau biên thiết kế bị phá vỡ nghiêm trọng. Điều này hình thành một **đới tổn thương nứt nẻ do nổ mìn** (chiều sâu $0,5 - 2,0\text{ m}$ phía sau bờ tầng moong hoặc vòm nóc hầm) với các đặc trưng: khe nứt bị mở toác, các cầu đá nguyên vẹn bị bẻ gãy, và góc ma sát bị phá hủy ($D \to 1,0$ trong tiêu chuẩn Hoek-Brown), dẫn đến các vụ đá rơi sập nguy hiểm.

---

## 12.2 Các Phương Pháp Nổ Mìn Kiểm Soát Biên

Để bảo vệ độ toàn vẹn và khả năng chịu lực tự nhiên của các vách moong cuối cùng và chu vi vòm hầm, các công nghệ nổ mìn tạo biên được áp dụng nghiêm ngặt:

```
A. NỔ TÁCH TRƯỚC (Pre-Splitting - Mỏ lộ thiên)   B. NỔ TẠO BIÊN NHẴN (Smooth Blasting - Hầm lò)
   [o] [o] [o] [o] [o]  (Lỗ đệm không nạp thuốc)     [X]  [X]  (Các lỗ phá nổ trước)
    |   |   |   |   |                                 \   /
   =================== (Mặt nứt cắt tách trước)      [o]-[o]-[o] (Hàng lỗ biên nổ SAU CÙNG)
   Kích nổ TRƯỚC các lỗ phá chính                    Thuốc nổ nhẹ cắt phẳng biên hầm
```

| Phương Pháp | Bố Trí Lỗ Khoan | Quy Cách Nạp Thuốc | Trình Tự Khởi Nổ |
|-------------|-----------------|---------------------|-------------------|
| **Nổ Mìn Tách Trước (Pre-Splitting)** | Các lỗ khoan biên bố trí dày đặc ($s \approx 8 - 12 d_{\text{lỗ}}$) dọc theo tuyến biên thiết kế cuối cùng | Lượng nổ nhẹ, không tiếp xúc thành lỗ (khoảng đệm không khí hoặc dây nổ định lượng) | Kích nổ **đồng thời TRƯỚC** khi nổ bất kỳ lỗ mìn phá khai thác nào |
| **Nổ Mìn Tạo Biên Nhẵn (Smooth Blasting)** | Hàng lỗ biên khoan gần nhau ($s \approx 15 - 16 d_{\text{lỗ}}$) với tỷ số gờ cản trên khoảng cách $B/s \approx 1,2 - 1,5$ | Thỏi thuốc nổ nhỏ định lượng, có khoảng hở với thành lỗ | Kích nổ ở **vi sai CUỐI CÙNG** sau khi toàn bộ đất đá phần ruột bên trong đã được đào giải phóng mặt thoáng |
| **Nổ Mìn Tỉa Đệm (Cushion Blasting)** | Hàng lỗ tỉa khoan sát vách biên tầng | Nạp thuốc nhẹ có vật liệu chèn đệm giảm chấn | Nổ sau khi đã xúc dọn đống đá nổ phá chính để cắt tỉa các phần nhô gồ ghề |

---

## 12.3 Vận Tốc Dao Động Hạt Cực Đại (PPV) & Ngưỡng Tổn Hại

Các dao động sóng địa chấn lan truyền qua khối đá được định lượng bằng **Vận tốc dao động hạt cực đại (PPV - Peak Particle Velocity)** đo bằng máy đo địa chấn 3 thành phần (geophone):

### Quy Luật Khoảng Cách Tỷ Lệ Thực Nghiệm USBM:

$$\text{PPV} = K \left( \frac{R}{\sqrt{Q}} \right)^{-B}$$

Trong đó $R$ là khoảng cách từ điểm đo đến tâm bãi nổ ($\text{m}$), $Q$ là lượng thuốc nổ nổ đồng thời lớn nhất trong một kíp vi sai ($\text{kg}$), và $K, B$ là các hằng số truyền sóng đặc thù của hiện trường.

### Tiêu Chuẩn Ngưỡng Tổn Thương Khối Đá:
- **$\text{PPV} < 50\text{ mm/s}$**: Rủi ro không đáng kể đối với đá tươi; mức an toàn tuyệt đối cho vỏ hầm bê tông và các công trình xây dựng lân cận.
- **$\text{PPV} \approx 100 - 250\text{ mm/s}$**: Bắt đầu xuất hiện hiện tượng mở rộng nhẹ các khe nứt và rơi rụng các khối đá lỏng lẻo ở nóc chưa chống giữ.
- **$\text{PPV} \approx 400 - 700\text{ mm/s}$**: Ngưỡng tới hạn gây tổn thương vĩnh viễn; xuất hiện các vi nứt kéo mới xuyên qua các cầu đá nguyên vẹn.
- **$\text{PPV} > 1.000\text{ mm/s}$**: Khối đá bị dập vỡ vụn nát hoàn toàn; tương đương với vùng nghiền nát quanh lỗ mìn.

---

## 12.4 Mạng Lưới Quan Trắc Chấn Động Nổ Mìn

Để bảo vệ an toàn cho các bờ moong mỏ và các buồng ngầm quan trọng xung quanh:
- Lắp đặt các đầu đo vi chấn geophone 3 trục tại đỉnh các cơ tầng mỏ lộ thiên để bảo đảm nổ mìn tạo biên không vượt quá ngưỡng $\text{PPV} \le 150\text{ mm/s}$.
- Kết nối các máy ghi chấn động với cổng truyền dữ liệu số ADAQS để tự động lập báo cáo tuân thủ an toàn sau mỗi ca nổ mìn và tối ưu hóa bước thời gian kíp nổ vi sai điện tử (chính xác đến từng mili giây).

---

## 12.5 Thuật ngữ Đối chiếu Chuẩn hóa

| Thuật ngữ Tiếng Anh | Thuật ngữ Tiếng Việt Chuẩn hóa | Định nghĩa Kỹ thuật |
|---------------------|--------------------------------|----------------------|
| Pre-splitting | Nổ mìn tạo khe trước / Nổ tách trước | Kích nổ đồng thời các lỗ biên trước khi nổ bãi phá để tạo mặt nứt phẳng bảo vệ vách |
| Smooth blasting | Nổ mìn tạo biên nhẵn | Phương pháp nổ hàng lỗ biên ở vi sai cuối cùng để tạo thành vách hầm phẳng nhẵn |
| Decoupled charge | Lượng thuốc nổ không tiếp xúc thành lỗ | Lượng nổ có đường kính nhỏ hơn đường kính lỗ khoan tạo đệm khí giảm chấn |
| Peak Particle Velocity (PPV) | Vận tốc dao động hạt cực đại (PPV) | Vận tốc dao động lớn nhất của hạt đất đá khi sóng địa chấn nổ mìn truyền qua |
| Scaled distance | Khoảng cách tỷ lệ | Tỷ số hình học liên kết khoảng cách với căn bậc hai lượng thuốc nổ một vi sai |
