---
lang: vi
lang_alt: reference-manuals/geovadis-vol2/chapter-02-practice-risk-site-characterisation/
---

# Thực hành, Đánh giá Rủi ro & Khảo sát Hiện trường

!!! abstract "Tóm tắt Chuyên đề"
    Phiên 7 của *GeoVadis (GAIC 2025)* kết nối các công nghệ chẩn đoán tiên tiến với thực tiễn hành nghề địa kỹ thuật và quản lý rủi ro công trình. Nội dung trọng tâm bao gồm đo ảnh điện trở theo chuỗi thời gian (time-lapse ERT) theo dõi dòng thấm nội tại, địa vật lý sóng mặt (MASW), tiêu tán áp lực trong thí nghiệm dilatometer (DMT) xác định lịch sử ứng suất quá cố kết, kỹ thuật chụp ảnh phát quang cơ học khi đóng cọc và mô hình hóa thông tin công trình (BIM).

---

## 1. Đo Ảnh Điện Trở Theo Chuỗi Thời Gian (Time-Lapse ERT) Quan Trắc Thấm (V. Bherde, B. Umashankar)

### Phát Hiện Sớm Khuyết Tật Ẩn Không Phá Hủy
Xói ngầm (piping), hố sụt ngầm và sự dâng cao bất thường của mặt thấm bên trong đập đất và đê bao thường phát triển âm thầm trước khi xảy ra vỡ đập thảm khốc. Bherde và Umashankar nghiên cứu mô hình thực nghiệm sử dụng phương pháp đo ảnh điện trở 2D/3D theo chuỗi thời gian (time-lapse ERT):
- **Độ tương phản điện trở suất:** Mức độ bão hòa nước làm sụt giảm mạnh điện trở suất biểu kiến ($\rho$), tạo ra sự phân tách rõ nét giữa vùng đất đắp khô chưa bão hòa ($\rho > 500\,\Omega\cdot\text{m}$) và vùng bão hòa dòng thấm ($\rho < 50\,\Omega\cdot\text{m}$).
- **Độ phân giải nghịch đảo:** Bằng cách tối ưu hóa sơ đồ mảng điện cực (kết hợp Wenner-Schlumberger và Dipole-Dipole), hệ thống phát hiện chính xác lỗ rỗng xói ngầm giai đoạn khởi phát ($D \approx 50\,\text{mm}$) và theo dõi vận tốc lan truyền của mũi thấm trong thời gian thực mà không làm tổn hại đến lõi đập.

```
            Nguồn nước ngấm từ thượng lưu
                         │
                         ▼
       ┌──────────────────────────────┐
       │ Đất đắp thân đập chặt khô    │ ◄─── Điện trở suất cao (Khô: > 500 Ω·m)
       │                              │
       │     Chuỗi điện cực quan trắc │
       │     ▼   ▼   ▼   ▼   ▼   ▼   ▼ │
       │                              │
       │       ░░░░░░░░░░░░░░░░       │ ◄─── Luồng thấm ngầm / Mũi nước thấm
       │       ░ Luồng rò rỉ  ░       │      Điện trở suất thấp (< 50 Ω·m)
       │       ░░░░░░░░░░░░░░░░       │      Ảnh cắt lớp 2D hiển thị tức thời
       └──────────────────────────────┘
```

---

## 2. Địa Vật Lý Sóng Mặt Đa Kênh Nâng Cao (MASW) (P. Vishwakarma; C.P. Lin, et al.)

### Thiết Lập Biểu Đồ Vận Tốc Sóng Cắt ($V_s$)
Phương pháp phân tích sóng mặt đa kênh (MASW) cung cấp biểu đồ độ cứng theo chiều sâu một cách nhanh chóng, phi phá hủy và không cần khoan lỗ sâu tốn kém:
- **Tối ưu hóa bài toán nghịch đảo:** Vishwakarma áp dụng thuật toán tối ưu hóa dựa trên dạy và học (TLBO) để giải bài toán nghịch đảo đường cong tán sắc sóng Rayleigh, xác định phân bố vận tốc sóng cắt ($V_s$) xuống độ sâu $30\,\text{m}$.
- **Phân loại cấp đất nền theo địa chấn:** Lin và cộng sự triển khai các cảm biến sóng mặt thế hệ mới để tính toán chỉ số $V_{s30}$, xác định các vùng khuếch đại sóng địa chấn, thung lũng đá ngầm chôn vùi và sự suy giảm mô-đun trượt ($G_{max} = \rho V_s^2$).

---

## 3. Thí Nghiệm Dilatometer (DMT) Tiêu Tán Áp Lực Trong Sét Yếu (K. Das, G.R. Dodagoudar, et al.)

### Xác Định Trực Tiếp Tỷ Số Quá Cố Kết ($OCR$) Tại Hiện Trường
Xác định ứng suất tiền cố kết ($\sigma'_p$) và hệ số cố kết ngang ($c_h$) của bùn sét yếu bằng thí nghiệm nén cố kết một trục trong phòng thí nghiệm thường bị sai lệch lớn do xáo động mẫu. Das và cộng sự sử dụng thí nghiệm xuyên nén ngang Marchetti (DMT) có đo tiêu tán áp lực theo thời gian (chuỗi chỉ số $A$):
- **Chỉ số ứng suất ngang ($K_D$):** Tỷ số quá cố kết ($OCR$) tại chỗ có quan hệ trực tiếp với chỉ số $K_D$:
  $$OCR = (0{,}5 \cdot K_D)^{1{,}56}$$
- **Tiêu tán áp lực kẽ rỗng:** Thời gian cần thiết để tiêu tán $50\%$ áp lực ($t_{50}$) cho phép suy ra hệ số cố kết ngang ($c_h$), phù hợp chặt chẽ với tốc độ lún tính ngược từ các đoạn nền đường đắp thực tế có lắp đặt thiết bị quan trắc.

---

## 4. Hình Ảnh Hóa Quá Trình Đóng Cọc Bằng Hạt Phát Quang Cơ Học (A. Kondo, E. Kohama, D. Takano, R.J. Bathurst)

### Quan Sát Trực Tiếp Tiếp Xúc Hạt Quy Mô Vi Mô
Việc quan sát vùng tập trung biến dạng cắt và vùng vỡ hạt dưới mũi cọc chuyển dịch trước đây đòi hỏi hệ thống chụp tia X phức tạp. Kondo và cộng sự phát minh phương pháp quang học sử dụng các hạt cát được phủ lớp **phốt pho phát quang cơ học** ($\text{SrAl}_2\text{O}_4:\text{Eu}$):
- **Cơ chế phát sáng theo ứng suất:** Khi chịu ứng suất nén tiếp xúc và biến dạng cắt, lớp phủ phốt pho phát ra ánh sáng màu xanh lục có cường độ tỷ lệ thuận với độ lớn ứng suất tiếp xúc.
- **Phân tích trắc quang tốc độ cao:** Máy ảnh tốc độ cao ghi lại bóng tập trung ứng suất động và sự hình thành dải trượt dẻo phát tỏa từ mũi cọc trong suốt quá trình cọc xuyên vào tầng cát chặt.

---

## 5. Thí Nghiệm Xuyên Tiêu Chuẩn (SPT): Thực Tiễn & Hiệu Chuẩn (M.M. Hoque, M.M. Rahman)

### Tiêu Chuẩn Quốc Tế So Với Thực Tế Hiện Trường
Chỉ số xuyên tiêu chuẩn ($N$-value) vẫn là thông số cơ bản phổ biến nhất trong thiết kế móng công trình. Hoque và Rahman khảo sát thực tế thi công tại khu vực Nam Á, chỉ ra những sai lệch lớn so với chuẩn mực ASTM D1586:
- **Tỷ số năng lượng búa thực tế ($ER$):** Cơ cấu búa kéo dây thủ công qua tang quay chỉ truyền được năng lượng thực tế từ $45\%$ đến $58\%$, thấp hơn nhiều so với chuẩn $60\%$ của búa tự động ($N_{60}$).
- **Vệ sinh đáy lỗ khoan & Cân bằng áp lực:** Đáy lỗ khoan không sạch và mất cân bằng cột áp thủy tĩnh trong ống vách gây hiện tượng bùng cát đáy lỗ khoan, làm giảm giá trị $N$ đo được tới $50\%$.
- **Bắt buộc hiệu chuẩn chuẩn hóa:** Các kỹ sư thiết kế bắt buộc phải áp dụng đầy đủ công thức hiệu chuẩn:
  $$N_{60} = N_{raw} \cdot \frac{ER}{60} \cdot C_B \cdot C_S \cdot C_R$$
  trong đó $C_B, C_S, C_R$ lần lượt là các hệ số hiệu chỉnh đường kính lỗ khoan, ống lấy mẫu và chiều dài cần khoan.

---

## 6. Ma Trận Thiết Bị Khảo Sát & Quan Trắc Hiện Trường

| Phương pháp Khảo sát Hiện trường | Thiết bị Cảm biến Chính | Thiết bị Bổ trợ / Kiểm chứng | Thông số Địa kỹ thuật Thu được |
| :--- | :--- | :--- | :--- |
| **Đo ảnh điện trở Time-Lapse ERT**| Cáp điện trở đa điện cực | Áp kế dây rung tại vùng dị thường | Mức độ bão hòa, vận tốc thấm, phát hiện lỗ rỗng |
| **Mảng địa vật lý sóng mặt MASW** | Dàn geophone tần số thấp ($4{,}5\,\text{Hz}$) | Đầu thu địa chấn lỗ khoan P-S | Vận tốc sóng cắt $V_s$, mô-đun trượt nhỏ $G_0$ |
| **Xuyên nén ngang Flat Dilatometer**| Lưỡi dao DMT thép không gỉ | Xuyên côn đo áp lực nước (CPTu) | Tỷ số quá cố kết $OCR$, hệ số cố kết ngang $c_h$ |
| **Chụp ảnh hạt phát quang cơ học**| Cảm biến trắc quang máy ảnh CCD | Cảm biến đo tải trọng trên đầu cọc | Bóng ứng suất tiếp xúc, dải trượt biến dạng |
| **Hệ thống búa SPT chuẩn hóa** | Cần khoan gắn cảm biến đo năng lượng | Hộp đo tỷ số năng lượng búa | Năng lượng búa thực tế $ER$, chỉ số chuẩn $N_{60}$ |
