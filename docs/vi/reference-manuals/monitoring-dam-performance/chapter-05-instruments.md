---
lang: vi
lang_alt: reference-manuals/monitoring-dam-performance/chapter-05-instruments/
---
# Chương 5 — Các Họ Thiết bị Quan trắc cho Đập

## 5.1 Một thực đơn các phép đo

Chương này khảo sát các họ thiết bị dùng để giám sát đập. Các chương sau đi sâu
hơn vào những họ quan trọng nhất đối với an toàn. Đối với các quy trình lắp đặt
chi tiết, xem các tài liệu [Dunnicliff](../dunnicliff/index.md) và [FHWA](../fhwa/index.md)
trong kho kiến thức này.

## 5.2 Các hạng mục đo lường

| Hạng mục | Đo cái gì | Thiết bị đại diện |
|----------|-----------------|----------------------------|
| **Mực nước / hồ chứa** | Cao độ mặt nước, mức | Thước vạch (staff gauges), cảm biến áp suất (pressure transducers), phao đo mức (float gauges) |
| **Áp lực lỗ rỗng / uplift** | Áp suất nước trong đất/đá/bê tông | Piezometer dây rung (vibrating-wire), khí nén (pneumatic), ống đứng (standpipe), thủy lực (hydraulic) |
| **Thấm / rò rỉ** | Lưu lượng & chất lượng dòng chảy | Wei (weirs), xô đong (tipping buckets), cảm biến độ đục (turbidity), quan sát |
| **Biến dạng — bề mặt** | Chuyển động bề mặt đập | Mốc khảo sát (survey monuments), GNSS, máy kinh vĩ điện tử (total station) |
| **Biến dạng — trong lòng** | Chuyển động bên trong thân đập/nền móng | Thiết bị đo nghiêng (inclinometer), thiết bị đo biến dạng sâu (extensometer), bàn đo lún, mảng SAA |
| **Kết cấu** | Nứt, mở khe, tải trọng | Cảm biến đo khe nứt (crackmeter), cảm biến đo khe nối (jointmeter), cảm biến đo tải trọng (load cell), cảm biến đo biến dạng (strain gauge) |
| **Môi trường** | Lượng mưa, nhiệt độ, khí quyển | Máy đo mưa, cảm biến nhiệt (thermistor), áp kế khí quyển (barometer) |
| **Bê tông / lão hóa** | Suy yếu, kiềm, ăn mòn | Đầu dò ăn mòn cốt thép, phát xạ âm (acoustic emission) |

## 5.3 Các công nghệ cảm biến

Thiết bị chuyển một đại lượng vật lý thành một tín hiệu có thể đọc. Các công nghệ
thường gặp:

- **Dây rung (Vibrating-Wire — VW)** — một sợi dây thép căng có tần số thay đổi theo biến dạng;
  bền bỉ, ổn định lâu dài, và là công nghệ chủ lực của quan trắc đập hiện đại.
- **Khí nén (Pneumatic)** — áp suất khí cân bằng áp suất đo; hữu ích nơi nguồn
  điện hoặc cáp kéo dài không khả thi.
- **Thủy lực (Hydraulic)** — áp suất cột chất lỏng; đơn giản và đã được chứng minh lâu đời.
- **Điện trở & cảm ứng** — biến trở (potentiometer), LVDT, và cảm biến đo biến dạng (strain gauge).
- **Áp điện & MEMS** — gia tốc kế (accelerometer), cảm biến đo độ nghiêng (tiltmeter), và các cảm biến MEMS hiện đại.

## 5.4 Thủ công so với tự động

- **Thi thủ công** được đọc tại hiện trường bằng một bộ đọc xách tay. Chi phí thấp,
  nhưng tần suất hạn chế và phơi nhân sự trước các điều kiện nguy hiểm.
- **Tự động** cung cấp dữ liệu cho bộ ghi dữ liệu (dataloggers) và viễn thông
  (telemetry), cho phép tần suất cao, truy cập từ xa và báo động ([Chương 9](chapter-09-automated.md)).

## 5.5 Độ chính xác, độ phân giải và dải đo

Ba khái niệm riêng biệt thường bị nhầm lẫn:

- **Độ chính xác (Accuracy)** — độ gần với giá trị thực (hiệu chuẩn quan trọng).
- **Độ phân giải (Resolution)** — thay đổi nhỏ nhất mà thiết bị có thể phát hiện.
- **Dải đo (Range)** — khoảng mà nó vẫn còn hợp lệ.

Một con đập có thể chỉ cần độ chính xác trung bình nhưng độ phân giải cao để phát
hiện các xu hướng chậm. Hãy quy định cả ba, và một ngân sách sai số thực tế.

## 5.6 Lựa chọn một họ thiết bị

Sự lựa chọn tuân theo bước lập kế hoạch: ghép thiết bị với chỉ báo, vị trí, nguồn
điện sẵn có, khả năng tiếp cận, tuổi thọ dự kiến và hệ thống dữ liệu. Sự dự phòng
tại các vị trí quan trọng nhất là thận trọng — nếu piezometer duy nhất bảo vệ một
hình thức hư hỏng bị hỏng, chương trình sẽ có một điểm mù.

![Figure: dam-monitoring-layout](../../../assets/figures/dam-monitoring-layout.svg)

**Hình.** Bố trí thiết bị điển hình trên đập đắp: khảo sát đỉnh đập, piezometer, extensometer, inclinometer, tầng thoát nước chân và trạm đo thấm (phạm vi ASCE MOP-135).

## 5.7 Các điểm chính cần nhớ

- Thiết bị thuộc về các họ mực nước, áp lực lỗ rỗng, thấm, biến dạng, kết cấu và môi trường.
- Cảm biến dây rung (vibrating-wire) là công cụ chủ lực hiện đại; khí nén và thủy lực vẫn hữu ích.
- Phân biệt độ chính xác, độ phân giải và dải đo — phát hiện xu hướng thường cần độ phân giải nhiều nhất.
- Ghép họ thiết bị với chỉ báo và môi trường đã lập kế hoạch; thêm dự phòng tại các điểm quan trọng.
