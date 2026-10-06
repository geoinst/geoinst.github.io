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

## 6. Cơ sở Lưu giữ Bùn thải & An toàn Đập bùn thải

* **Bùn thải (Tailings)**: Chất thải rắn dạng hạt mịn còn lại sau khi tách kim loại/khoáng sản khỏi quặng, được vận chuyển và thải dưới dạng huyền phù (bùn).
* **Cơ sở lưu giữ bùn thải - TSF (Tailings Storage Facility)**: Toàn bộ hệ thống lưu giữ gồm đập/đê chắn, khối bùn thải lắng đọng, hồ nước bề mặt, hệ thống xả tràn và công trình thu hồi nước.
* **Đập bùn thải (Tailings Dam)**: Đập/đê nhân tạo chắn giữ khối bùn thải; thường được nâng cao dần theo tuổi mỏ và nhiều khi được đắp từ chính bùn thải.
* **Đợt đắp cao (Embankment Raise / Dam Raise)**: Mỗi lần nâng cao đập bùn thải, đắp theo phương pháp thượng nguồn, tim tuyến hoặc hạ lưu.
* **Phương pháp đắp hạ lưu (Downstream Method)**: Mỗi đợt nâng được đắp lùi về phía hạ lưu so với đợt trước, phần lớn thân đập tựa trên nền móng — phương pháp an toàn nhất.
* **Phương pháp đắp tim tuyến (Centerline Method)**: Các đợt nâng đắp trên tim tuyến ban đầu; mức rủi ro trung bình.
* **Phương pháp đắp thượng nguồn (Upstream Method)**: Mỗi đợt nâng đắp về phía thượng nguồn, thân đập tựa trên bùn thải lỏng, bão hòa — rủi ro cao nhất, dễ hóa lỏng.
* **Bãi bùn (Beach)**: Mặt dốc thoải của khối bùn thải lắng đọng giữa điểm xả bùn và hồ nước bề mặt.
* **Hình học bãi bùn (Beach Geometry)**: Độ dốc và chiều dài bãi bùn, quyết định vị trí mặt nước thấm và chiều cao an toàn được duy trì.
* **Hồ nước bề mặt (Supernatant Pond)**: Khối nước trong phía trên khối bùn lắng, được thu hồi hoặc xả tràn.
* **Hệ thống xả tràn - Decant (Decant Tower / Decant System)**: Kết cấu và đường ống dùng để tháo nước bề mặt, kiểm soát mực hồ và chiều cao an toàn.
* **Chiều cao an toàn - Freeboard (Freeboard)**: Khoảng cách thẳng đứng giữa mặt hồ và điểm thấp nhất của đỉnh đập; biện pháp bảo vệ chính chống tràn qua đỉnh.
* **Phân phối bùn (Spigotting / Deposition)**: Xả bùn từ đỉnh đập để tạo bãi bùn bằng phương pháp lắng đọng thủy lực.
* **Bùn thải cô đặc / hồ dẻo / lọc ép (Thickened / Paste / Filtered Tailings)**: Bùn thải đã khử nước (hàm lượng rắn tăng dần), giảm nước tự do và giảm nguy cơ hóa lỏng.
* **Lưu giữ trong hố khai thác / bãi vành khuyên (In-Pit / Paddock Storage)**: Lưu giữ bùn thải trong hố mỏ đã khai thác hoặc bãi đê vành khuyên thay vì đập chắn thung lũng.
* **Hóa lỏng (Liquefaction)**: Mất sức kháng cắt khi đất bão hòa, rời (co ngót thể tích) bị gia tải hoặc rung động và áp lực nước lỗ rỗng tăng đến mức ứng suất hiệu dụng gần bằng không.
* **Hóa lỏng tĩnh (Static Liquefaction)**: Hóa lỏng do tải trọng tĩnh (đợt nâng cao, mực hồ dâng nhanh, hoặc nền yếu) chứ không do động đất — cơ chế thảm khốc chủ đạo của phá hoại đập bùn thải.
* **Hóa lỏng do động đất (Seismic Liquefaction)**: Hóa lỏng do rung động lặp của động đất.
* **Tỷ số áp lực lỗ rỗng ($r_u$)**: Tỷ số giữa áp lực nước lỗ rỗng đo được và ứng suất hiệu dụng thẳng đứng ban đầu ($r_u = u / \sigma'_v$); giá trị tăng báo hiệu nguy cơ hóa lỏng.
* **Áp lực lỗ rỗng dư (Excess Pore Pressure)**: Áp lực nước lỗ rỗng vượt giá trị ổn định (thủy tĩnh), sinh ra do gia tải, thi công hoặc rung động.
* **Phá hoại dòng chảy / tầm xa (Flow Failure / Run-out)**: Khối đất đã hóa lỏng chảy nhanh và đi xa, gây thiệt hại nghiêm trọng ở hạ lưu.
* **Tầng thoát nước chân đập (Toe Drain)**: Đới thấm hoặc rãnh thoát ở chân hạ lưu để thu và kiểm soát dòng thấm, giữ mặt nước thấm ở mức thấp.
* **Thấm đục (Turbid Seepage)**: Dòng thấm mang theo hạt đất mịn (nước đục) — dấu hiệu cảnh báo xói mòn trong (piping).
* **Cấp hậu quả (Consequence Category)**: Phân loại cơ sở theo mức ảnh hưởng tiềm ẩn ở hạ lưu khi phá hoại (thường A/B/C), quyết định cường độ giám sát và kiểm tra.
* **Đóng cửa mỏ (Closure / Mine Closure)**: Giai đoạn sau khai thác, cơ sở được ngừng vận hành và làm an toàn, đòi hỏi giám sát tiếp tục cho đến khi đạt trạng thái ổn định lâu dài.
* **InSAR / A-DInSAR (Giao thoa radar vệ tinh)**: Kỹ thuật viễn thám dùng các lần vệ tinh radar lặp lại để đo chuyển vị mặt đất cỡ milimét trên toàn cơ sở mà không cần thiết bị tại chỗ.

---

## 7. Giám sát Hiệu năng Đập (phạm vi ASCE MOP-135)

* **Hiệu năng đập (Dam Performance)**: Ứng xử quan sát được của đập, nền và công trình phụ trợ so với ứng xử mong đợi.
* **Ứng xử mong đợi so với đo được (Expected vs. Measured Behavior)**: Phép so sánh cốt lõi của quan trắc; khác biệt lớn, không giải thích được hoặc có xu hướng là một bất thường.
* **Tín hiệu hiệu năng (Performance Signal)**: Chênh lệch giữa ứng xử đo được và mong đợi, dùng để đánh giá đập có vận hành chấp nhận được hay không.
* **Mode phá hoại tiềm ẩn (Potential Failure Mode)**: Một cách phá hoại khả dĩ của đập (tràn qua đỉnh, xói mòn trong, mất ổn định mái dốc, thấm nền); cơ sở để lựa chọn thiết bị quan trắc.
* **Áp lực đẩy nổi - Uplift (Uplift)**: Áp lực nước hướng lên tác dụng lên đáy đập bê tông hoặc trong nền, làm giảm ổn định.
* **Công trình phụ trợ (Appurtenant Structures)**: Các công trình hỗ trợ như tràn xả lũ, công trình lấy nước và hệ thống xả tràn.
* **Lún / chuyển vị đỉnh đập (Crest Settlement / Displacement)**: Chuyển động thẳng đứng hoặc ngang của đỉnh đập — chỉ báo biến dạng chính.
* **Kế hoạch giám sát (Surveillance Plan)**: Chương trình được lập thành văn bản nêu rõ giám sát cái gì (trực quan và bằng thiết bị), tần suất nào, và cách ứng phó với từng bất thường.
* **Kiểm tra độc lập (Independent Review)**: Định kỳ rà soát dữ liệu và chương trình quan trắc bởi một bên độc lập với đội vận hành, nhằm phát hiện các xu hướng bị "bình thường hóa".

---

## 8. Lập kế hoạch Chương trình Quan trắc & Độ tin cậy (Dunnicliff)

* **Thiết bị quan trắc địa kỹ thuật (Geotechnical Instrumentation)**: Việc đo ứng xử của đất, đá, nền và kết cấu nhằm xác nhận hiệu năng và phát hiện thay đổi.
* **Tiếp cận lập kế hoạch có hệ thống (Systematic Planning Approach)**: Quy trình có cấu trúc của Dunnicliff (trọng tâm của cuốn sách): xác định câu hỏi địa kỹ thuật trước, rồi mới chọn thông số, thiết bị, vị trí và tần suất.
* **Câu hỏi địa kỹ thuật (Geotechnical Question)**: Câu hỏi cụ thể mà việc quan trắc phải trả lời (ví dụ: "tường có vượt chuyển vị cho phép không?"), quyết định đo cái gì và hỗ trợ quyết định nào.
* **Chuỗi 25 mắt xích (The Chain of 25 Links)**: Ẩn dụ của Dunnicliff: thành công của quan trắc là một chuỗi từ xác định nhu cầu dự án đến số đọc phục vụ quyết định; đứt bất kỳ mắt xích nào, cả chuỗi thất bại.
* **Công thức cho sự tin cậy (Recipe for Reliability)**: Tập hợp các "thành phần" (lựa chọn, mua sắm, lắp đặt, hiệu chuẩn, đọc số, bảo trì, xử lý dữ liệu, con người) tạo nên sự tin cậy của quan trắc.
* **Phương pháp quan sát (Observational Method)**: Cách tiếp cận thiết kế được tinh chỉnh trong quá trình thi công dựa trên hiệu năng quan trắc được.
* **Cảm biến biến đổi (Transducer)**: Thiết bị chuyển đổi một đại lượng vật lý (áp lực, chuyển vị, tải) thành tín hiệu điện hoặc khí nén.
* **Độ chính xác so với độ đúng đắn (Accuracy vs. Precision)**: Độ chính xác là mức gần với giá trị thật; độ đúng đắn (độ lặp lại) là mức gần nhau của các số đọc lặp. Riêng một yếu tố không đảm bảo phép đo tốt.
* **Hiện tượng trễ (Hysteresis)**: Sự phụ thuộc của đầu ra thiết bị vào chiều thay đổi (tăng tải so với giảm tải).
* **Ngân sách sai số (Error Budget)**: Tổng hợp ảnh hưởng của mọi nguồn không đảm bảo riêng lẻ (cảm biến, cáp, thiết bị đọc, môi trường), giới hạn tổng độ không đảm bảo của phép đo.
* **Hệ số hiệu chuẩn / Điểm không / Dải đo (Calibration Factor / Zero / Span)**: Độ dốc của quan hệ đầu vào–đầu ra (hệ số hiệu chuẩn), số đọc khi đầu vào bằng không (điểm không) và toàn dải đo (dải đo).
* **Số đọc cơ sở (Baseline Reading)**: (Các) số đọc tham chiếu lấy sau khi lắp đặt và ổn định, dùng làm mốc so sánh cho mọi thay đổi về sau.
* **Cột áp piezometric (Piezometric Head)**: Cao độ mặt nước tương đương ứng với một áp lực nước lỗ rỗng đo được.
* **Độ trễ thủy lực (Hydraulic Time Lag)**: Độ trễ phản hồi của piezometer trước thay đổi áp lực nước lỗ rỗng, phụ thuộc tính thấm và hình học của đất xung quanh và màng lọc.
* **Bão hòa / Khử khí (Saturation / De-airing)**: Quy trình loại bỏ không khí khỏi màng lọc và ống nối của piezometer để nó phản hồi đúng áp lực nước lỗ rỗng; bước lắp đặt quan trọng, hay bị bỏ qua.
* **Hội tụ (Convergence)**: Sự co ngắn (khép) khoảng cách giữa các điểm trong hầm hoặc hố đào, biểu thị chuyển động của đất.
* **Telltale (Thiết bị báo chuyển vị)**: Thiết bị đơn giản chỉ thị chuyển động tương đối bắc qua một khe nối hoặc tiết diện.
* **Thanh sister bar (Sister Bar)**: Đầu đo biến dạng dây rung gắn song song với thanh thép (rebar) để đo biến dạng của thanh khi đúc trong bê tông.
* **Khoan giải ứng suất (Overcoring)**: Kỹ thuật giải phóng ứng suất, trong đó thiết bị trong lỗ khoan được giải phóng bằng khoan bao quanh để tính ngược trạng thái ứng suất nguyên sinh của đá.
* **Kích nạp phẳng (Flat Jack)**: Kích thủy lực mỏng đặt vào rãnh cắt trên đá để đo giải phóng ứng suất và ước lượng ứng suất nguyên sinh.
* **Tế bào áp lực hố khoan - BPC (Borehole Pressure Cell)**: Thiết bị bơm vữa cố định trong lỗ khoan để theo dõi thay đổi ứng suất đá quanh đường hầm/hố đào.
* **Tế bào ứng suất tiếp xúc (Contact Stress Cell)**: Tế bào áp lực đặt áp sát mặt tiếp xúc đất–kết cấu để đo ứng suất tiếp xúc.

## 9. Thiết bị quan trắc đường bộ FHWA (phạm vi FHWA-HI-98-034)

* **Quy tắc vàng (quan trắc)**: Mỗi thiết bị phải được chọn và đặt để trả lời một câu hỏi địa kỹ thuật cụ thể — nếu không có câu hỏi, thì không nên có thiết bị.
* **Chuỗi 31 mắt xích (Chain of 31 Links)**: 21 mắt xích lập kế hoạch cộng 10 mắt xích thực thi; tất cả phải đứng vững để chương trình quan trắc thành công — chỉ một mắt xích yếu có thể làm đứt cả chuỗi.
* **Tế bào áp lực đất chôn (Embedment Earth Pressure Cell)**: Tế bào dẹt chứa chất lỏng, chôn trong đất để đo ứng suất tổng vuông góc với mặt của nó.
* **Tỷ số kích thước (Aspect Ratio – tế bào)**: Tỷ số đường kính trên chiều dày của tế bào áp lực đất; tỷ số cao giúp giảm sai số đo.
* **Tỷ số độ cứng đất/tế bào (Soil/Cell Stiffness Ratio)**: Tỷ số quyết định mức độ tế bào áp lực đất phân phối lại ứng suất cục bộ, và do đó quyết định sai số đo.
* **Giếng quan sát (Observation Well)**: Ống hở không có lớp bịt dưới bề mặt; tạo kết nối thẳng đứng giữa các tầng nên hiếm khi phù hợp để quan trắc hiệu năng.
* **Piezometer ống đứng hở – Casagrande (Open Standpipe Piezometer)**: Ống dẫn có đầu lọc; đáng tin cậy nhưng có độ trễ thủy lực dài.
* **Piezometer khí nén (Pneumatic Piezometer)**: Màng cân bằng bởi áp lực khí qua hai ống; độ trễ ngắn, không đóng băng, nhưng phụ thuộc người vận hành.
* **Piezometer dây rung – VW (Vibrating-Wire Piezometer)**: Thiết bị màng cứng đọc theo sự thay đổi tần số dây; độ trễ ngắn và kết nối sẵn sàng với bộ ghi dữ liệu.
* **Piezometer nhiều điểm (Multipoint Piezometer)**: Một hố khoan chứa nhiều cảm biến để mô tả áp lực theo độ sâu.
* **Bàn lún (Settlement Platform)**: Bản mặt (thường có ống dẫn) ghi lún của nền đắp trong quá trình thi công.
* **Điểm lún dưới bề mặt (Subsurface Settlement Point)**: Neo đặt ở độ sâu (đóng/gắn vữa hoặc Borros) ghi lún của một tầng bị chôn.
* **Đo mực nước dạng ống (Liquid-Level Gage)**: Ống chứa chất lỏng nối với một tế bào, đo lún hoặc trương nở qua thay đổi áp lực hoặc mực chất lỏng.
* **Extensometer chuỗi (Series Extensometer)**: Một chồng neo trong một hố khoan, phân giải biến dạng thành gia số giữa các neo kề nhau.
* **Inclinometer ngang (Horizontal Inclinometer)**: Inclinometer di chuyển dọc ống vách nằm ngang để cho profile lún.
* **Inclinometer tại chỗ – cố định (In-Place Inclinometer)**: Một chuỗi cảm biến để lại trong ống vách để quan trắc liên tục, tự động.
* **Chỉ báo mặt trượt (Shear-Plane Indicator)**: Thiết bị phát hiện độ sâu mà ống vách inclinometer bị cắt.
* **Quan trắc phát xạ âm – AE (Acoustic Emission Monitoring)**: Phát hiện âm tần số cao sinh ra khi hạt đất/đá trượt và vỡ, làm cảnh báo sớm mất ổn định đang phát triển.
* **Tenzo Demec (Demec Gage)**: Tenzo cơ học gắn trên bề mặt, đo sự thay đổi khoảng cách giữa hai đĩa chuẩn.
* **Kích thủy lực đã hiệu chuẩn (Calibrated Hydraulic Jack)**: Kích có lỗ xuyên tâm dùng để căng và đo tải; phải được hiệu chuẩn vì số đọc áp lực chất lỏng mang sai số ma sát.
* **Tế bào áp lực đất tiếp xúc (Contact Earth Pressure Cell)**: Tế bào đo ứng suất hoặc tải tại mặt tiếp giáp đất–kết cấu, tại mũi cọc hoặc đáy cọc khoan.
* **Truyền tải (Load Transfer – móng sâu)**: Phân bố tải dọc trục giữa ma sát thành bên và sức kháng mũi, xác định từ tenzo, thanh chị em và telltale.
* **Gia cố nền (Ground Improvement)**: Cải tạo tính chất nền tại chỗ — bằng phụt vữa, đầm chặt hoặc thoát nước — để nền phù hợp cho xây dựng.
* **Nghiệm thu trước/sau lắp đặt (Acceptance Test)**: Phép kiểm xác nhận thiết bị đạt thông số kỹ thuật trước khi lắp và sống sót qua lắp đặt sau đó.
* **Biên bản lắp đặt (Installation Record Sheet)**: Hồ sơ hoàn công ghi vị trí, độ sâu, lớp bịt và các giá trị hiệu chuẩn đang áp dụng — hồ sơ vĩnh viễn giúp dữ liệu còn diễn giải được.
* **Đồ thị nhân–quả (Cause-and-Effect Plot)**: Đồ thị của thay đổi đo được so với một yếu tố ảnh hưởng (tải, mưa, chiều cao đắp) để bộc lộ quan hệ.
* **Triển khai (Implementation – mắt xích cuối)**: Hành động theo dữ liệu đã diễn giải — bước làm cho công tác quan trắc trở nên có ý nghĩa.

---

*Xem thêm: [English Technical Glossary](../../glossary/index.md) · [Ma trận Tuân thủ Nghị định 114 & TCVN 9398](../tuan-thu/nghi-dinh-114-tcvn-9398.md) · [Môi trường thử nghiệm tương tác](../visualizer.md)*
