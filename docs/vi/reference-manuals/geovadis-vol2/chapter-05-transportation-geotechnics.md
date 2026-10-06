---
lang: vi
lang_alt: reference-manuals/geovadis-vol2/chapter-05-transportation-geotechnics/
---

# Địa kỹ thuật Giao thông

!!! abstract "Tóm tắt Chuyên đề"
    Phiên 10 của *GeoVadis (GAIC 2025)* giải quyết các bài toán kỹ thuật khắc nghiệt trong xây dựng công trình giao thông đường bộ và đường sắt. Các chủ đề cốt lõi bao gồm tường đất có cốt (MSE) xây dựng lưng đối lưng chịu tải trọng tàu hỏa chu kỳ, lưới cao su tái chế từ băng tải phế thải giảm vỡ đá ba-lát, mô phỏng 3D tương tác động lực học tàu - ray - nền đường, gia cố ô địa kỹ thuật (geocell) cho nền đường đất trương nở, nền đắp bằng khối xốp siêu nhẹ EPS geofoam và ảnh hưởng của tải trọng xe điện (EV) lên độ bền mặt đường.

---

## 1. Tường Đất Có Cốt (MSE) Lưng Đối Lưng Chịu Tải Trọng Tàu Hỏa (S. Attara, B. Umashankar)

### Nền Đường Đầu Cầu Hẹp Có Tường Chắn Đôi
Tại các hành lang giao thông chật hẹp và đoạn đường dẫn đầu cầu, các tường chắn đất có cốt thường được xây dựng theo sơ đồ lưng đối lưng với các lớp lưới địa kỹ thuật đặt xếp chồng hoặc liên kết trực tiếp xuyên suốt. Attara và Umashankar phân tích ứng xử động học của tường MSE lưng đối lưng chịu tải trọng trục tàu hỏa chu kỳ ($P_{axle} = 250\,\text{kN}$):
- **Cốt xếp chồng so với cốt liên kết xuyên suốt:** Khi khoảng cách giữa hai mặt tường ($W$) nhỏ ($W/H < 1{,}4$), việc nối liền liên tục các lớp lưới địa kỹ thuật giữa hai mặt tường giúp ngăn chặn hiện tượng phình bụng mặt tường và giảm hơn $40\%$ độ dịch chuyển ngang so với phương án đặt lưới xếp chồng không liên kết.
- **Áp lực đất ngang động:** Bánh tàu chạy tốc độ cao tạo ra các xung áp lực đất ngang động tức thời suy giảm nhanh theo chiều sâu. Biến dạng kéo lớn nhất trong cốt tập trung chủ yếu ở đới nông $0{,}3H$ ngay sát dưới bản đế đường ray.

```
       Mặt Cắt Tường MSE Lưng Đối Lưng Chịu Tải Trọng Trục Tàu Hỏa
       ┌────────────────────────────────────────────────────────┐
       │     Tải trọng trục tàu hỏa tốc độ cao (250 kN)         │
       │   ══════════════════════════════════════════════════   │
       │   ┌────────────────────────────────────────────────┐   │
       ├───┴────────────────────────────────────────────────┴───┤
       │◄── Mặt tường 1    Đất đắp hạt đầm chặt     Mặt tường 2──►│
       ││ ════════════════════════════════════════════════════ ││
       ││ Các lớp lưới địa kỹ thuật nối liền liên tục xuyên suốt││
       ││ ════════════════════════════════════════════════════ ││
       ││ (Loại trừ trượt tuột mối nối; Chuyển vị rất nhỏ)     ││
       ││ ════════════════════════════════════════════════════ ││
       ├───┬────────────────────────────────────────────────┬───┤
       │   │ Tầng đất nền tự nhiên bên dưới                 │   │
       └───┴────────────────────────────────────────────────┴───┘
```

---

## 2. Lưới Cao Su Tái Chế Từ Băng Tải Phế Thải Cho Đá Ba-lát Đường Sắt (S. Hettiyahandi, B. Indraratna, et al.)

### Kinh Tế Tuần Hoàn Trong Bảo Trì Tuyến Đường Sắt Tốc Độ Cao
Hiện tượng vỡ vụn và lún sụt của tầng đá ba-lát chiếm tới hơn $50\%$ tổng chi phí duy tu đường sắt trên toàn thế giới. Nhóm nghiên cứu của Giáo sư Indraratna phát minh các tấm lưới cao su dập lỗ gia công từ các dải băng tải công nghiệp thải loại:
- **Tiêu tán năng lượng va đập:** Được lắp đặt ngay dưới đáy lớp đá ba-lát, độ cản nhớt và tính đàn hồi cao của lưới cao su hấp thụ hiệu quả các sóng xung kích chấn động do khuyết tật tiếp xúc bánh xe - đường ray sinh ra.
- **Giảm suy thoái vỡ hạt đá:** Thí nghiệm ba trục chu kỳ quy mô lớn ($500.000$ chu kỳ gia tải ở tần số $f = 15\,\text{Hz}$) chứng minh lưới cao su giúp giảm chỉ số vỡ hạt đá ba-lát ($BBI$) từ $45\% - 50\%$ so với lớp ba-lát không gia cố.
- **Mô-đun đàn hồi phục hồi ($M_R$):** Tấm đệm cao su dập tắt gia tốc rung động của đường ray mà vẫn giữ nguyên độ đàn hồi cần thiết, giảm đáng kể chu kỳ chèn tà-vẹt và sàng đá ba-lát.

---

## 3. Gia Cố Nền Đường Đất Trương Nở Bằng Ô Địa Kỹ Thuật (Geocell) (S. Srivastava, B. Umashankar, P.K. Mahopatra, et al.)

### Khống Chế Nứt Nẻ Do Trương Nở - Co Ngót Theo Mùa
Mặt đường xây dựng trên nền đất sét trương nở thường xuyên bị nứt mỏi dạng mai rùa và gồ ghề do độ ẩm biến thiên theo mùa khô - mùa mưa. Srivastava và cộng sự nghiên cứu giải pháp đệm ô địa kỹ thuật 3D (geocell) bố trí tại ranh giới giữa lớp móng và nền đất yếu:
- **Cơ chế giam giữ không gian 3 chiều:** Các vách ngăn geocell giam giữ chặt cốt liệu đá dăm, phát sinh ứng suất vòng cao giúp chuyển hóa tải trọng tập trung từ bánh xe thành vùng phân bố ứng suất đáy rất rộng.
- **Hệ số hưởng lợi giao thông ($TBR$):** Thí nghiệm bàn nén chu kỳ và mô phỏng số cho thấy việc gia cố geocell làm tăng hệ số $TBR$ từ $2{,}5 - 3{,}8$ lần, cho phép giảm tới $30\%$ chiều dày lớp bê tông nhựa asphalt mà vẫn triệt tiêu hoàn toàn hiện tượng hằn lún vệt bánh xe.

---

## 4. Nền Đường Đắp Khối Xốp Siêu Nhẹ EPS Geofoam Trên Bùn Sét Yếu (V.V. Butle, G.S. Parvathi, A. Mandal, V. Srinivasan)

### Triệt Tiêu Độ Lún Cố Kết Trên Nền Đất Bùn Ven Biển
Đắp nền đường bằng đất đá thông thường ($\gamma = 18 - 20\,\text{kN/m}^3$) trên các tầng bùn sét dày ven biển gây ra độ lún cố kết khổng lồ và nguy cơ trượt trồi chân taluy. Butle và cộng sự đánh giá giải pháp thay thế bằng các khối xốp siêu nhẹ Expanded Polystyrene (EPS geofoam) có dung trọng siêu nhỏ ($\gamma \approx 0{,}15 - 0{,}25\,\text{kN/m}^3$):
- **Bù trừ áp lực trọng lực:** Việc thay thế 3 mét đất đắp bằng khối EPS geofoam làm giảm hơn $90\%$ ứng suất phụ thêm tác dụng lên nền sét yếu, triệt tiêu gần như hoàn toàn độ lún cố kết sơ cấp và từ biến thứ cấp.
- **Khả năng chịu tải động:** Mô phỏng số xác nhận bản bê tông cốt thép phân phối tải trọng trên đỉnh khối EPS giúp khống chế biến dạng nén chu kỳ trong giới hạn đàn hồi ($\epsilon < 1\%$), đảm bảo tuổi thọ mỏi lâu dài dưới tác động của các đoàn xe tải nặng.

---

## 5. Tác Động Của Xe Điện (EV) Lên Độ Bền Kết Cấu Áo Đường (P. Chaudhary, S. Saride)

### Ảnh Hưởng Của Bộ Pin Nặng Lên Tuổi Thọ Mặt Đường
Xe điện (EV) trang bị các cụm pin dung lượng lớn có trọng lượng không tải nặng hơn từ $20\% - 35\%$ so với các dòng xe sử dụng động cơ đốt trong truyền thống tương đương:
- **Biến đổi phổ tải trọng trục:** Chaudhary và Saride phân tích hệ số hư hỏng mặt đường bằng thiết bị mô phỏng xe tải nặng gia tốc (HVS) và mô hình nhớt đàn hồi Kenlayer.
- **Hư hỏng nứt mỏi và hằn lún:** Tải trọng trục xe điện nặng hơn làm tăng biến dạng kéo đáy lớp bê tông nhựa ($\epsilon_t$) và biến dạng nén thẳng đứng đỉnh nền đất ($\epsilon_v$), làm gia tăng tốc độ hằn lún nền đường từ $28\% - 42\%$.
- **Khuyến nghị thiết kế mới:** Quy trình thiết kế áo đường cần cập nhật lại hệ số trục xe đơn tương đương (ESAL), đồng thời ưu tiên sử dụng nhựa đường biến tính polyme hoặc lớp chèn vật liệu địa kỹ thuật tổng hợp để bảo toàn tuổi thọ thiết kế của tuyến đường.

---

## 6. Danh Mục Thiết Bị Quan Trắc Hiện Trường Cho Địa Kỹ Thuật Giao Thông

| Công trình Giao thông | Thiết bị Quan trắc Kết cấu Chính | Thiết bị Động lực / Tải trọng | Chỉ tiêu Kỹ thuật Theo dõi |
| :--- | :--- | :--- | :--- |
| **Tường MSE lưng đối lưng** | Ống đo nghiêng (Inclinometer) trong tường | Hộp đo áp lực đất động lực | Chuyển vị ngang tường, áp lực ngang do đoàn tàu |
| **Đường sắt rải đá ba-lát** | Cảm biến đo tải trọng dưới đáy tà-vẹt | Gia tốc kế 3 chiều đo dao động ray | Ứng suất tiếp xúc đáy tà-vẹt, độ rung chấn $a_{rms}$ |
| **Nền đường gia cố Geocell** | Hộp đo áp lực đất tại đáy lớp móng | Cảm biến đo dịch chuyển LVDT vệt bánh | Phân bố ứng suất đáy, độ sâu hằn lún vệt bánh |
| **Nền đắp xốp EPS Geofoam** | Thiết bị đo biến dạng sâu (Extensometer) | Hộp đo áp lực đất dưới bản phân phối | Độ lún nền bùn bên dưới, biến dạng nén khối EPS |
| **Thực nghiệm kết cấu áo đường**| Cảm biến đo biến dạng bê tông nhựa (ASG) | Cảm biến đo độ võng đa tầng sâu (MDD) | Biến dạng kéo đáy áo đường $\epsilon_t$, độ võng đàn hồi |
