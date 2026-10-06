---
lang: vi
lang_alt: glossary/
---

# 📖 Từ điển Thuật ngữ Quan trắc Địa kỹ thuật & Hệ thống ADAQS

> Từ điển và sổ tay thuật ngữ chuyên sâu về quan trắc hiện trường địa kỹ thuật, cảm biến công trình, vật lý đo lường, hệ thống thu thập dữ liệu tự động (ADAQS/ADAS) và truyền dữ liệu không dây. Căn cứ theo các tiêu chuẩn quốc tế (ISO 18674, ASTM, BS 5930), tiêu chuẩn Việt Nam (TCVN 9398, TCVN 9360, Nghị định 114/2018/NĐ-CP) và các nguyên lý của John Dunnicliff.

---

## 1. Cảm biến địa kỹ thuật & Thiết bị đo ngầm

### Áp lực nước lỗ rỗng & Mực nước ngầm

* **Piezometer (Đầu đo áp lực nước lỗ rỗng / Áp kế)**: Thiết bị quan trắc đặt trong đất, đá hoặc vật liệu đắp để đo áp lực nước lỗ rỗng hoặc cao trình mực nước ngầm.
* **Vibrating Wire Piezometer - VWP (Đầu đo áp lực kiểu dây rung)**: Cảm biến có màng ngăn kim loại đàn hồi nối với một sợi dây thép căng. Áp lực nước tác dụng lên màng làm thay đổi độ căng của dây thép và làm thay đổi tần số dao động tự nhiên ($f$) của nó. Rất ổn định lâu dài và không bị suy giảm tín hiệu trên đường cáp dài.
* **Standpipe Piezometer - Casagrande (Ống đo áp lực hở kiểu Casagrande)**: Ống đo áp lực gồm một mũi lọc bằng gốm xốp hoặc nhựa gắn ở đáy ống đứng. Đo mực nước thủy tĩnh bằng thiết bị đo mực nước cầm tay (đèn còi / dip meter).
* **Pneumatic Piezometer (Đầu đo áp lực kiểu khí nén)**: Cảm biến màng van vận hành bằng áp lực khí (thường là nitơ). Bơm khí theo đường ống nạp đến khi cân bằng với áp lực nước lỗ rỗng làm mở van xả khí qua ống hồi. Không gây biến đổi thể tích nước, độ trễ thủy lực gần như bằng 0.
* **Drive-In / Push-In Piezometer (Đầu đo áp lực kiểu đóng / ấn trực tiếp)**: Đầu đo có mũi côn thép chịu lực cao, được ấn trực tiếp vào các tầng sét mềm hoặc bùn mà không cần khoan tạo lỗ trước.
* **Màng lọc High-Air-Entry (HAE) và Low-Air-Entry (LAE)**:
    * **HAE Ceramic (Màng lọc khí cao)**: Kích thước lỗ rỗng cực nhỏ (1–2 µm), áp lực sủi bọt cao, ngăn không cho khí lọt vào buồng đo trong điều kiện áp lực nước lỗ rỗng âm (lực hút dính matrict) ở đất chưa bão hòa.
    * **LAE Carborundum (Màng lọc khí thấp)**: Kích thước lỗ rỗng tiêu chuẩn (~50 µm), thấm nước nhanh, dùng trong điều kiện đất bão hòa nước thông thường.
* **Multi-Level Piezometer Array (Cụm đầu đo áp lực nhiều tầng)**: Lắp đặt nhiều đầu đo VWP ở các cao trình khác nhau trong cùng một lỗ khoan để quan sát gradient thủy lực thẳng đứng và các tầng thấm kẹp.

### Thiết bị đo chuyển vị ngang & Biến dạng sườn dốc

* **Inclinometer Casing (Ống đo nghiêng)**: Ống nhựa chuyên dụng (thường bằng ABS hoặc hợp kim nhôm) có 4 rãnh định hướng vuông góc bên trong, dẫn hướng cho đầu đo nghiêng di chuyển dọc theo trục chính xác.
* **Traversing Probe Inclinometer (Thiết bị đo nghiêng luồn cáp)**: Đầu đo hình thoi có bánh xe chứa 2 cảm biến gia tốc servo hoặc MEMS vuông góc, được thả dọc theo ống rãnh bằng cáp điều khiển có vạch chia khoảng cách (0.5 m) để đo góc nghiêng tích lũy.
* **In-Place Inclinometer - IPI (Thiết bị đo nghiêng cố định trong lỗ khoan)**: Chuỗi các đầu đo góc nghiêng liên kết với nhau bằng thanh truyền và treo cố định tại các tầng đất trọng yếu, kết nối với bộ ghi tự động để theo dõi chuyển vị ngang liên tục.
* **ShapeArray - SAA (Mảng cảm biến hình dạng 3D linh hoạt)**: Chuỗi các đốt cảm biến MEMS 3 trục siêu nhỏ kết nối với nhau bằng khớp mềm, cho phép uốn cong theo chuyển vị đất và xuất biên dạng chuyển vị 3D thời gian thực.
* **Horizontal Inclinometer (Thiết bị đo nghiêng nằm ngang)**: Hệ thống ống rãnh lắp đặt theo phương ngang dưới đáy nền đắp, đập hoặc bãi chôn lấp để đo biểu đồ lún và trồi theo phương đứng.
* **Spiral Twist Survey (Đo độ xoắn rãnh ống đo nghiêng)**: Phép đo kiểm tra độ vặn xoắn cơ học của các rãnh ống qua chiều sâu lỗ khoan lớn, dùng để hiệu chỉnh góc phương vị của chuyển vị ngang.

### Đo lún & Chuyển vị thẳng đứng

* **Multipoint Borehole Extensometer - MPBX (Thiết bị đo biến dạng nhiều điểm trong lỗ khoan)**: Cụm các mỏ neo cố định tại các độ sâu khác nhau trong lỗ khoan, nối bằng thanh thép/sợi thủy tinh qua ống bảo vệ lên đầu đo tham chiếu ở miệng lỗ khoan. Đo độ giãn dài hoặc co ngắn của các tầng đất đá.
* **Magnetic Settlement Gauge (Thiết bị đo lún kiểu từ trường)**: Gồm ống dẫn hướng bọc ngoài bởi các mỏ neo nam châm cánh nhện cắm chặt vào thành lỗ khoan. Đầu đo công tắc từ (reed switch) luồn trong ống sẽ phát tín hiệu âm thanh khi đi qua từng vòng nam châm.
* **Liquid Level Settlement Cell (Tế bào đo lún kiểu thủy tĩnh)**: Cảm biến áp lực vi sai kết nối bằng ống chứa chất lỏng với bình chuẩn tham chiếu, đo độ chênh cao thẳng đứng của kết cấu hoặc bản móng ngầm.
* **Settlement Plate (Bàn đo lún / Mốc đĩa đo lún)**: Bản thép đặt trên mặt đất tự nhiên trước khi đắp đất, hàn với ống đứng nối dài dần theo chiều cao đắp.
* **Tape Extensometer (Thước thép đo hội tụ)**: Thước đo thép có đồng hồ đo vi sai và bộ phận tạo lực căng chuẩn, dùng để đo cự ly hội tụ giữa các mốc gắn trên vách hầm hoặc thanh chống hố đào.

### Tải trọng & Ứng suất kết cấu

* **Anchor Load Cell (Đầu đo tải trọng neo / Load cell vòng)**: Thiết bị đặt dưới đai ốc của neo đất, neo đá hoặc đầu thanh chống để đo lực kéo hoặc lực nén dọc trục. Thường chứa từ 3 đến 6 cảm biến dây rung bố trí song song.
* **Vibrating Wire Strain Gauge - VWSG (Cảm biến đo biến dạng dây rung)**: Cảm biến hàn lên kết cấu thép hoặc đúc trực tiếp trong bê tông (thanh đo biến dạng sister bar) để đo biến dạng vi mô ($\mu\varepsilon$).
* **Earth Pressure Cell - EPC (Hộp đo áp lực đất / Áp lực tổng)**: Gồm hai tấm thép tròn hoặc chữ nhật hàn kín mép, ở giữa chứa dầu thủy lực không chịu nén nối với cảm biến áp lực. Đặt tại mặt tiếp xúc giữa đất và công trình hoặc trong thân đập.
* **Tiltmeter (Đầu đo độ nghiêng kết cấu)**: Cảm biến gắn trên tường chắn, trụ cầu hoặc công trình lân cận để đo góc nghiêng xoay theo 1 hoặc 2 trục.
* **Crackmeter / Jointmeter (Đầu đo khe nứt / Khe nối)**: Thiết bị đo khoảng cách vi sai gắn bắc qua vết nứt bê tông hoặc khe nối khối đá để theo dõi độ mở rộng, khép lại và trượt của khe.

---

## 2. Hệ thống Thu thập Dữ liệu Tự động (ADAQS) & Truyền thông

### Xử lý tín hiệu & Chuẩn giao tiếp

* **ADAQS / ADAS (Hệ thống thu thập dữ liệu tự động)**: Hệ thống tích hợp gồm cảm biến, bộ ghi dữ liệu, nguồn năng lượng và mô-đun viễn thông hoạt động độc lập không cần người trực tiếp tại hiện trường.
* **Kích thích dao động dây rung (Pluck Frequency Excitation)**: Cuộn dây điện từ phóng xung điện quét tần số để làm dây thép dao động tự do, sau đó cuộn dây thu nhận điện áp cảm ứng hình sin phát ra từ dây.
* **Công nghệ phân tích phổ (VSPECT / Spectral Analysis)**: Kỹ thuật biến đổi Fourier nhanh (FFT) trên tín hiệu dao động dây rung, bóc tách chính xác tần số dao động cơ bản của dây ngay cả khi môi trường bị nhiễu điện từ mạnh.
* **Vòng dòng 4–20 mA (Current Loop)**: Chuẩn truyền tín hiệu analog dạng dòng điện, miễn nhiễm với điện trở suy hao của cáp truyền khoảng cách xa.
* **RS-485 / Modbus RTU**: Chuẩn truyền thông nối tiếp vi sai cân bằng, cho phép kết nối mạng chuỗi (multidrop) lên tới hơn 32 cảm biến kỹ thuật số trên khoảng cách dây dẫn tới 1.200 m.
* **SDI-12**: Chuẩn giao tiếp kỹ thuật số năng lượng thấp, tốc độ 1200 baud, chuyên dụng cho cảm biến môi trường và địa kỹ thuật.
* **CAN Bus / CANopen**: Giao thức mạng truyền dữ liệu tốc độ cao, độ tin cậy cực lớn trong môi trường máy đào hầm (TBM) và ngầm.

### Mạng truyền thông không dây & Phần cứng hiện trường

* **Data Logger (Đầu ghi dữ liệu / Bộ tích lũy số liệu)**: Thiết bị điện tử cấp nguồn cho cảm biến, số hóa tín hiệu analog, tính toán theo công thức hiệu chuẩn và lưu trữ dữ liệu kèm mốc thời gian vào bộ nhớ flash.
* **Relay Multiplexer (Bộ ghép kênh / Bộ chuyển mạch)**: Mô-đun mở rộng dùng rơ-le bán dẫn hoặc rơ-le tiếp điểm kín để tuần tự chuyển tín hiệu từ nhiều cảm biến vào một kênh đo của bộ ghi.
* **LoRaWAN (Mạng diện rộng công suất thấp)**: Giao thức truyền không dây tầm xa hoạt động trên dải tần không cấp phép (868 MHz, 915 MHz, 923 MHz). Khả năng xuyên thấu cao qua địa hình đồi núi và hố móng sâu.
* **Mạng không dây dạng lưới (Wireless Mesh Network)**: Cấu trúc mạng tự kết nối và tự phục hồi, trong đó các nút cảm biến đóng vai trò làm trạm tiếp sức chuyển tiếp gói tin về trạm gốc (Gateway).
* **Cellular IoT (NB-IoT & LTE-M)**: Chuẩn mạng di động băng hẹp tiêu thụ ít năng lượng, truyền dữ liệu cảm biến trực tiếp lên đám mây qua trạm BTS viễn thông.
* **Vệ tinh viễn thông (Satellite Telemetry - Iridium SBD)**: Truyền dữ liệu qua vệ tinh quỹ đạo thấp, phục vụ các công trình thủy điện, hồ chứa nước ở vùng rừng núi hiểm trở không có sóng di động.
* **Hệ thống điện mặt trời & Bộ nạp MPPT**: Tấm pin năng lượng mặt trời kết hợp bộ điều khiển nạp theo dõi điểm công suất tối đa (MPPT) và ắc quy khô AGM hoặc pin LiFePO4 cho phép trạm đo vận hành liên tục nhiều năm.

---

## 3. Vật lý Đo lường & Công thức Tính toán

### Cảm biến dây rung (Vibrating Wire)

* **Phương trình tần số dao động cơ bản**: Tần số tự nhiên $f$ của sợi dây thép hai đầu ngàm chịu kéo $\sigma$:

    $$
    f = \frac{1}{2L} \sqrt{\frac{\sigma}{\rho}} = \frac{1}{2L} \sqrt{\frac{E \cdot \varepsilon}{\rho}}
    $$

    Trong đó $L$ là chiều dài dây, $\rho$ là khối lượng riêng, $E$ là mô-đun đàn hồi, và $\varepsilon$ là độ biến dạng tương đối của dây.

* **Đơn vị Digits (Số đọc tuyến tính)**:

    $$
    \text{Digits} = \frac{f^2}{1000}
    $$

* **Phương trình hiệu chuẩn tuyến tính**:

    $$
    P = G \cdot (R_0 - R)
    $$

    Trong đó $G$ là hệ số hiệu chuẩn (gage factor), $R_0$ là số đọc ban đầu (digits), và $R$ là số đọc hiện tại.

* **Phương trình hiệu chuẩn đa thức bậc 2**:

    $$
    P = A \cdot R^2 + B \cdot R + C
    $$

* **Hiệu chỉnh nhiệt độ** ($K_T$):

    $$
    P_{corr} = P_{raw} + K_T \cdot (T - T_0)
    $$

    Bù trừ sự chênh lệch giãn nở nhiệt giữa sợi dây thép và vỏ thân cảm biến bằng thép không gỉ.

* **Hiệu chỉnh áp suất khí quyển (Barometric Compensation)**:

    $$
    P_{net} = P_{do} - (B - B_0)
    $$

    Bắt buộc áp dụng cho các piezometer màng kín để loại bỏ sự thay đổi áp suất khí quyển của thời tiết ra khỏi áp lực nước ngầm thực tế.

### Xử lý số liệu Inclinometer

* **Độ lệch phân đoạn** ($\delta_i$):

    $$
    \delta_i = L \cdot \sin(\theta_i) = C \cdot (A_0 - A_{180})
    $$

    Trong đó $L$ là chiều dài cơ sở đầu đo (thường 500 mm), $\theta_i$ là góc nghiêng, $A_0$ và $A_{180}$ là hai lần đo đảo ngược $180^\circ$.

* **Tổng kiểm tra (Check Sum)**:

    $$
    \text{Check Sum} = A_0 + A_{180}
    $$

    Giá trị Check Sum phải gần như không đổi ở mọi độ sâu, chứng minh cảm biến hoạt động chính xác và bánh xe không bị kẹt bụi bẩn.

* **Chuyển vị tích lũy** ($D_k$):

    $$
    D_k = \sum_{i=1}^k \delta_i
    $$

    Tích lũy chuyển vị tính từ đáy lỗ khoan (điểm mốc ngàm cố định) lên dần đến miệng lỗ khoan.

---

## 4. Quản lý Rủi ro & Kế hoạch Ứng phó TARP

* **TARP (Trigger Action Response Plan - Kế hoạch Hành động theo Ngưỡng kích hoạt)**: Khung quản lý rủi ro quy định cụ thể các hành động kỹ thuật ứng với từng cấp độ đo đạc:
    * **Cấp 0 (Xanh lá / Bình thường)**: Số liệu nằm trong giới hạn thiết kế dự báo. Chu kỳ đo đạc tiêu chuẩn.
    * **Cấp 1 (Vàng / Cảnh báo)**: Giá trị vượt ngưỡng thống kê nền hoặc đạt 50–70% giới hạn cho phép. Tăng gấp đôi tần suất đo; cử kỹ sư kiểm tra thực địa.
    * **Cấp 2 (Cam / Nguy cơ)**: Tốc độ chuyển dịch gia tăng nhanh hoặc ứng suất tiệm cận tải trọng thiết kế. Kích hoạt hội đồng chuyên gia, kiểm tra chéo bằng thiết bị phụ trợ, chuẩn bị phương án gia cố.
    * **Cấp 3 (Đỏ / Hành động Khẩn cấp)**: Vượt ngưỡng an toàn nghiêm trọng; có nguy cơ trượt lở hoặc bục vỡ công trình. Dừng thi công ngay lập tức, sơ tán hiện trường và kích hoạt biện pháp cứu nạn khẩn cấp.
* **Tốc độ chuyển vị ($v = \frac{d\delta}{dt}$)**: Vận tốc biến dạng theo thời gian. Sự gia tăng gia tốc chuyển dịch là dấu hiệu báo trước chuẩn xác nhất của thảm họa sạt trượt mái dốc và sập hố móng.
* **Đường bão hòa (Phreatic Surface / Seepage Line)**: Ranh giới mặt trên của dòng thấm qua thân đập đất, tại đó áp lực nước lỗ rỗng bằng áp lực khí quyển.
* **Xói ngầm (Piping / Internal Erosion)**: Hiện tượng dòng thấm cuốn trôi các hạt đất mịn bên trong thân đập hoặc nền, tạo thành các đường hầm xói ngầm dẫn đến vỡ đập.

---

## 5. Phương pháp Lắp đặt Hiện trường & Kỹ thuật Bơm vữa

* **Phương pháp bơm vữa toàn bộ (Fully Grouted Method - Mikkelsen / Contreras)**: Phương pháp lắp đặt đầu đo áp lực VWP trực tiếp vào lỗ khoan rồi bơm vữa xi măng-bentonite lấp đầy toàn bộ lỗ khoan mà không cần túi cát lọc hay viên bentonite truyền thống. Nhờ thể tích biến dạng màng đo cực nhỏ, áp lực nước lỗ rỗng truyền qua lớp vữa hầu như tức thời.
* **Tỷ lệ cấp phối vữa (Grout Mix)**: Tỷ lệ pha trộn Nước : Xi măng : Bột Sodium Bentonite theo khối lượng:
    * *Đất mềm / Đất sét*: Nước : Xi măng : Bentonite $\approx$ 2.5 : 1.0 : 0.3 đến 0.4.
    * *Đá cứng / Đất chặt*: Nước : Xi măng : Bentonite $\approx$ 1.5 : 1.0 : 0.1.
* **Khớp nối trượt co giãn (Telescoping Coupling)**: Các đoạn khớp nối lồng trượt lắp dọc theo ống đo nghiêng hoặc ống đo lún để tránh cho ống bị nén gập gãy khi nền đất xảy ra độ lún lớn.

---

*Xem thêm: [English Technical Glossary](../../glossary/index.md) · [Ma trận Tuân thủ Nghị định 114 & TCVN 9398](../tuan-thu/nghi-dinh-114-tcvn-9398.md) · [Môi trường thử nghiệm tương tác](../visualizer.md)*
