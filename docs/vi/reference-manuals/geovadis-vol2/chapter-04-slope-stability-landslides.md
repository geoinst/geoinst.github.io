---
lang: vi
lang_alt: reference-manuals/geovadis-vol2/chapter-04-slope-stability-landslides/
---

# Ổn định Mái dốc, Pháp y Trượt lở & Cảnh báo Sớm

!!! abstract "Tóm tắt Chuyên đề"
    Phiên 9 của *GeoVadis (GAIC 2025)* cung cấp các phân tích chuyên sâu về cơ học mái dốc, khám nghiệm pháp y sự cố sạt lở, ngưỡng thấm kích hoạt do mưa và hệ thống cảnh báo sớm cấp vùng. Trọng tâm nghiên cứu bao gồm phân tích ngược mái dốc mỏ lộ thiên, phương pháp phần tử hữu hạn ngẫu nhiên (RFEM) đánh giá biến thiên hệ số thấm, gia cố mái dốc bằng đinh đất xoắn ốc, cơ chế sinh học rễ cây gia cố đất dốc và mô hình cảnh báo sớm TRIGRS / SWI.

---

## 1. Khám Nghiệm Pháp Y Sự Cố Mái Dốc Mỏ Lộ Thiên (A.J.D. Pineda, R.A.C. Luna, et al.)

### Kết Hợp Bất Liên Tục Địa Chất Với Hình Học Mặt Trượt Phá Hoại
Khai thác mỏ lộ thiên tạo ra các mái dốc tầng đào khổng lồ ($H > 300\,\text{m}$), nơi độ ổn định của từng bậc tầng và toàn bộ bờ moong bị chi phối bởi hướng khe nứt kiến tạo, áp lực nước ngầm và nứt nẻ do nổ mìn. Pineda và cộng sự phân tích pháp y một vụ trượt lở nhiều bậc tầng quy mô lớn:
- **Đo vẽ cấu trúc địa chất bằng UAV/LiDAR:** Sử dụng ảnh chụp từ máy bay không người lái và đám mây điểm LiDAR để đo vẽ thế nằm (hướng phương vị/góc dốc), độ liên tục và khoảng cách các hệ khe nứt trên vách trượt.
- **Phương pháp giảm cường độ kháng cắt (SSR):** Phân tích cân bằng giới hạn (LEM) và sai phân hữu hạn liên tục chứng minh rằng việc gán chỉ tiêu khối đá đẳng hướng (như GSI / Hoek-Brown) sẽ không thể dự báo chính xác vị trí trượt nếu không mô phỏng rõ nét các hệ khe nứt dị hướng thực tế.
- **Tái lập trường áp lực thủy tĩnh:** Phân tích cho thấy mạng lưới nứt nẻ do nổ mìn không được thoát nước đã dẫn dòng nước mặt chảy thẳng vào mặt trượt chính, làm áp lực kẽ rỗng tăng vọt kích hoạt trượt phẳng và trượt nêm bất ngờ.

```
       Hình học Bờ Moong Mỏ Lộ Thiên & Đường Dẫn Nước Thấm
       ┌────────────────────────────────────────────────────────┐
       │ Đỉnh tầng 1                                            │
       │ ──┐                                                    │
       │   │ Mái bậc tầng                                       │
       │   └──┐ Đỉnh tầng 2                                     │
       │      │                                                 │
       │      └──┐ Đỉnh tầng 3                                  │
       │         │ ╲  Hệ khe nứt cấu trúc địa chất có sẵn       │
       │         │   ╲   (Góc dốc θ = 45°)                      │
       │         │     ╲                                        │
       │         │  ▲    ╲  Nước mặt ngấm vào & Áp lực kẽ       │
       │         │  │ u    ╲  rỗng dâng cao dọc khe nứt         │
       │         └──┼───────╲───────────────────────────────────┤
       │            │         ╲ Mặt trượt phá hoại (Phòi chân)   │
       │            │           ╲                               │
       │    Chuỗi Áp kế quan trắc ▼ Đáy moong khai thác         │
       └────────────────────────────────────────────────────────┘
```

---

## 2. Phương Pháp Phần Tử Hữu Hạn Ngẫu Nhiên (RFEM) Biến Thiên Độ Thấm (A. Ajith, R.J. Pillai)

### Vượt Qua Hệ Số An Toàn Định Tính Cổ Điển
Các mô hình mái dốc truyền thống luôn giả định hệ số thấm thủy lực ($k$) đồng nhất trong toàn khối đất, dẫn đến tính toán sai lệch tiến trình thấm nước mưa. Ajith và Pillai triển khai phương pháp **Phần tử hữu hạn ngẫu nhiên (RFEM)**, ghép trường ngẫu nhiên tương quan chéo giữa hệ số thấm bão hòa ($k_{sat}$) và chỉ tiêu sức kháng cắt ($c', \phi'$) thông qua phân tích Cholesky:
- **Hình thành các luồng thấm ưu tiên:** Trường hệ số thấm bất đồng nhất tạo ra các kênh thấm tập trung, làm hình thành nhanh chóng các túi áp lực nước lỗ rỗng cục bộ ở tầng nông.
- **Xác suất phá hoại ($P_f$):** Một mái dốc được tính toán định tính đạt hệ số an toàn $FS = 1{,}35$ dưới mưa lớn thực chất lại có xác suất phá hoại thực tế $P_f > 22\%$ khi hệ số biến thiên của độ thấm ($COV_k$) vượt quá $1{,}0$.

---

## 3. Gia Cố Mái Dốc Bằng Đinh Đất Xoắn Ốc (G. Harshitha, R.M. Varghese)

### Công Nghệ Neo Xoắn Thi Công Nhanh
Đinh đất khoan phụt vữa truyền thống đòi hỏi thời gian khoan tạo lỗ, đặt ống vách và chờ vữa ninh kết, làm gia tăng nguy cơ mất an toàn cho công nhân trên các sườn dốc đang sạt lở. Harshitha và Varghese mô phỏng đinh đất xoắn ốc (trục thép gắn các cánh xoắn cơ học):
- **Cơ chế chịu tải tì ép:** Sức kháng nhổ của đinh đất xoắn ốc được huy động thông qua sự tì ép trực tiếp của các cánh xoắn vào khối đất xung quanh kết hợp ma sát dọc thân trục giữa các cánh.
- **Khả năng chịu tải tức thì:** Đinh xoắn ốc đạt toàn bộ sức kháng nhổ ngay sau khi vặn xoắn cơ học vào đất bằng mô-men xoắn kiểm soát, không cần thời gian chờ đóng rắn vữa ướt.
- **Hệ số an toàn tổng thể:** Mô phỏng số cho thấy đinh xoắn ốc làm tăng hệ số an toàn mái dốc thêm $35\% - 55\%$ so với đinh khoan phụt vữa cùng đường kính, đồng thời rút ngắn hơn $60\%$ thời gian thi công hiện trường.

---

## 4. Cơ Học Rễ Cây Gia Cố Mái Dốc Đất Feralit (D. Mahima, P.K. Jayasree, K. Balan)

### Kỹ Thuật Sinh Học Bảo Vệ Mái Dốc Nhiệt Đới Thân Thiện Môi Trường
Gia cố mái dốc bằng thảm thực vật là giải pháp xanh, phát thải carbon thấp phù hợp với các vùng mưa gió mùa lớn. Mahima và cộng sự nghiên cứu tương tác cơ học giữa rễ cây và đất dốc feralit:
- **Cường độ kháng kéo của rễ cây ($T_r$):** Thí nghiệm nhổ đứt rễ cây bản địa có hệ rễ cọc sâu chứng minh cường độ kéo của rễ tỷ lệ nghịch với đường kính rễ: $T_r = \alpha \cdot d^{-\beta}$.
- **Gia số lực dính biểu kiến ($\Delta c$):** Áp dụng mô hình sợi gia cố Wu-Waldron để định lượng mức tăng sức kháng cắt do rễ cây:
  $$\Delta c = 1{,}2 \cdot T_r \cdot \left(\frac{A_r}{A}\right)$$
  trong đó $A_r/A$ là tỷ số diện tích rễ cây trên diện tích mặt cắt trượt. Rễ cọc đâm sâu tạo chốt neo cơ học vững chắc xuống độ sâu $2{,}0\,\text{m}$, ngăn ngừa hoàn toàn các vụ trượt nông bề mặt.

---

## 5. Cảnh Báo Sớm Trượt Lở Cấp Vùng: Mô Hình TRIGRS & Chỉ Số Nước Trong Đất (M. Susarla, et al.; S. Siva Subramanian, et al.)

### Thiết Lập Ngưỡng Thấm Thủy Văn Cảnh Báo Sạt Lở
Chuyển hóa dữ liệu đo mưa thành các cảnh báo hành động thực tế đòi hỏi mô hình thủy văn - địa kỹ thuật chuẩn xác:
- **Mô hình TRIGRS:** Susarla và cộng sự áp dụng mô hình thấm nước mưa tức thời trên lưới không gian TRIGRS cho hành lang miền núi $50\,\text{km}^2$ tại Karnataka (Ấn Độ), giải bài toán thấm 1D qua các lớp đất chưa bão hòa để lập bản đồ biến thiên hệ số an toàn theo thời gian thực ($FS(x,y,t)$).
- **Chỉ số nước trong đất (SWI):** Cục Địa chất Ấn Độ phát triển mô hình dòng chảy 3 bể chứa tuyến tính để tính toán chỉ số SWI. Việc thiết lập ngưỡng cảnh báo kép (cường độ mưa ngắn hạn kết hợp độ ẩm tích lũy SWI dài hạn) cho phép đưa ra cảnh báo sớm trước tới 24 giờ, giảm thiểu tối đa thiệt hại nhân mạng trong mùa mưa bão cực đoan.

---

## 6. Mạng Lưới Thiết Bị Quan Trắc Hiện Trường Cho Mái Dốc & Trượt Lở

| Loại Hình Mái Dốc / Cơ Chế | Thiết bị Quan trắc Chính | Thiết bị Bổ trợ / Đối chứng | Thông số Kỹ thuật Giám sát |
| :--- | :--- | :--- | :--- |
| **Vách dốc bờ moong mỏ lộ thiên** | Radar giao thoa mặt đất InSAR / Gương robot | Chuỗi ống đo nghiêng cố định (IPI) | Vận tốc chuyển vị bề mặt, chiều sâu mặt trượt |
| **Mái dốc đất chịu mưa bão** | Áp kế dây rung đa tầng (Piezometer) | Tensiometer & Vũ kế tự động đo mưa | Áp lực nước lỗ rỗng tức thời, mất lực hút, lượng mưa |
| **Mái dốc đóng đinh đất xoắn ốc** | Cảm biến đo biến dạng trên thân đinh | Cảm biến đo tải trọng dưới bản đệm | Biểu đồ lực kéo đinh đất, lực ép bản mặt |
| **Mái dốc gia cố rễ thực vật** | Cảm biến đo độ ẩm đất dạng que (TDR) | Cảm biến đo độ nghiêng bề mặt (Tiltmeter) | Độ ẩm vùng rễ cây, biến dạng từ biến tầng nông |
| **Hành lang giao thông cấp vùng** | Trạm khí tượng tự động ghi nhận SWI | Ảnh vệ tinh giao thoa vi sóng InSAR | Lượng mưa tích lũy, tốc độ biến dạng sườn dốc |
