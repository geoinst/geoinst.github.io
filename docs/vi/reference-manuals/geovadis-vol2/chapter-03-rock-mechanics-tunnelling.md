---
lang: vi
lang_alt: reference-manuals/geovadis-vol2/chapter-03-rock-mechanics-tunnelling/
---

# Cơ học Đá & Kỹ thuật Công trình Ngầm

!!! abstract "Tóm tắt Chuyên đề"
    Phiên 8 của *GeoVadis (GAIC 2025)* công bố những tiến bộ nổi bật trong phân loại khối đá, công nghệ thi công hầm cơ giới hóa bằng khiên đào (TBM), lưu trữ địa chất khí $\text{CO}_2$ và giảm thiểu rủi ro sạt lở đá lăn. Các báo cáo then chốt đi sâu vào kỹ thuật địa chấn dự báo trước gương hầm, mô phỏng 3D tương tác giữa các tuyến hầm lân cận, phân tích ngược tổn thất thể tích đất đào hầm và mạng lưới cảm biến IoT cảnh báo sớm nguy cơ đá lở.

---

## 1. Địa Vật Lý Sóng Địa Chấn Dự Báo Trước Gương Hào Hầm (S.C. Chian, Y.Z. Tan, Y.E. Li, C.H.A. Cheng)

### Ngăn Chặn Thảm Họa Địa Chất Trong Thi Công Ngầm
Việc đột ngột bắt gặp đới đứt gãy dập vỡ, hang ngầm karst hoặc túi nước áp lực cao trong quá trình đào hầm gây sập hầm nghiêm trọng và đình trệ dự án. Chian và cộng sự làm rõ hiệu quả của hệ thống **Dự báo Địa chấn Trong Hầm (Tunnel Seismic Prediction - TSP)**:
- **Nguyên lý lan truyền và phản xạ sóng:** Sóng địa chấn tần số cao phát ra từ các vụ nổ vi mô hoặc va đập cơ học bên thành hầm sẽ phản xạ ngược lại khi gặp các ranh giới bất tương xứng trở kháng âm học phía trước gương đào.
- **Phạm vi nhìn trước:** Dàn cảm biến gia tốc 3 trục gắn cố định trên vỏ hầm xử lý biểu đồ phân cực sóng P và sóng S, lập bản đồ chính xác các khe nứt kiến tạo và đới đứt gãy phía trước gương đào ở cự ly từ $100\,\text{m} - 150\,\text{m}$.
- **Quy trình an toàn:** Dữ liệu nghịch đảo thời gian thực giúp ban chỉ huy công trường kịp thời triển khai khoan thăm dò nòng dài và khoan phụt vữa gia cố trước gương hầm trước khi máy đào tiến vào vùng nguy hiểm.

```
       Mặt cắt Hầm & Sơ đồ Hình học Thăm dò Địa chấn Trước Gương
       ┌───────────────────────────────┐
       │ Đoạn hầm đã thi công xong    │
       │                               │
       │  Nguồn phát chấn động         │
       │    (Nổ mìn vi sai / Va đập)   │
       │          ●                    │   Sóng P & S phát tỏa về phía trước
       │          │ ╲                  │   ─────────►  ─────────►
       │          │   ╲                │
       │  Mảng đầu đo gia tốc          │
       │    gắn trên vỏ hầm            │
       │    ▲   ▲   ▲   ▲   ▲          │
       ├───────────────────────────────┤   ◄─── Gương đào hầm hiện tại
       │                               │
       │     Khối đá chưa đào          │        Đới đứt gãy / Túi nước ngầm
       │                               │        (Trở kháng âm học sụt giảm)
       │                               │             ║║║║║║║║║║
       │                               │   Sóng phản ║║║║║║║║║║
       │                               │   xạ dội lại ◄║║║║║║║║║
       └───────────────────────────────┘             ║║║║║║║║║║
```

---

## 2. Mô Phỏng Số 3D Khiên Đào TBM Trong Địa Tầng Phân Lớp (J. Agarwal, G. Garg, et al.)

### Thi Công Hầm Bằng Khiên Đào Cân Bằng Áp Lực Đất (EPB)
Sử dụng phần mềm MIDAS GTS-NX, Agarwal và các đồng tác giả mô phỏng chi tiết 3D tương tác liên tục giữa khiên đào EPB và địa tầng gồm các lớp cát và sét cứng xen kẹp:
- **Áp lực giữ gương đào:** Áp lực trong buồng đào được hiệu chỉnh để cân bằng với áp lực đất ngang tĩnh và áp lực nước lỗ rỗng tự nhiên ($p_{face} = K_0 \sigma'_v + u_w$), ngăn chặn hiện tượng đất gương đào chảy xẹp vào buồng máy gây sụt lún mặt đất.
- **Bơm vữa chèn khe hở đuôi khiên & Lực kích đẩy:** Mô hình tích hợp áp lực phụt vữa chèn khe hở đuôi khiên ($p_{grout} \approx 200 - 300\,\text{kPa}$), lực ma sát côn của vỏ khiên và lực kích đẩy của hệ xi lanh thủy lực lên các vòng vỏ hầm bê tông đúc sẵn.
- **Phễu lún sụt ngang bề mặt:** Phân bố lún sụt mặt đất tuân theo hàm phân phối Gauss của Peck:
  $$S(x) = S_{max} \cdot \exp\left( -\frac{x^2}{2 i^2} \right)$$
  trong đó độ rộng phễu lún $i = K \cdot z_0$ được tính toán chính xác phù hợp với địa tầng thực tế.

---

## 3. Ứng Xử Của Hầm Hiện Hữu Khi Đào Hầm Mới Liền Kề (J.Q. Lin, J.H. Zhang, X.S. Chen, et al.)

### Thi Công Hầm Gần Trong Đô Thị Mật Độ Cao
Việc thi công đường hầm mới chạy song hành hoặc giao cắt bên dưới các tuyến hầm metro đang khai thác gây hiện tượng giải phóng ứng suất bất đối xứng:
- **Biến dạng méo hình vỏ hầm:** Sự tái phân bố ứng suất đất đá làm các đốt hầm bê tông hiện hữu bị dẹt hình học (giãn rộng theo phương ngang và lún xẹp theo phương đứng).
- **Hở khớp nối đốt vỏ hầm & Kéo đứt bu-lông:** Biến dạng trượt tương đối giữa các vòng đốt gây hở khe nối chống thấm và làm tăng vọt ứng suất kéo trong các bu-lông liên kết hướng tâm.
- **Biện pháp khống chế:** Khoan phụt vữa gia cố trước khối đất trụ ngăn giữa hai hầm và kiểm soát chặt chẽ tốc độ đào giúp giới hạn độ dịch chuyển hội tụ của hầm hiện hữu trong ngưỡng an toàn đường sắt ($< 5\,\text{mm}$).

---

## 4. Tương Tác Thủy - Cơ Trong Bể Chứa Khí $\text{CO}_2$ Tầng Nước Mặn (S.M. Chiang, M.C. Weng, H.K. Le, et al.)

### Độ Toàn Vẹn Tầng Chắn & Tái Kích Hoạt Đứt Gãy
Bơm ép khí carbon dioxide siêu tới hạn ($\text{scCO}_2$) vào các tầng ngậm nước mặn sâu ($> 1.000\,\text{m}$) làm tăng áp suất lỗ rỗng trong vỉa, làm biến đổi trạng thái ứng suất địa chất:
- **Phân tích ghép thủy - cơ:** Nhóm tác giả xây dựng mô hình phần tử hữu hạn ghép hai pha chất lưu và biến dạng đàn dẻo của khối đá xốp.
- **Nguy cơ trượt đứt gãy:** Áp lực lỗ rỗng do quá trình bơm ép làm giảm ứng suất pháp hữu hiệu ($\sigma'_n$) tác dụng lên các mặt đứt gãy xung quanh, có nguy cơ gây động đất kích hoạt nếu áp suất bơm vượt ngưỡng:
  $$\tau \le c' + (\sigma_n - u_{pore})\tan\phi'$$
- **Đánh giá tầng đá chắn nắp (Caprock):** Nghiên cứu định lượng áp lực bơm tối đa cho phép để ứng suất kéo trong tầng đá chắn luôn nhỏ hơn cường độ kháng kéo của đá ($f_t$), đảm bảo khí $\text{CO}_2$ không bị rò rỉ lên tầng nước ngầm nông.

---

## 5. Mạng Lưới Cảm Biến IoT Cảnh Báo Sớm Đá Lăn & Lũ Bùn Đá (R. Budhbhatti, R.R. Mahajan, D. Paldino)

### Hệ Thống Cảnh Báo Sớm Ứng Dụng Điện Toán Biên
Các tuyến quốc lộ và đường sắt vùng núi Himalaya thường xuyên đối mặt với các vụ đá lăn bất ngờ và lũ bùn đá quét qua sườn dốc. Budhbhatti và cộng sự triển khai hệ thống quan trắc IoT hiện trường:
- **Bố trí nút cảm biến:** Các cảm biến đo độ nghiêng bề mặt MEMS và cảm biến đo tải trọng được gắn trực tiếp trên các hệ rào chắn đá lăn dạng lưới thép vòng dẻo có khả năng hấp thụ năng lượng va đập lớn ($E > 500\,\text{kJ}$).
- **Quy trình kích hoạt ứng phó tự động (TARP):** Cổng kết nối không dây LoRaWAN truyền dữ liệu đo liên tục lên máy chủ đám mây; khi lực căng cáp hoặc góc nghiêng cột vượt ngưỡng cảnh báo Cấp 3 (TARP), hệ thống tự động phát tín hiệu cảnh báo đèn hiệu đường sắt để dừng đoàn tàu từ xa.

---

## 6. Ma Trận Thiết Bị Quan Trắc Hiện Trường Cho Cơ Học Đá & Công Trình Ngầm

| Hạng mục Thi công Ngầm | Thiết bị Quan trắc Chủ đạo | Thiết bị Đo Đối chứng | Chỉ tiêu Kỹ thuật Giám sát |
| :--- | :--- | :--- | :--- |
| **Khiên đào TBM thi công hầm** | Mốc laser đo biến dạng hội tụ trong hầm | Thiết bị đo biến dạng sâu (Extensometer) | Độ méo vỏ hầm, phễu lún mặt đất $S(x)$ |
| **Thăm dò đứt gãy trước gương** | Mảng gia tốc kế 3 chiều gắn vỏ hầm | Khoan lấy lõi ngang nòng dài | Phổ sóng phản xạ P/S, cự ly đới đứt gãy |
| **Hầm hiện hữu lân cận hầm mới**| Cảm biến Sister Bar / Cảm biến biến dạng | Robot toàn đạc tự động quan trắc | Độ mở khớp nối đốt hầm, mô-men uốn vỏ |
| **Bơm ép $\text{CO}_2$ tầng ngậm nước**| Cảm biến áp suất thạch anh đáy giếng | Mảng quan trắc vi địa chấn bề mặt | Áp lực lỗ rỗng vỉa chứa, chấn động trượt đứt gãy |
| **Rào chắn đá lăn dạng lưới mềm**| Cảm biến đo độ nghiêng MEMS & Load cell | Thiết bị quét laser 3D LiDAR | Lực va đập đá lăn, mất lực căng cáp, trượt đá |
