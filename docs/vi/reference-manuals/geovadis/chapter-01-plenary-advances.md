---
lang: vi
lang_alt: reference-manuals/geovadis/chapter-01-plenary-advances/
---

# Báo cáo Toàn thể: Tiến bộ trong Kỹ thuật Nền móng & Địa kỹ thuật Năng lượng

!!! abstract "Tóm tắt Chuyên đề"
    Phiên Báo cáo Toàn thể của *GeoVadis (GAIC 2025)* quy tụ các bài giảng then chốt từ các chuyên gia đầu ngành quốc tế, giải quyết các thách thức địa kỹ thuật cốt lõi: kiểm soát chất lượng trong xử lý nền đất sâu, trượt lở mái dốc do động đất chịu tác động của nước ngầm, khai thác năng lượng địa nhiệt đô thị bền vững trong móng công trình, cơ học cố kết thoát nước hướng tâm và các kỹ thuật thực nghiệm tiên tiến cho đất không bão hòa.

---

## 1. Đánh giá & Kiểm soát Chất lượng Cọc Trộn Sâu và Jet Grouting (F.H. Lee)

### Bối cảnh Kỹ thuật & Thách thức Thực tế
Công nghệ trộn sâu (cột xi măng - đất) và khoan phụt vữa áp lực cao (jet grouting) được ứng dụng rất rộng rãi tại Châu Á và Việt Nam để làm tường vây chắn giữ hố móng, màn chống thấm và cải tạo nền đất sét yếu ven biển. Tuy nhiên, các cột xi măng - đất tạo thành thường có độ biến thiên không gian rất lớn về cường độ kháng nén ($q_u$), độ liên tục của cọc và đường kính thực tế do sự tiêu tán năng lượng phụt không đồng đều và tính phân tầng của đất tự nhiên.

### Phương pháp Chẩn đoán & Kiểm tra Chất lượng
Giáo sư F.H. Lee tổng hợp các phương pháp đánh giá phá hủy và không phá hủy (NDE) hiện đại:
- **Khoan lấy mẫu lõi liên tục:** Là tiêu chuẩn vàng hiện trường, đòi hỏi tỷ lệ thu hồi mẫu lõi tối thiểu phải đạt 85% để xác định biểu đồ biến thiên cường độ theo chiều sâu.
- **Lấy mẫu ướt tại chỗ (Wet grab sampling):** Hút mẫu vữa lỏng ngay sau khi phụt để kiểm tra độ đồng nhất của mẻ trộn trước khi ninh kết.
- **Đo ảnh điện trở (ERT) & Thí nghiệm siêu âm qua ống đặt sẵn (CSL):** Dò quét không phá hủy hình học thân cọc, phát hiện khuyết tật thắt cổ bồng và kiểm tra độ thẳng đứng của cọc.

### Ý nghĩa Kỹ thuật & Độ tin cậy
Hệ số biến thiên ($COV$) của sức kháng nén một trục ($q_u$) trong đất trộn sâu thường dao động từ $0{,}30$ đến $0{,}65$. Các tính toán kết cấu và độ lún bỏ qua sự biến thiên này sẽ đánh giá quá cao hệ số an toàn thiết kế. Báo cáo đề xuất hệ số thành phần dựa trên lý thuyết độ tin cậy nhằm đảm bảo trạng thái giới hạn sử dụng (SLS) và trạng thái giới hạn cường độ (ULS).

---

## 2. Ảnh hưởng của Nước ngầm đến Mất ổn định Mái dốc do Địa chấn: Động đất Bán đảo Noto 2024 (I. Towhata, S. Oji, T. Hosoya)

### Sự kiện Động đất Bán đảo Noto 2024
Ngày 1 tháng 1 năm 2024, một trận động đất mạnh ($M_w 7{,}5$) đã xảy ra tại Bán đảo Noto thuộc tỉnh Ishikawa, Nhật Bản, kích hoạt hàng nghìn vụ sạt lở đất và lũ bùn đá, làm cô lập các khu dân cư và phá hủy hệ thống hạ tầng ven biển huyết mạch.

### Vai trò Quyết định của Nước ngầm
Giáo sư Ikuo Towhata và các đồng tác giả đã chứng minh rằng trượt lở mái dốc không chỉ đơn thuần do lực quán tính rung chấn gây ra:
- **Lượng mưa tích lũy trước động đất:** Mưa mùa đông và tuyết tan kéo dài trước đó đã đẩy mực nước ngầm lên rất cao, làm bão hòa tầng đá trầm tích Neogene phong hóa và tro núi lửa.
- **Xung áp lực nước lỗ rỗng tức thời:** Rung chấn động đất cực mạnh đã kích hoạt áp lực nước lỗ rỗng dư ($\Delta u$) tăng vọt dọc theo ranh giới địa chất giữa các tầng thấm và không thấm nước, làm suy giảm đột ngột ứng suất pháp hữu hiệu ($\sigma' = \sigma - u$).
- **Sạt lở chậm trễ:** Nhiều vụ trượt lở quy mô lớn xảy ra sau rung chấn chính nhiều giờ, nhấn mạnh vai trò của quá trình tái phân bố thấm nước ngầm và hiện tượng nghẽn tắc đường thoát nước cục bộ.

```
                  Trạng thái trước động đất: Mực nước ngầm dâng cao
                  ┌───────────────────────────────────────────────┐
                  │ Nước mưa / Tuyết tan ngấm xuống               │
                  │    ▼          ▼          ▼          ▼         │
        Mặt đất   ┌─────────────────────────────────────────────┐ │
                  │ Tầng phong hóa bão hòa nước                 │ │
                  │═════════════════════════════════════════════│ │
                  │ Mực nước ngầm (dâng cao)                    │ │
                  └─────────────────────────────────────────────┘ │
                                         │                        │
                   Rung chấn địa chấn mạnh (Mw 7.5)               │
                                         ▼                        │
                  ┌─────────────────────────────────────────────┐ │
                  │ Áp lực nước lỗ rỗng dư tăng vọt (Δu)        │ │
                  │ Ứng suất hữu hiệu σ' = σ - (u + Δu) tụt sâu │ │
                  │ Sức kháng cắt τ_f suy giảm nghiêm trọng     │ │
                  │ ──► Kích hoạt trượt phẳng và trượt cung tròn│ │
                  └─────────────────────────────────────────────┘ │
                  └───────────────────────────────────────────────┘
```

---

## 3. Móng Năng lượng Địa nhiệt Đô thị Bền vững (L. Laloui, E. Ravera, A.F. Rotta Loria)

### Khái niệm Kết cấu Địa kỹ thuật Kích hoạt Nhiệt
Các kết cấu địa kỹ thuật năng lượng—như cọc năng lượng, tường vây năng lượng và vỏ hầm năng lượng—tích hợp các ống trao đổi nhiệt (vòng tuần hoàn chất lỏng khép kín) trực tiếp bên trong cấu kiện móng nhằm thực hiện hai chức năng song hành:
1. Chịu tải trọng cơ học từ kết cấu bên trên của công trình.
2. Trao đổi nhiệt năng tái tạo với tầng đất xung quanh để sưởi ấm hoặc làm mát tòa nhà thông qua hệ thống bơm nhiệt nguồn đất (GSHP).

### Tương tác Nhiệt - Cơ giữa Đất và Kết cấu
Biến thiên nhiệt độ ($\Delta T$) gây ra sự giãn nở và co ngót nhiệt chu kỳ bên trong bê tông kết cấu:
- **Ứng suất nhiệt bị cản trở:** Khi biến dạng giãn nở nhiệt dọc trục bị cản trở bởi sức kháng mũi cọc và ma sát thành bên, ứng suất nén nhiệt đáng kể sẽ phát sinh:
  $$\Delta \sigma_{th} = - E_{pile} \cdot \alpha_c \cdot \Delta T$$
  trong đó $E_{pile}$ là mô-đun đàn hồi của cọc và $\alpha_c$ là hệ số giãn nở nhiệt của bê tông.
- **Từ biến của đất và biến dạng dẻo chu kỳ:** Chu kỳ gia nhiệt / làm lạnh theo mùa làm biến đổi độ cứng và sự huy động sức kháng cắt của tầng đất sét xung quanh, đòi hỏi phải kiểm tra mỏi nhiệt và độ lún lệch lâu dài.

---

## 4. Cơ học Cố kết Thoát nước Hướng tâm (R.G. Robinson, G. Sridhar, R.P. Aparna)

### Cơ chế Thoát nước Hướng tâm Nền đất Yếu
Cố kết hướng tâm kết hợp bấc thấm (PVD) là giải pháp tiêu chuẩn để xử lý gia tải trước cho bùn sét ven biển và đất nạo vét. Giáo sư R.G. Robinson phân tích sâu các nghiệm giải tích kinh điển của Barron và Hansbo:

$$\bar{U}_r = 1 - \exp\left( -\frac{8 \, T_r}{\mu} \right)$$

trong đó $T_r = c_h t / d_e^2$ là nhân tố thời gian hướng tâm, $d_e$ là đường kính vùng ảnh hưởng tương đương của bấc thấm, và $\mu$ là hệ số hình học và hệ số cản xáo động (smear effect):

$$\mu \approx \ln\left(\frac{n}{s}\right) + \frac{k_h}{k_s}\ln(s) - \frac{3}{4} + \pi z (2l - z)\frac{k_h}{q_w}$$

### Bài học Thực tiễn Quan trọng
- **Độ thấm vùng xáo động ($k_h / k_s$):** Tỷ số giữa hệ số thấm nguyên dạng theo phương ngang và hệ số thấm vùng xáo động thường nằm trong khoảng từ $2$ đến $5$. Nếu trục cắm bấc (mandrel) làm xáo động đất quá mức, tốc độ cố kết sẽ bị chậm lại nghiêm trọng.
- **Sức cản dòng chảy của bấc ($q_w$):** Đối với bấc thấm có chiều dài lớn ($> 20\,\text{m}$), khả năng thoát nước theo phương dọc của lõi bấc thấm trở thành nút thắt điều tiết tốc độ thoát nước.

---

## 5. Thực nghiệm Cơ học Đất Không Bão hòa Tiên tiến (T. Nishimura)

### Thí nghiệm Kiểm soát Lực hút dính Ma mao dẫn trong Phòng
Giáo sư T. Nishimura trình bày các kỹ thuật thực nghiệm hiện đại nhằm xác định các đặc trưng của đất không bão hòa:
- **Kỹ thuật tịnh tiến trục (Axis Translation Technique):** Tách biệt áp lực khí lỗ rỗng ($u_a$) và áp lực nước lỗ rỗng ($u_w$) thông qua đĩa gốm có điểm xâm nhập khí cao nhằm kiểm soát lực hút dính ma mao dẫn ($\psi = u_a - u_w$).
- **Đường cong đặc trưng nước - đất (SWCC):** Xác định vòng trễ giữa quá trình hút ẩm và thoát ẩm chi phối khả năng giữ nước của đất.
- **Sức kháng cắt mở rộng Mohr-Coulomb:**
  $$\tau_f = c' + (\sigma - u_a)\tan\phi' + (u_a - u_w)\tan\phi^b$$
  trong đó $\phi^b$ là góc ma sát quy ước thể hiện tốc độ tăng sức kháng cắt theo lực hút dính ma mao dẫn.

---

## 6. Bảng Thiết bị Quan trắc Hiện trường cho Kỹ thuật Đất Nền

| Ứng dụng công trình | Thiết bị quan trắc chính khuyến nghị | Thiết bị bổ trợ / Đo đối chứng | Đại lượng kỹ thuật theo dõi |
| :--- | :--- | :--- | :--- |
| **Cọc trộn sâu & Jet grouting** | Thí nghiệm siêu âm CSL | Khoan lõi + Thí nghiệm nén một trục $q_u$ | Độ liên tục thân cọc, $q_u$, thắt cổ bồng |
| **Mái dốc trượt địa chấn** | Áp kế dây rung (Vibrating Wire Piezometer) | Ống đo nghiêng (Inclinometer) | Áp lực nước lỗ rỗng ($\Delta u$), độ sâu mặt trượt |
| **Cọc năng lượng nhiệt** | Cảm biến đo biến dạng & Sister Bar | Cáp quang đo nhiệt độ phân bố (DTS) | Biến dạng dọc trục nhiệt ($\epsilon_{th}$), nhiệt độ ($T$) |
| **Bấc thấm kết hợp hút chân không** | Áp kế đa tầng theo độ sâu | Thiết bị đo biến dạng sâu (Extensometer) | Tiêu tán áp lực kẽ rỗng ($U_r$), lún cố kết |
| **Mái dốc đất không bão hòa** | Tensiometer / Cảm biến áp suất âm | Thiết bị đo độ ẩm điện dung (TDR) | Lực hút ma mao dẫn ($\psi$), độ ẩm thể tích ($\theta$) |
