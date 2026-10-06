---
lang: vi
lang_alt: reference-manuals/dunnicliff/chapter-09-load-strain-temp/
---

# Chương 9 — Đo tải trọng, biến dạng kết cấu và nhiệt độ

## 9.1 Quan trắc lực trong kết cấu địa kỹ thuật

Tại những vị trí khối đất đá tương tác trực tiếp với các cấu kiện gia cố nhân tạo — như thanh chống hố đào (struts), neo trong đất (tiebacks), bu lông neo đá (rock bolts), cọc móng và vỏ hầm — việc quan trắc **tải trọng và biến dạng nội lực** là biện pháp kiểm chứng an toàn kết cấu và phát hiện sớm hiện tượng quá tải nguy hiểm.

## 9.2 Tế bào đo tải (Load Cells)

### Cấu tạo và chủng loại
- **Tế bào đo tải rỗng tâm (Center-hole Load Cells)**: Thiết kế dạng đĩa vành khăn có lỗ xuyên tâm để xỏ qua thanh neo đất, tao cáp dự ứng lực hoặc bu lông neo đá. Bên trong vành thép tích hợp từ 3 đến 6 cảm biến dây rung bố trí đối xứng hình học xung quanh đường tròn để tự động triệt tiêu sai số do tải trọng lệch tâm (eccentric loading).
- **Tế bào đo tải thanh chống (Strut Load Cells)**: Tế bào nén hình trụ gắn tại đầu mút thanh chống thép hình của hố đào sâu, đo lực ép dọc trục do tường vây truyền vào hệ giằng.

### Lưu ý sử dụng
Bắt buộc phải sử dụng các tấm đệm phân bố tải trọng bằng thép gia công cơ khí phẳng song song (spherical bearing plates hoặc hardened washer plates) ở mặt trên và mặt dưới của tế bào đo tải để đảm bảo lực truyền phân bố đều, tránh làm méo mó và hỏng cảm biến.

## 9.3 Đầu đo biến dạng (Strain Gauges)

Đầu đo biến dạng đo trực tiếp độ giãn dài hoặc co ngắn tương đối ($\varepsilon = \Delta L / L$) của vật liệu kết cấu:

- **Cảm biến hàn (Arc-weldable VWSG)**: Hàn điểm trực tiếp lên cánh hoặc bụng của thép hình thanh chống, cọc thép cừ larsen hoặc ống chống vách.
- **Thanh đo biến dạng bê tông (Sister Bar)**: Cảm biến dây rung được bảo vệ sẵn bên trong một thanh cốt thép ngắn ($D = 12 - 16\text{ mm}$), được buộc song song vào lồng cốt thép chịu lực chính của cọc khoan nhồi, dầm giằng hoặc tường vây trước khi đổ bê tông.

### Quy đổi từ Biến dạng ($\varepsilon$) sang Lực ($P$):

$$P = \varepsilon \cdot E \cdot A$$

Trong đó $A$ là diện tích mặt cắt ngang và $E$ là mô đun đàn hồi của vật liệu.

!!! warning "Lưu ý sống còn về mô đun đàn hồi của bê tông"
    Mô đun đàn hồi $E$ của bê tông thay đổi liên tục theo thời gian ninh kết, đồng thời bê tông chịu ảnh hưởng rất lớn từ hiện tượng **co ngót (shrinkage)** và **từ biến (creep)**. Nếu chỉ đo biến dạng rồi nhân với một hằng số $E$ giả định, sai số tính toán tải trọng có thể lên đến 50–100%! Bắt buộc phải đặt các cảm biến biến dạng không chịu tải (No-stress dummy gauges) đúc trong các khối bê tông cùng cấp phối để trừ đi biến dạng do nhiệt và co ngót tự nhiên.

## 9.4 Thanh truyền chuyển vị (Telltale Extensometer)

Trong thí nghiệm nén tĩnh cọc, việc đo lún đỉnh cọc không phản ánh được mức độ lún thực tế của mũi cọc:
- Thanh truyền telltale là một thanh thép tự do luồn trong ống bảo vệ, cắm cố định tại mũi cọc hoặc các phân đoạn cọc.
- Đồng hồ so đo độ lún của đỉnh thanh telltale so với dầm chuẩn sẽ phản ánh chính xác độ lún của mũi cọc, cho phép phân tách rành mạch giữa **độ nén đàn hồi của thân cọc**, **sức kháng ma sát thành bên (skin friction)** và **sức kháng mũi cọc (end bearing)**.

## 9.5 Đo nhiệt độ và hiệu chỉnh nhiệt độ

Nhiệt độ là yếu tố môi trường gây biến động dữ liệu mạnh nhất trong quan trắc địa kỹ thuật:
- **Cảm biến nhiệt độ**: Các cảm biến dây rung hiện đại đều tích hợp sẵn nhiệt điện trở NTC $3\text{ k}\Omega$.
- **Công thức hiệu chỉnh nhiệt độ**:

$$P_{\text{hiệu chỉnh}} = P_{\text{đo}} + C_T \cdot (T - T_0)$$

- **Ứng dụng công trình**: Đo nhiệt thủy hóa bê tông khối lớn trong đài móng cọc khoan nhồi, trụ tháp cầu và khối đập bê tông để kiểm soát gradient nhiệt độ chống nứt nẻ.

## 9.6 Các điểm then chốt cần ghi nhớ

- Tế bào đo tải rỗng tâm phải có từ 3 cảm biến trở lên để triệt tiêu tải trọng lệch tâm.
- Sử dụng tấm đệm phẳng gia công cơ khí chuẩn khi lắp đặt load cell.
- Tính toán tải trọng từ biến dạng bê tông bắt buộc phải bù trừ co ngót và từ biến.
- Thanh telltale là công cụ kinh tế và chính xác để đo chuyển vị mũi cọc độc lập với thân cọc.
- Mọi cảm biến dây rung đều phải được ghi nhận nhiệt độ và hiệu chỉnh sai số nhiệt.
