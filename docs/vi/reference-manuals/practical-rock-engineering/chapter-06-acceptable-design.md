---
lang: vi
lang_alt: reference-manuals/practical-rock-engineering/chapter-06-acceptable-design/
---

# Chương 6 — Khi Nào Một Thiết Kế Cơ Học Đá Là Chấp Nhận Được?

## 6.1 Ngụy Biện Của Một Con Số Hệ Số An Toàn Duy Nhất

Trong tính toán kết cấu thép hay bê tông cốt thép truyền thống, một hệ số an toàn đơn định ($FS$) từ $1,5$ đến $2,0$ bảo đảm độ an toàn gần như tuyệt đối vì các vật liệu này được sản xuất công nghiệp với quy trình kiểm chuẩn khắt khe có hệ số biến động rất nhỏ ($COV < 10\%$).

Tuy nhiên, trong địa kỹ thuật và cơ học đá:
- Các thông số khối đá có độ phân tán không gian cực kỳ lớn (hệ số biến thiên $COV$ của cường độ đá nguyên vẹn thường là $20 - 40\%$; độ phát triển khe nứt và GSI thường là $15 - 35\%$).
- Một bờ dốc mỏ có hệ số an toàn đơn định tính theo giá trị trung bình $FS = 1,3$ hoàn toàn có thể có **xác suất phá hoại ($P_f$) vượt quá $20\%$** nếu độ lệch chuẩn của góc ma sát khe nứt hoặc áp lực nước ngầm quá lớn.
- Ngược lại, một mái dốc có $FS = 1,15$ nhưng độ không đảm bảo địa kỹ thuật được khống chế rất chặt chẽ lại có thể có $P_f < 1\%$.

**Một con số hệ số an toàn đơn định thuần túy là vô nghĩa nếu không gắn liền với mức độ không đảm bảo của số liệu đầu vào và hậu quả rủi ro khi công trình bị phá hoại.**

---

## 6.2 Hệ Số An Toàn Đơn Định ($FS$) Đối Chiếu Xác Suất Phá Hoại ($P_f$)

```
             SỨC KHÁNG R (Khả năng chịu lực)
                 \       /
                  \     /
                   \   /
                    \ /
                     X  <--- VÙNG GIAO NHAU: Xác suất phá hoại Pf
                    / \
                   /   \
                  /     \
                 /       \
             TẢI TRỌNG TÁC ĐỘNG S
```

1. **Biên An Toàn Đơn Định**:

$$FS = \frac{\text{Sức kháng trung bình } \bar{R}}{\text{Tải trọng trung bình } \bar{S}} = \frac{\sum \text{Lực giữ chống trượt}}{\sum \text{Lực gây trượt}}$$

2. **Chỉ Số Độ Tin Cậy ($\beta$)**:
   Giả thiết sức kháng $R$ và tải trọng $S$ tuân theo hàm phân phối chuẩn:

$$\beta = \frac{\bar{R} - \bar{S}}{\sqrt{\sigma_R^2 + \sigma_S^2}}$$

   Xác suất phá hoại được tính trực tiếp thông qua hàm tích lũy xác suất chuẩn tắc:

$$P_f = \Phi(-\beta)$$

3. **Mô Phỏng Ngẫu Nhiên Monte Carlo**:
   Thay vì chỉ giải một bài toán đơn định, các thông số đầu vào ($c', \phi', \text{GSI}, r_u$) được lấy mẫu ngẫu nhiên từ các hàm phân phối xác suất thống kê (Phân phối chuẩn, Lognormal, Beta) qua $10.000$ vòng lặp tính toán:

$$P_f = \frac{\text{Số vòng lặp có } FS < 1,0}{\text{Tổng số vòng lặp Monte Carlo}}$$

---

## 6.3 Tiêu Chí Rủi Ro Chấp Nhận Được Giữa Các Ngành

Tiến sĩ Hoek đã thiết lập bảng tiêu chí mục tiêu cân bằng giữa chi phí kinh tế đầu tư và cấp hậu quả rủi ro thảm họa:

| Loại Công Trình | Cấp Độ Hậu Quả Rủi Ro | Hệ Số $FS$ Tĩnh Tối Thiểu | Xác Suất Phá Hoại Chấp Nhận Được Tối Đa ($P_f$) |
|-----------------|------------------------|---------------------------|------------------------------------------------|
| **Bờ Tầng Tạm Mỏ Lộ Thiên** | Thấp (chỉ rơi tràn đá cục bộ trên tầng, không ảnh hưởng người) | $1,1 - 1,2$ | $15\% - 30\%$ |
| **Đường Vận Tải Chính / Bờ Dốc Toàn Mỏ** | Trung bình (gián đoạn vận chuyển quặng, thiệt hại kinh tế lớn) | $1,3$ | $5\% - 10\%$ |
| **Mái Dốc Đường Cao Tốc Dân Dụng** | Cao (đe dọa an toàn giao thông công cộng) | $1,5$ | $1\%$ |
| **Vai Đập Thủy Điện & Gian Máy Ngầm** | Rất nghiêm trọng (nguy cơ vỡ đập, tổn thất nhân mạng thảm khốc) | $1,5 - 2,0$ | $< 0,1\%$ |

---

## 6.4 Vai Trò Của Kế Hoạch Ứng Phó Ngưỡng Kích Hoạt (TARP)

Bởi vì kỹ thuật cơ học đá chấp nhận mức độ không đảm bảo còn tồn lưu, quá trình vận hành bắt buộc phải liên kết dữ liệu quan trắc thời gian thực với ma trận hành động **TARP (Trigger Action Response Plan)**:

- **Mức 1 (Xanh — Vận hành Bình thường)**: Vận tốc dịch chuyển $< 1,0\text{ mm/ngày}$; áp lực nước lỗ rỗng nằm dưới đường bão hòa thiết kế. Hoạt động khai thác mỏ/đào hầm diễn ra bình thường.
- **Mức 2 (Vàng — Cảnh báo / Tăng cường Giám sát)**: Vận tốc dịch chuyển tăng lên $2 - 5\text{ mm/ngày}$ hoặc xuất hiện xu hướng gia tốc. Tăng gấp đôi tần suất đo cảm biến; lắp đặt bổ sung cáp neo dự ứng lực; kiểm tra kỹ vết nứt tách đỉnh dốc.
- **Mức 3 (Đỏ — Di tản Khẩn cấp)**: Phân tích vận tốc nghịch đảo ($1/v \to 0$) cho thấy khối đá đã bước vào pha biến dạng trườn tam cấp (tertiary creep) sắp sạt lở. Hú còi báo động; lập tức di tản toàn bộ công nhân và rút máy móc thiết bị; phong tỏa hiện trường.

---

## 6.5 Thuật ngữ Đối chiếu Chuẩn hóa

| Thuật ngữ Tiếng Anh | Thuật ngữ Tiếng Việt Chuẩn hóa | Định nghĩa Kỹ thuật |
|---------------------|--------------------------------|----------------------|
| Factor of Safety (FS) | Hệ số an toàn (FS) | Tỷ số giữa tổng lực kháng giữ chống trượt và lực gây trượt |
| Probability of failure ($P_f$) | Xác suất phá hoại ($P_f$) | Khả năng xuất hiện trường hợp tải trọng vượt quá khả năng chịu lực |
| Reliability index ($\beta$) | Chỉ số độ tin cậy ($\beta$) | Số độ lệch chuẩn ngăn cách giữa biên an toàn trung bình với trạng thái phá hoại |
| Monte Carlo simulation | Mô phỏng Monte Carlo | Phương pháp tính toán lặp ngẫu nhiên để đánh giá phân phối xác suất |
| Trigger Action Response Plan (TARP) | Kế hoạch ứng phó ngưỡng kích hoạt (TARP) | Ma trận định sẵn các hành động vận hành tương ứng với từng mức đo cảm biến |
