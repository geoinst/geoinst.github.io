---
lang: vi
lang_alt: reference-manuals/cfem/chapter-25-instrumentation-monitoring/
---
# Chương 25 — Quan trắc Địa kỹ thuật và Giám sát (Bản tổng hợp)

*Nguồn: CFEM 2022 (ấn bản 4), Chương 25, tác giả Pierre Choquet, Dr.-Eng., P. Eng.
Trang này là bản tổng hợp nguyên bản kèm **phần tham khảo được khai triển**; không
phải bản sao nguyên văn chương có bản quyền.*

Thiết kế địa kỹ thuật luôn gắn với độ không đảm bảo. Độ không đảm bảo ấy được đánh
giá trong giai đoạn thi công và vận hành nhờ các thiết bị quan trắc. Chương 25 khảo
sát những thiết bị thường dùng để giám sát ứng xử ngắn hạn và dài hạn của nền đất đỡ
các công trình do con người tạo ra, cùng các hệ thu thập dữ liệu đứng sau chúng.

Chương được tổ chức quanh **sáu đại lượng đo**, và bản tổng hợp này theo đúng cấu
trúc đó trước khi chuyển sang nửa *tự động* của chủ đề — cách lấy số đọc, truyền và
trình bày mà không cần người ra hiện trường.

---

## 25.1 — Giới thiệu

Sáu đại lượng quan trắc chính, và thiết bị đo chúng:

| Đại lượng | Thiết bị thường dùng |
|---|---|
| **Áp lực nước ngầm** | Áp kế (ống đứng, dây rung, khí nén, đóng ép, gắn vữa toàn phần) |
| **Chuyển vị** (bề mặt và theo chiều sâu; x, y, z; tương đối hoặc tuyệt đối) | Thiết bị đo biến dạng sâu, bàn đo lún, thiết bị đo nghiêng, cảm biến đo độ nghiêng, phương pháp trắc đạc |
| **Biến dạng** (trên mặt đất hay mặt kết cấu, hoặc nhúng trong kết cấu) | Cảm biến đo biến dạng |
| **Tải trọng** (từ cấu kiện xuống nền) | Cảm biến đo tải trọng (neo giữ, cọc thử) |
| **Áp lực tổng** (tiếp xúc đất – kết cấu) | Hộp đo áp lực đất |
| **Nhiệt độ** (bề mặt, hoặc phân bố theo chiều sâu) | Cảm biến nhiệt điện trở (thermistor) |

Chương cũng đề cập **phương pháp trắc đạc** — máy toàn đạc, đo cao, GPS RTK vi phân,
và các phương pháp mới hơn như LiDAR, InSAR đặt trên mặt đất và InSAR vệ tinh — vì
chúng thường dùng kèm thiết bị quan trắc địa kỹ thuật và kết cấu.

---

## 25.2 — Nguồn thông tin *(khai triển)*

> **Đây là mục biến chương này thành một công cụ tra cứu.** Không phải danh mục tài
> liệu thuần túy, §25.2 là một danh mục đọc *có dẫn dắt*, tổ chức theo loại tài liệu.
> Dưới đây, mỗi mục được phân nhóm và chú giải về nội dung cùng vai trò của nó.

### 25.2.1 — Giáo trình nền tảng

- ***Geotechnical Instrumentation for Monitoring Field Performance*** — **John
  Dunnicliff (1993)**, Wiley, 577 tr. — tác phẩm chuẩn mực của ngành, được biết đến
  rộng rãi với tên **"Sách Đỏ"**. Chương 25 coi đây là nguồn được thừa nhận nhất
  trong lĩnh vực.
- **Chuyên mục định kỳ của Dunnicliff** trên tạp chí *Geotechnical News* (CGS) — 93
  chuyên mục, được lập chỉ mục và cho phép tra cứu trong phần công khai của
  [trang web CGS](https://www.cgs.ca/instrumentation_news.html). Một kho lưu trữ thực
  hành nối tiếp cuốn sách.

### 25.2.2 — Giáo trình và các sổ tay hướng dẫn chính

| Tài liệu | Nội dung |
|---|---|
| **De Rubertis, K. (chủ biên), 2018** — *Monitoring Dam Performance: Instrumentation and Measurements*, ASCE, 442 tr. | Nguồn chính của chương về **đặc tính đo lường** (§25.5) và quan trắc trắc đạc; tài liệu an toàn đập của ASCE/USSD |
| **Sharon, R. & Eberhardt, E. (chủ biên), 2020** — *Guidelines for Slope Performance Monitoring*, CSIRO Publishing / CRC Press, 331 tr. | Triết lý và thực hành quan trắc riêng cho mái dốc |
| **Stark, Oommen & Ning, 2021** — *Remote Sensing for Monitoring Embankments, Dams, and Slopes*, ASCE GSP 322, 114 tr. | Hiện trạng thực hành viễn thám (InSAR, LiDAR, quang trắc) |
| **ICE Manual of Geotechnical Engineering** (Burland và cs., 2012) — Ch. 94 *Principles of Geotechnical Monitoring* (16 tr.) và Ch. 95 *Types of Geotechnical Instrumentation and Their Usage* (26 tr.) | Một cách trình bày kinh điển thứ hai; Ch. 94 cũng bàn về thực hành hợp đồng |
| **Walker & Awange, 2020** — *Surveying for Civil and Mine Engineers*, Springer, 411 tr. | Phương pháp trắc đạc/đo đạc (§25.17) |
| **Glisic & Inaudi, 2007** — *Fibre Optic Methods for Structural Health Monitoring*, Wiley, 281 tr. | Tài liệu tham chiếu cho **cảm biến quang** (§25.4.4) |
| **Ferretti và cs., 2007** — *InSAR Principles: Guidelines for SAR Interferometry Processing*, ESA TM-19 | Nguyên lý đằng sau **InSAR vệ tinh** (§25.17.5) |
| **Chartered Institution of Civil Engineering Surveyors, 2017** — *Client Guide to Instrumentation and Monitoring*, Survey Liaison Group, London, 28 tr. | Hướng dẫn phía chủ đầu tư về mua sắm và phạm vi công việc |

### 25.2.3 — Tiêu chuẩn

**Tiểu ban ASTM D18.23 (Thiết bị hiện trường)** — các phương pháp thử và thực hành
tiêu chuẩn Hoa Kỳ điều chỉnh trực tiếp từng thiết bị:

| Tiêu chuẩn | Nội dung |
|---|---|
| **D4403-20** | Thực hành tiêu chuẩn cho thiết bị đo biến dạng sâu dùng trong đá |
| **D6230-13** | Phương pháp thử tiêu chuẩn để giám sát chuyển dịch nền bằng thiết bị đo nghiêng kiểu đầu dò |
| **D6598-19** | Hướng dẫn tiêu chuẩn lắp đặt và vận hành mốc đo lún để giám sát biến dạng đứng |
| **D7299-12** | Thực hành tiêu chuẩn kiểm tra hiệu năng đầu dò đo nghiêng đứng |
| **D7764-12** | Thực hành tiêu chuẩn nghiệm thu trước lắp đặt áp kế dây rung |

**Ủy ban Kỹ thuật ISO TC 182 / WG2 — bộ *ISO 18674*** ("Geotechnical investigation
and testing — Geotechnical monitoring by field instrumentation"), đối tác quốc tế
tương ứng, xuất bản theo từng phần:

| Phần | Nội dung | Trạng thái tại thời điểm biên soạn |
|---|---|---|
| **ISO 18674-1:2015** | Phần 1: Quy tắc chung | Đã ban hành |
| **ISO 18674-2:2016** | Phần 2: Đo dọc tuyến — thiết bị đo biến dạng sâu | Đã ban hành |
| **ISO 18674-3:2017** | Phần 3: Đo ngang tuyến — thiết bị đo nghiêng | Đã ban hành |
| **ISO 18674-4** | Phần 4: Đo áp lực nước lỗ rỗng — áp kế | Đã ban hành |
| **ISO 18674-5** | Phần 5: Đo thay đổi ứng suất bằng hộp đo áp lực tổng | Đã ban hành |
| Phần 6 / 7 / 8 / 9 | Bàn đo lún thuỷ lực / cảm biến đo biến dạng / cảm biến đo tải trọng / thiết bị quan trắc trắc đạc | **Dự kiến** |

**DIN (Deutsches Institut für Normung)** — tiêu chuẩn rung động được dẫn cho §25.19:

- **DIN 45669-1:1995** — Đo rung động và xung kích cơ học
- **DIN 4150-1:2001** — Rung động kết cấu, Phần 1: dự báo các tham số rung động
- **DIN 4150-2:1999** — Ảnh hưởng của rung động lên người trong nhà *(đang soát xét)*
- **DIN 4150-3:2016** — Rung động trong nhà, Phần 3: ảnh hưởng lên kết cấu

**Tiêu chuẩn và hướng dẫn của cơ quan khác:**

- **Transportation Research Board (TRB), 2008** — *Use of Inclinometers for
  Geotechnical Instrumentation on Transportation Projects* (Machan & Bennett) — một
  ghi chú kỹ thuật toàn diện về thực hành thiết bị đo nghiêng.
- **USGS, 2008** — *Instrumentation Guidelines for the Advanced National Seismic
  System (ANSS)*, Open-File Report 2008–1262, 48 tr. — nguồn của **phân loại hệ
  đo rung động mạnh theo lớp A–D** dùng ở §25.18.
- **COSMOS, 2016** — *Guidelines and General Considerations for Strong-Motion
  Instrumentation of Tall Buildings* — hướng dẫn đo rung động mạnh cho nhà cao tầng.
- **US Bureau of Mines RI 8507, 1980** (Siskind và cs.) — *Structure Response and
  Damage by Ground Vibration from Mine Blasting* — tài liệu tham chiếu kinh điển về
  rung động do nổ mìn, nền tảng của §25.19.

### 25.2.4 — Sổ tay quy định (an toàn đập)

Danh mục **hướng dẫn quan trắc an toàn đập cho phép tải về** của chương — những sổ
tay quy định mà một chương trình quan trắc cuối cùng phải chịu trách nhiệm trước:

| Sổ tay | Đơn vị / năm | Số trang |
|---|---|---|
| **EM 1110-2-1908** — *Instrumentation of Embankment Dams and Levees* | Công binh Lục quân Hoa Kỳ (USACE), 2020 | 290 tr. |
| **EM 1110-2-4300** — *Instrumentation for Concrete Structures* | USACE, 1987 *(đang soát xét)* | 306 tr. |
| *Embankment Dam Instrumentation Manual* (Bartholomew, Murray & Goins) | Cục Khai hoang Hoa Kỳ (Reclamation), 1987 *(đang soát xét)* | 269 tr. |
| *Concrete Dam Instrumentation Manual* (Bartholomew & Haverland) | Reclamation, 1987 | 153 tr. |
| *Engineering Guidelines for the Evaluation of Hydropower Projects*, Ch. 9 *Instrumentation and Monitoring* (2005); Ch. 14 *Dam Safety Performance Monitoring Program* (2017) | FERC | 86 / 188 tr. |
| **ICOLD Bulletin 158** — *Dam Surveillance Guide* (2018) | ICOLD | 109 tr. |
| **7 Sách trắng** về Xây dựng và Triển khai Chương trình Giám sát An toàn Đập (2008–2020) | Hội Đập Hoa Kỳ (USSD) | bộ |
| *Manual de Mecánica de Suelos: Instrumentación y Monitoreo del Comportamiento de Obras Hidráulicas* (2012) | Comisión Nacional del Agua, Mexico | 322 tr. |

> **Liên kết chéo.** Trang này tổng hợp trực tiếp một số tài liệu trên — xem
> [Giám sát hiệu năng đập](../monitoring-dam-performance/index.md) (ASCE MOP-135) và
> [An toàn đập thải](../tailings-dam-safety/index.md) (ICOLD Bulletin 194).

### 25.2.5 — Chuỗi hội thảo

Nghiên cứu quan trắc toàn diện được công bố qua chuỗi hội thảo **"Field Measurements
in Geomechanics" (FMGM)**: Zurich 1983, Kobe 1987, Oslo 1991, Bergamo 1995, Singapore
1999, Oslo 2003, Boston 2007, Berlin 2011, Sydney 2015 và Rio de Janeiro 2018 — do các
tình nguyện viên (phần lớn là học giả) tổ chức và các nhà xuất bản thương mại ấn hành.
Hội thảo kế tiếp dự kiến tại London năm 2022 dưới bảo trợ của ISSMGE. Kỷ yếu các hội
thảo này là nơi **các ca nghiên cứu** (case history) quan trắc được báo cáo chi tiết.

---

## 25.3 — Yếu tố con người

Chương 25 dành sự chú ý sớm cho **yếu tố con người**, dựa trên ba chương của
Dunnicliff: lập kế hoạch có hệ thống, đặc tả mua sắm, và thoả thuận hợp đồng. Luận
điểm của chương vẫn còn nguyên giá trị: thiết bị cơ học/thuỷ lực đơn giản từng hoạt
động tốt trong tay những kỹ sư tận tâm, có mục đích rõ ràng; khi công nghệ tiến bộ,
"ngày càng nhiều chương trình quan trắc nằm trong tay những người thiếu động lực và
thiếu mục đích," và nhiều thất bại trở thành **thất bại của sự kết hợp giữa thiết bị
và con người** chứ không phải của thiết bị. Dù viết đã nhiều thập kỷ, chương lưu ý
điểm này *"nay còn đúng hơn nữa"* do nhịp độ thi công ngày càng nhanh.

---

## 25.4 — Nguyên lý đo

Thiết bị địa kỹ thuật dựa trên các nguyên lý **điện, cơ, thuỷ lực và khí nén**. Hai
nguyên lý *điện* chủ đạo:

- **Dây rung (vibrating wire)** — phổ biến nhất. Một dây thép căng trước (đường kính
  thường **0,25 mm**, dài 5–15 cm) được kích thích bằng hai cuộn dây điện từ; dây dao
  động ở tần số (**1.000–2.000 Hz**) biến đổi theo lực căng. Được khẳng định ở các đập
  bê tông châu Âu sau Thế chiến II nhờ độ bền và độ ổn định dài hạn; nay bao phủ áp
  lực nước lỗ rỗng, độ lún, giãn/nén, biến dạng, tải trọng, ứng suất và áp lực đất.
  Nhiệt độ thường được tích hợp sẵn qua một thermistor kín.
- **Cảm biến gia tốc MEMS** — thay thế gia tốc kế servo và cảm biến nghiêng điện phân
  khoảng năm 2010 cho **độ nghiêng**, với đặc tính đo tương đương hoặc tốt hơn, cộng
  thêm độ bền và đặc tính bù nhiệt tốt hơn. Mạch điện có thể gồm vi điều khiển và bộ
  chuyển đổi tương tự – số, cho **đầu ra số** trên bus RS-485.
- **Thiết bị đầu ra số** (một họ liên quan) — cảm biến mực nước kiểu điện trở áp với
  đầu ra 4–20 mA, đầu dò chất lượng nước đa thông số, và chuỗi thermistor số, dùng
  giao thức **RS-485** hoặc **SDI-12** do USGS phát triển.
- **Cảm biến quang** — miễn nhiễm với sét và quá độ điện; có loại điểm, **bán phân
  tán** (cách tử Bragg) và **phân tán toàn phần** (tán xạ Brillouin, đo biến dạng/nhiệt
  độ mỗi mét trên cáp dài tới **30 km**).

---

## 25.5 — Đặc tính đo lường

Vì thiết bị thường **không thể thay thế** sau khi lắp, yêu cầu về đặc tính đo lường rất
cao. Các đặc tính (theo De Rubertis, 2018), kèm giá trị điển hình của dây rung:

| Đặc tính | Ý nghĩa | Giá trị điển hình (dây rung) |
|---|---|---|
| **Độ phân giải** | Thay đổi nhỏ nhất phân biệt được | Mịn hơn độ chính xác nhiều lần |
| **Độ chính xác** | Mức khớp với một chuẩn được chấp nhận | **±0,1 % F.S.** (truy nguyên NIST) |
| **Độ chụm** (sai số ngẫu nhiên) | Độ gần nhau của các số đọc lặp lại | **±0,025 % F.S.** |
| **Độ lặp lại** | Mức đồng thuận của các đo liên tiếp | Bằng độ chụm (dây rung) |
| **Độ tuyến tính** (phi tuyến) | Mức lệch khỏi đường thẳng | **0,1–0,5 % F.S.** |
| **Độ chệch** | Giá trị chỉ báo trung bình so với giá trị thực | Bằng độ chính xác (thực tế) |
| **Độ ổn định dài hạn** | Trôi đầu ra qua nhiều năm ở đầu vào không đổi | Xác lập qua nhiều ca nghiên cứu hàng thập kỷ |

Điểm cốt lõi của chương với công tác quan trắc: **điều cần quan tâm thường là sự thay
đổi, không phải giá trị tuyệt đối** — điều này khiến *độ chụm* quan trọng hơn độ
chính xác.

---

## 25.6–25.7 — Tĩnh và động; chuỗi thiết bị

**Quan trắc tĩnh** chiếm ưu thế trong địa kỹ thuật (nền đất ứng xử chậm), còn **quan
trắc động** bao gồm động đất, nổ mìn và rung động máy. Thuật ngữ được làm rõ dọc chuỗi:
**cảm biến → đầu chuyển đổi → bộ phát → thiết bị**, một phân biệt mà chương dùng nhất
quán ở các mục sau.

---

## 25.8 — Áp lực nước ngầm (áp kế)

Mục dài nhất về thiết bị của chương, bao gồm:

- **Áp kế ống đứng Casagrande** — chuẩn mực đơn giản, bền bỉ.
- **Đầu chuyển đổi áp lực điện** — loại dây rung và các loại khác.
- **Áp kế dây rung trong ống đứng Casagrande** — kiểu lắp ghép hỗn hợp.
- **Lắp đặt phân vùng** trong hố khoan — cô lập vùng đo bằng nút vữa.
- **Áp kế đóng ép** — triển khai nhanh khi nền cho phép.
- **Áp kế gắn vữa toàn phần** — phương pháp (với các tham chiếu Contreras, Mikkelsen,
  McKenna, Vaughan, Penman trong danh mục) đã trở thành chuẩn cho nhiều công trình
  đập đất.
- **Áp lực nước lỗ rỗng âm / độ hút** — phép đo khó nhất, có kỹ thuật riêng.

---

## 25.9 — Độ nghiêng

- **Cảm biến đo độ nghiêng** — cho kết cấu và độ nghiêng cục bộ.
- **Thiết bị đo nghiêng** — công cụ chủ lực cho chuyển dịch ngang của nền, đọc theo
  bước cố định (ví dụ 0,5 m / 2 ft) với hệ đầu dò.
- **Thiết bị đo nghiêng cố định và ShapeArray** — biên dạng lắp đặt vĩnh viễn, với
  chương nêu **các lưu ý chọn lựa** cho từng loại (§25.9.3.1–25.9.3.2).

---

## 25.10 — Độ lún, độ trương và lún lệch

Các thiết bị: **thiết bị đo biến dạng sâu kiểu đầu dò**, **thiết bị đo biến dạng sâu
trong hố khoan**, **bàn đo lún thuỷ lực**, **bàn đo lún thuỷ lực vi phân**, và **thiết
bị đo nghiêng ngang** — bao quát từ độ lún bề mặt đến độ trương sâu.

---

## 25.11–25.14 — Khe nứt, biến dạng/tải trọng, áp lực đất, nhiệt độ

- **Khe nứt và khe nối** — cảm biến đo khe nứt, cảm biến đo khe nối, thiết bị đo biến
  dạng sâu trong đất.
- **Biến dạng và tải trọng** — cảm biến đo biến dạng, cảm biến đo tải trọng (bê tông,
  thép, neo).
- **Áp lực đất** — hộp đo áp lực tổng, hộp đo áp lực đất đóng ép.
- **Nhiệt độ** — thermistor và chuỗi thermistor (cũng là đại lượng tham chiếu để bù cho
  nhiều thiết bị khác).

---

## 25.15 — Thu thập dữ liệu tự động và truyền dẫn

**ADAS (Hệ thống thu thập dữ liệu tự động)** là thiết bị điện tử triển khai tại hiện
trường, thu và lưu số đo từ nhiều cảm biến qua cáp hoặc sóng vô tuyến, và tuỳ chọn
truyền về máy tính từ xa không cần can thiệp của con người. Các tính năng yêu cầu:

- **Quản lý tín hiệu** cho nhiều loại cảm biến (dây rung, MEMS số, 4–20 mA, đầu ra
  tương tự 0–5/0–10 V, số RS-485/SDI-12).
- **Nguồn pin** (kiềm, lithium, hoặc ắc-quy chì + tấm pin mặt trời).
- **Bộ nhớ lưu dữ liệu** tại thiết bị hiện trường.
- **Truyền thông băng thông thấp** — vô tuyến, modem di động hoặc vệ tinh, theo lịch.
- **Khả năng báo động/điều khiển cục bộ** (tuỳ chọn).
- Một dải liên tục từ **bộ ghi độc lập 1 kênh đến mạng 1.000+ kênh**.

Chương phân biệt **bộ ghi dữ liệu** (một thiết bị mang toàn bộ/hầu hết tính năng) với
**ADAS** (bộ ghi tinh vi có thể tạo thành **mạng**, quản lý điều kiện báo động, và
**điều khiển thiết bị ngoài** — SMS, van, còi/đèn nháy). *Lưu ý xu hướng thị trường:*
các bộ ghi nhỏ nay mang những tính năng từng chỉ có trong mạng ADAS.

**Bộ ghi nhỏ** (§25.15.1) — 1–10 kênh, công suất thấp, pin "D" 3,6 V cho **thời gian
tự chủ ≥1 năm**, dải nhiệt độ hoạt động **−40 °C đến +80 °C**, và ngày càng có chip vô
tuyến miễn phí giấy phép công suất thấp (vài km ở địa hình thoáng, ~1 km đô thị).

**Mạng ADAS tích hợp** (§25.15.2) — hai kiến trúc:

1. **Vài hệ thu thập trung tâm + đường cáp dài** — nhược điểm: chi phí cáp, đào rãnh/
   ống bảo vệ, **nguy cơ quá độ do sét gần mặt đất**, tăng điện trở, và rủi ro sai số
   tại mối nối. Khuyến nghị của chương rất rõ: **giữ cáp cảm biến ngắn** và tăng số
   điểm thu thập.
2. **Mạng vô tuyến hub-to-node** dùng bộ ghi nhỏ có vô tuyến đặt gần thiết bị — cấu
   hình **hình sao** hoặc **mạng lưới (mesh)** nơi các bộ ghi chuyển tiếp cho nhau tới
   một **gateway**, rồi về văn phòng qua di động, vệ tinh, Wi-Fi hoặc LAN.

---

## 25.16 — Phần mềm quản lý, trực quan hoá, báo động và báo cáo

Hầu hết bộ ghi/ADAS xuất **tệp giá trị phân cách** (`*.csv`, `*.dat`) với cột dấu thời
gian và một cột mỗi kênh — thường là số đọc **thô**, mà hầu hết người dùng muốn giữ.
Bảng tính đủ cho việc nhỏ; dự án lớn hơn hoặc dài hơn cần phần mềm chuyên dụng, thường
có:

- **Bảng điều khiển** (tổng quan dự án, giá trị thời gian thực, cảm biến đang báo động)
- **Hiển thị thời gian thực** với mã màu (**Xanh: OK / Vàng: ngưỡng / Đỏ: báo động**)
- **Đường xu hướng** (số đọc theo thời gian, có cuộn và thu phóng)
- **Báo động** kiểm tra ngưỡng với **SMS/email** tự động
- **Biến ảo** (tính từ một hay nhiều cảm biến)
- **Kiểm soát truy cập** (hồ sơ người dùng)
- **Bộ chuyển đổi tệp** (nhập từ hầu hết hệ ghi, bảng tính, ghi thủ công)
- **Đồ thị tương quan (XY)** (ví dụ mực nước áp kế vs mưa; biến dạng vs nhiệt độ)
- **Xem biên dạng** (thiết bị đo nghiêng cố định, ShapeArray)
- **Báo cáo tự động** theo lịch
- **Xem trên điện thoại/máy tính bảng** và **lưu trữ đám mây**
- **Đa ngôn ngữ**
- **Nhập dữ liệu trắc đạc (máy toàn đạc) và InSAR**
- **GIS / Google Earth** định vị cảm biến

---

## 25.17 — Đo đạc trắc đạc

Phương pháp đo đạc mặt đất phát hiện chuyển dịch ngang và đứng trên một **lưới khống
chế trắc đạc** gồm mốc hoặc điểm gắn trên kết cấu:

- **Máy toàn đạc và máy thuỷ bình** — thiết bị đo đạc cốt lõi; chế độ robot, không cần
  gương và nhận mục tiêu tự động cho phép vận hành **tự động**. Độ chính xác điển hình:
  **1–5 giây cung** về góc; **1–1,5 mm + 1–2 ppm** về khoảng cách.
- **Laser quay** — cho căn chỉnh và độ dốc.
- **Máy quét laser** — thu nhận 3D mật độ cao (xem Adamson và cs., 2019, trong danh mục).
- **GNSS** — định vị tuyệt đối.
- **InSAR vệ tinh** — so sánh ảnh SAR lặp lại; băng X, C và L; **kích thước pixel
  0,25–20 m** (phổ biến 1–3 m), **độ chính xác 1–20 mm**; **>50.000 điểm/km²** trên
  diện tích vượt hàng trăm km²; đo dọc tia radar (≈50–70° so với phương ngang), nên
  chuyển vị đứng thực phải tính bằng lượng giác; chu kỳ lặp **vài ngày đến 14+ ngày**.
  Chòm sao bay lên + bay xuống bổ sung thông tin ngang.
- **InSAR đặt trên mặt đất** — giao thoa radar mặt đất cho vùng phủ cục bộ.
- **Quang trắc UAV** — khảo sát trên không để phát hiện biến dạng (xem Stafford và cs., 2019).

---

## 25.18–25.19 — Rung động mạnh và rung động

- **Máy đo rung động mạnh** — gia tốc kế 3D + bộ ghi, thu **gia tốc hạt đỉnh** (đơn vị
  *g*) và lịch sử thời gian. Thực hành tốt nhất: một thiết bị ở **vùng tự do**, cộng một
  thiết bị ở **điểm cao nhất** của kết cấu và các vị trí trung gian, **đồng bộ GPS** khi
  dùng nhiều thiết bị. Phân loại **A–D** theo **USGS (2008)** cho mạng ANSS; Canada vận
  hành **CNSN** (100+ địa chấn kế độ lợi cao, 60+ máy đo gia tốc).
- **Máy đo rung động** — cảm biến vận tốc ba trục (**geophone**) + bộ ghi, đo **vận tốc
  hạt tính bằng cm/s** (nổ mìn, giao thông, rung động nền — điều chỉnh bởi chuỗi DIN 4150).

---

## 25.20 — Trình bày dữ liệu quan trắc

Luận điểm khép chương: **mọi dữ liệu phải chung một dấu thời gian**, và dấu thời gian
ấy là **mối liên kết duy nhất** giữa dữ liệu quan trắc và hoạt động thi công (vốn dỡ
tải rồi gia tải lại nền). Các yếu tố môi trường — **nhiệt độ và lượng mưa** — cũng phải
được ghi lại, vì việc dỡ tải có thể mở ra các khe nứt mà nước mưa khai thác (Hình
25-23). Việc tích hợp dữ liệu quan trắc với hoạt động thi công và yếu tố môi trường
**vẫn là thách thức với hầu hết phần mềm vẽ đồ thị thương mại** — và bất kỳ chương
trình quan trắc nào cũng phải **phân bổ nguồn lực thoả đáng** để dữ liệu được trình
bày và diễn giải không mập mờ.

---

## Các điểm then chốt

- **Sáu đại lượng, một kỷ luật.** Áp lực nước ngầm, chuyển vị, biến dạng, tải trọng,
  áp lực tổng và nhiệt độ — mỗi đại lượng có những họ thiết bị riêng.
- **§25.2 là tài sản tái sử dụng được nhiều nhất của chương** — một bản đồ dẫn dắt về
  các tiêu chuẩn (ASTM D18.23, ISO 18674, DIN 4150), giáo trình (Dunnicliff, De
  Rubertis, Sharon & Eberhardt, Hoek), sổ tay quy định (USACE, Reclamation, FERC,
  ICOLD) và hội thảo đứng sau thực hành quan trắc.
- **Dây rung và MEMS chiếm ưu thế** trong đo điện; cảm biến quang là họ thứ ba đang nổi lên.
- **Độ chụm quan trọng hơn độ chính xác** trong quan trắc, vì *sự thay đổi* mới là điều
  cần quan tâm.
- **Giữ cáp cảm biến ngắn và phân tán điểm thu thập** — đường cáp dài trên mặt đất mời
  gọi hư hỏng do sét và sai số mối nối.
- **Tự động hoá là một dải phổ**, từ bộ ghi 1 kênh đến mạng ADAS 1.000+ kênh có báo
  động và điều khiển.
- **Gắn dấu thời gian cho mọi thứ, và ghi cả nhiệt độ lẫn lượng mưa** — nếu không thì
  dữ liệu không thể diễn giải theo hoạt động thi công.
- **Yếu tố con người quyết định thành công.** Sự kết hợp thiết bị – con người quan
  trọng ngang với bản thân thiết bị.

---

## Danh mục tham chiếu đầy đủ

*Sao lục theo thư mục tài liệu tham chiếu của chương, để tra cứu. Các tiêu chuẩn được
soát xét theo chu kỳ riêng — hãy kiểm tra ấn bản hiện hành.*

**Adamson, D., Alfaro, M., Blatz, J., Bannister, K.** — Construction and Post-Construction Deformations of an MSE Wall using Terrestrial Laser Scanning. *Geo St John's 2019*, Hội Địa kỹ thuật Canada.

**Anderson, C., Vessely, M., Christiansen, C., 2020** — Advances in Unstable Slope Instrumentation and Monitoring. TRB / NCHRP, National Academies, Washington DC.

**Burland, J., Chapman, T., Skinner, H., Brown, M. (chủ biên), 2012** — *ICE Manual of Geotechnical Engineering*, Ch. 94 (Dunnicliff, Marr & Standing) và Ch. 95 (Dunnicliff). ICE Publishing, London.

**Choquet, P., Juneau, F., Debreuille, P.J., Bessette, J., 1999** — Reliability, Long-term Stability and Gage Performance of Vibrating Wire Sensors with Reference to Case Histories. *Proc. 5th Int. Symp. on Field Measurements in Geomechanics*, Singapore.

**Choquet, P., Taylor, R.M., 2014** — Automatic Data Acquisition Systems (ADAS) for Dam and Levee Monitoring. *Geo-Congress 2014*, ASCE, 180–191.

**Client guide to instrumentation and monitoring**, 2017 — Chartered Institution of Civil Engineering Surveyors for the Survey Liaison Group, London.

**Contreras, I.A., Grosser, A.T., VerStrate, R.H., 2007** — The use of the fully-grouted method for piezometer installation. *Proc. 7th Int. Symp. on Field Measurements in Geomechanics*, Boston. *(Xem thêm các bản cập nhật 2008, 2011, 2012 và 2020 của cùng nhóm tác giả.)*

**COSMOS, 2016** — *Guidelines and General Considerations for Strong-Motion Instrumentation of Tall Buildings*.

**De Rubertis, K. (chủ biên), 2018** — *Monitoring Dam Performance — Instrumentation and Measurements*, ASCE, 442 tr.

**DIN** — DIN 45669-1:1995; DIN 4150-1:2001; DIN 4150-2:1999 (đang soát xét); DIN 4150-3:2016.

**Dunnicliff, J., 1993** — *Geotechnical Instrumentation for Monitoring Field Performance*, Wiley, 577 tr.

**Dunnicliff, J., 1994** — Contract Practices for Geotechnical Instrumentation. *Geotechnical News*, Tập 12, Số 3.

**Elwood, D.E.Y. & Martin, C.D., 2016** — Ground response of closely spaced twin tunnels constructed in heavily overconsolidated soils. *Tunnelling and Underground Space Technology*, 51, 226–237.

**Ferretti, A., Monti-Guarnieri, A., Prati, C., Rocca, F., 2007** — *InSAR Principles: Guidelines for SAR Interferometry Processing and Interpretation*. ESA TM-19.

**Glisic, B., Inaudi, D., 2007** — *Fibre Optic Methods for Structural Health Monitoring*, Wiley, 281 tr.

**McKenna, G.T., 1995** — Grouted-in Installation of Piezometers in Boreholes. *Canadian Geotechnical Journal* 32, 355–363.

**McRae, J.B., Simmonds, T., 1991** — Long-term Stability of Vibrating-wire Instruments: One Manufacturer's Perspective. *Proc. 3rd Int. Symp. on Field Measurements in Geomechanics*, Tập 1:283–293, Balkema.

**Mikkelsen, P.E., 2002** — Cement-Bentonite Grout Backfill for Borehole Instruments. *Geotechnical News*, Tập 20, Số 4, 38–42.

**Mikkelsen, P.E. & Green, E.G., 2003** — Piezometers in Fully Grouted Boreholes. *6th Int. Symp. on Field Measurements in Geomechanics*, Oslo.

**Pantony, B., Fraser, S., Sinacori, J., 2021** — Satellite InSAR for Geotechnical and Structural Monitoring. *Canadian Geotechnique*, Tập 2, Số 1.

**Penman, A.D.M., 2002** — Measurement of Pore Water Pressures in Embankment Dams. *Geotechnical News*, Tập 20, Số 4, 43–49.

**Pieraccini, M., Miccinesi, L., 2019** — Ground-Based Radar Interferometry: A Bibliographic Review. *Remote Sensing* 11(9).

**Richards, D.J., Clark, J., Powrie, W., Heymann, G., 2007** — Performance of push-in pressure cells in overconsolidated clay. *Geotechnical Engineering* 160, GE1, 31–41.

**Richards, D.J., Powrie, W., Roscoe, H., Clark, J., 2007** — Pore water pressure and horizontal stress changes during construction of a contiguous bored pile multi-propped retaining wall in Lower Cretaceous clays. *Géotechnique* 57(2), 197–205.

**Ridley, A.M., 2015** — Soil suction — what it is and how to successfully measure it. *9th Symp. on Field Measurements in Geomechanics*, Australian Centre for Geomechanics, Perth, 27–46.

**Schuyler, J.N. & Gularte, F., 2000** — Automated Tiltmeter Monitoring of Bridge Response to Compaction Grouting. *SPIE 7th Annual Int. Symp. on Smart Structures and Materials*, Newport Beach, CA.

**Sellers, J.B., 1994** — Load Cell Calibrations. *Geotechnical News*, Tập 12, Số 3.

**Sellers, J.B., Taylor, R., 2008** — MEMS Basics. *Geotechnical News*, Tập 26, Số 1.

**Sharon, R., Eberhardt, E. (chủ biên), 2020** — *Guidelines for Slope Performance Monitoring*, CSIRO Publishing / CRC Press, 331 tr.

**Siskind, D.E., Stagg, M.S., Kopp, J.W., Dowding, C.H., 1980** — *Structure Response and Damage by Ground Vibration from Mine Blasting*. US Bureau of Mines RI 8507.

**Soe Moe, K.W., Cruden, D.M., Martin, C.D., Lewycky, D., Lach, P.R., 2009** — Mechanisms and kinematics of river valley landslides in Edmonton. *Annual Canadian Geotechnical Conference, GeoHalifax*.

**Stafford, D.M.J. và cs., 2019** — Preliminary deformation detection of high-fill sections along the Inuvik-Tuktoyaktuk Highway using UAV photogrammetry. *Geo St. John's 2019*, CGS.

**Stark, T.D., Oommen, T., Ning, Z., 2021** — *Remote Sensing for Monitoring Embankments, Dams, and Slopes: Recent Advances*, ASCE GSP 322, 114 tr.

**Tedd, P., Powell, J.J., Charles, J.A., Uglow, I.M., 1990** — In situ measurement of earth pressures using push-in spade-shaped pressure cells — 10 years' experience. *Geotechnical Instrumentation in Practice*, Thomas Telford, London, 701–715.

**U.S. Geological Survey, 2008** — *Instrumentation Guidelines for the Advanced National Seismic System*. Open-File Report 2008–1262, 48 tr.

**Vaughan, P.R., 1969** — A Note on Sealing Piezometers in Boreholes. *Géotechnique* 19(3), 405–413.

**Walker, J. & Awange, J.L., 2020** — *Surveying for Civil and Mine Engineers*, Springer, 411 tr.

> **Lời cảm ơn (chương gốc).** Tác giả chương cảm ơn các nhà cung cấp thiết bị quan
> trắc đã cung cấp hình vẽ và ảnh cho ấn phẩm gốc. Những hình ấy **không** được tái bản
> ở đây.
