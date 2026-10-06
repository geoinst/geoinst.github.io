---
lang: vi
lang_alt: reference-manuals/dunnicliff/chapter-06-piezometers/
---

# Chương 6 — Đo áp lực nước ngầm và áp lực nước lỗ rỗng

## 6.1 Vai trò quyết định của áp lực nước lỗ rỗng

Áp lực nước ngầm và áp lực nước lỗ rỗng ($u$) là thông số địa kỹ thuật được đo phổ biến nhất và mang tính quyết định nhất đối với sự ổn định của mọi công trình xây dựng. Theo nguyên lý ứng suất hữu hiệu Terzaghi ($\sigma' = \sigma - u$):
- Khi áp lực nước lỗ rỗng tăng cao (sau mưa lớn, dâng nước hồ chứa, hoặc do tải trọng đắp nhanh), ứng suất hữu hiệu $\sigma'$ giảm, kéo theo sức chống cắt của đất giảm sút nghiêm trọng, dẫn đến nguy cơ trượt lở mái dốc, bùng nền hố đào hoặc sạt trượt đập đất.
- Việc đo chính xác áp lực nước lỗ rỗng là cơ sở cốt lõi để kiểm soát tốc độ đắp phân tầng (staged construction), đánh giá hiệu quả hạ mực nước ngầm và theo dõi an toàn đập.

## 6.2 So sánh các loại Piezometer

| Loại Piezometer | Nguyên lý đo | Ưu điểm chính | Hạn chế / Phạm vi áp dụng |
|---|---|---|---|
| **Ống đứng hở (Casagrande)** | Nước dâng tự do trong ống PVC có đầu lọc xốp | Rất đơn giản, bền bỉ, chi phí thấp, kiểm tra được mực nước bằng đầu dò còi | Độ trễ thủy lực rất lớn; không dùng được cho đất sét ít thấm |
| **Piezometer thủy lực hai ống** | Màng thủy lực nối với 2 đường ống dẫn dầu/nước | Đo được áp lực nước âm cục bộ | Dễ bị tắc bọt khí, đòi hỏi buồng điều khiển bảo trì phức tạp |
| **Piezometer khí nén (Pneumatic)** | Khí nén uốn màng cao su cân bằng áp lực nước | Miễn nhiễm sét lan truyền, không có mạch điện ngầm | Chỉ đo thủ công từng điểm, tốc độ đo chậm |
| **Piezometer dây rung (VW)** | Màng kim loại uốn làm thay đổi tần số dây đàn hồi | **Tiêu chuẩn vàng**: Độ trễ thủy lực $\approx 0$, truyền xa không suy hao, kết nối ADAS | Cần bảo vệ chống sét, cần hiệu chỉnh nhiệt độ |

## 6.3 Độ trễ thủy lực (Hydrodynamic Time Lag)

Độ trễ thủy lực là khoảng thời gian cần thiết để một lượng nước nhất định chảy qua đầu lọc đi vào buồng đo của piezometer nhằm thiết lập trạng thái cân bằng áp lực với khối đất xung quanh.

- Với **ống đứng Casagrande**, để mực nước trong ống đường kính 19 mm dâng lên 1 m, cần một thể tích nước chảy vào khá lớn ($\Delta V \approx 280\text{ cm}^3$). Trong đất sét có hệ số thấm $k = 10^{-8}\text{ cm/s}$, thời gian để đạt 95% độ cân bằng có thể kéo dài **vài tuần đến vài tháng**!
- Với **piezometer dây rung**, màng ngăn kim loại cực cứng có biến dạng thể tích gần như bằng không ($\Delta V \approx 0.001\text{ cm}^3$). Thời gian đáp ứng cân bằng diễn ra **gần như tức thời (vài giây)**, cho phép ghi nhận chuẩn xác biến động áp lực nước lỗ rỗng thặng dư trong đất sét bão hòa.

## 6.4 Quy trình bão hòa đầu lọc (Filter Saturation)

Sự hiện diện của bọt khí bên trong buồng đo sẽ làm tăng thể tích nén đàn hồi của hệ thống và gây trễ kết quả nghiêm trọng:
- Đầu đá lọc xốp phải được ngâm trong nước sạch và khử bọt khí bằng cách **đun sôi tối thiểu 30 phút** hoặc rút chân không trong bình hút ẩm.
- Lắp ráp đầu lọc vào thân cảm biến dưới mặt nước để đảm bảo không có bọt khí nào bị giữ lại bên trong màng rung.

## 6.5 Phương pháp vữa chèn toàn phần (Fully Grouted Method)

Phương pháp lắp đặt truyền thống dùng túi cát lọc kết hợp nút đệm bentonite đòi hỏi kỹ thuật cao và dễ bị thông tầng rò rỉ nếu thi công không chuẩn. 

Dunnicliff đánh giá cao **Phương pháp bơm vữa chèn toàn phần (Fully Grouted Method)** do Mikkelsen và Green chuẩn hóa:
- Áp kế dây rung được treo trực tiếp vào độ sâu thiết kế trong hố khoan.
- Toàn bộ hố khoan từ đáy lên miệng hố được bơm chèn bằng hỗn hợp vữa xi măng - bentonite có độ thấm tương đương hoặc thấp hơn độ thấm của tầng đất ($k_{\text{vữa}} \le 10^{-6}\text{ cm/s}$).
- Do biến dạng thể tích của màng VW cực nhỏ, áp lực nước lỗ rỗng từ địa tầng sẽ truyền xuyên qua lớp vữa mỏng tác dụng trực tiếp lên màng đo mà không gây sai số áp lực, đồng thời triệt tiêu hoàn toàn nguy cơ rò rỉ nước giữa các tầng ngậm nước khác nhau.

## 6.6 Các điểm then chốt cần ghi nhớ

- Áp lực nước lỗ rỗng chi phối trực tiếp sức chống cắt của đất thông qua nguyên lý ứng suất hữu hiệu.
- Ống Casagrande chỉ thích hợp cho cát và cuội sỏi; đất sét dẻo bắt buộc phải dùng piezometer màng cứng (VW).
- Khử bọt khí và bão hòa đá lọc là bước thi công bắt buộc trước khi lắp đặt.
- Phương pháp bơm vữa chèn toàn phần (fully grouted) là giải pháp lắp đặt hiện đại, tin cậy và tối ưu tiến độ.
