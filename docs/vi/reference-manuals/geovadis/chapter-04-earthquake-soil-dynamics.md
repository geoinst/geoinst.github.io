---
lang: vi
lang_alt: reference-manuals/geovadis/chapter-04-earthquake-soil-dynamics/
---

# Kỹ thuật Địa chấn & Động lực học Đất

!!! abstract "Tóm tắt Chuyên đề"
    Phiên 3 của *GeoVadis (GAIC 2025)* công bố các nghiên cứu đột phá trong kỹ thuật động đất, cơ học biến dạng dẻo chu kỳ của đất và giải pháp giảm thiểu rung chấn công trình. Trọng tâm nghiên cứu bao gồm xử lý hóa lỏng bằng polyme sinh học thân thiện môi trường, đánh giá hóa lỏng bằng chỉ số xếp hạt (packing index), rãnh ngăn rung chấn bằng hỗn hợp cát - cao su (SRM), cô lập địa chấn cho móng bè cọc không liên kết và quan trắc dao động hiện trường do nổ mìn phá dỡ công trình.

---

## 1. Xử lý Hóa lỏng Cát Pha Sét bằng Polyme Sinh học Chitosan (N.V. Dasari, M.D. Tellam, K.K. Gonavaram)

### Giải pháp Gia cố Đất Xanh Thân thiện Môi trường
Các phương pháp phụt vữa hóa học và xi măng truyền thống phát thải lượng lớn khí nhà kính và có nguy cơ gây ô nhiễm nguồn nước ngầm. Dasari và cộng sự nghiên cứu ứng dụng **chitosan** tự nhiên (polyme sinh học chiết xuất từ vỏ giáp xác) làm chất ổn định đất xanh nhằm ngăn ngừa hiện tượng cát pha sét bị hóa lỏng ($FC = 15\% - 25\%$):
- **Cơ chế liên kết hydrogel:** Sau khi trộn và dưỡng hộ, chitosan hình thành các dải màng hydrogel nhớt bao bọc bề mặt các hạt thạch anh và bắc cầu qua các cổ rỗng giữa các hạt đất.
- **Tỷ số sức kháng chu kỳ ($CRR_{15}$):** Thí nghiệm ba trục chu kỳ khống chế biến dạng chỉ ra rằng việc xử lý cát pha sét rời bằng $1{,}0\%$ chitosan làm tăng tỷ số sức kháng chu kỳ ($CRR$) lên tới $180\%$.
- **Kìm hãm áp lực nước lỗ rỗng:** Tốc độ gia tăng áp lực nước lỗ rỗng dư ($\Delta u / \sigma'_0$) chậm lại rõ rệt, ngăn chặn hiện tượng mất ứng suất giam giữ hữu hiệu đột ngột trong các đợt rung chấn địa chấn.

```
       Cát rời pha sét chưa xử lý               Cát pha sét xử lý Chitosan
       ┌───────────────────────────┐            ┌───────────────────────────┐
       │   ○       ○       ○       │            │   ○───────○═══════○       │
       │     ○       ○       ○     │   ─────►   │   │  Màng Polyme  │       │
       │   ○       ○       ○       │            │   ○═══Hydrogel════○       │
       │ (Tiếp xúc hạt rời rạc)    │            │ (Liên kết mạng lưới hạt)  │
       └─────────────┬─────────────┘            └─────────────┬─────────────┘
                     │                                        │
               Rung chấn Động đất                       Rung chấn Động đất
                     ▼                                        ▼
       ┌───────────────────────────┐            ┌───────────────────────────┐
       │ Δu tăng vọt (ru ──► 1)    │            │ Δu bị triệt tiêu (ru <0.4)│
       │ Đất bị hóa lỏng hoàn toàn │            │ Kết cấu hạt ổn định bền   │
       └───────────────────────────┘            └───────────────────────────┘
```

---

## 2. Chỉ số Xếp Hạt Đánh giá Khả năng Kháng Hóa Lỏng (M.U. Rehman, R.K. Kandasami, S. Banerjee)

### Vượt qua Hạn chế của Độ chặt Tương đối ($D_r$)
Độ chặt tương đối ($D_r$) thường có độ tương quan kém với sức kháng hóa lỏng của cát khi hình dạng hạt góc cạnh hoặc thành phần cấp phối hạt trải rộng. Rehman và cộng sự đề xuất **Chỉ số xếp hạt (Packing Index - $I_p$)** dựa trên cơ sở vi cơ học hạt:

$$I_p = \frac{e_{max} - e}{e_{max} - e_{min}} \cdot \left( \frac{d_{50}}{d_{10}} \right)^{\alpha} \cdot \Phi_s$$

trong đó $\Phi_s$ là độ cầu của hạt và $\alpha$ là hệ số cấp phối hạt.
- **Kiểm chứng chụp cắt lớp vi tính Micro-CT:** Ảnh chụp cắt lớp 3D chứng minh rằng các loại cát có cùng độ chặt $D_r$ nhưng hạt có độ cầu thấp hơn sẽ tạo nên số phối vị tiếp xúc ($Z_c$) lớn hơn và các vòm lực tiếp xúc cứng vững hơn.
- **Tương quan với $CRR$:** Chỉ số xếp hạt $I_p$ cho phép xây dựng một hàm tương quan thống nhất với tỷ số sức kháng chu kỳ ($CRR$) cho cả cát sạch hạt đều và cát pha sét cấp phối tốt ($R^2 = 0{,}94$).

---

## 3. Ngăn cách Rung chấn bằng Rãnh Hỗn hợp Cát - Cao su (SRM) (A. Boominathan, J.S. Dhanya, et al.)

### Cơ chế Màng chắn Sóng Động lực học
Dao động lan truyền trong lòng đất do đóng cọc tải trọng xung, đường sắt tốc độ cao và máy móc công nghiệp nặng gây hiện tượng cộng hưởng và nứt mỏi các công trình lân cận. Boominathan và cộng sự triển khai rãnh ngăn sóng bằng hỗn hợp Cát - Hạt cao su lốp xe phế thải (SRM):
- **Bất tương xứng trở kháng sóng:** Hạt cao su lốp xe nghiền nhỏ trộn với cát hạt thô (tỷ lệ $30/70$ theo trọng lượng) tạo ra tỷ số trở kháng âm học ($\rho v_s$) nhỏ hơn $0{,}35$ so với nền đất tự nhiên xung quanh.
- **Triệt tiêu sóng Rayleigh:** Mô phỏng số 3D phần tử hữu hạn và thử nghiệm hiện trường chứng minh rằng rãnh vật liệu SRM với chiều sâu chuẩn hóa $H / \lambda_R \ge 0{,}75$ giúp suy giảm biên độ sóng bề mặt Rayleigh tới $68\%$ trong vùng được bảo vệ.
- **Tính ổn định địa kỹ thuật:** Khác với rãnh hở dễ bị sạt lở hoặc ngập nước ngầm, rãnh vật liệu SRM giữ cho thành hố đứng vững mà vẫn lọc và tiêu tán sóng chấn động hiệu quả.

---

## 4. Ứng xử Địa chấn của Móng Bè Cọc Không Liên kết (A.K. Suman, J.S. Rajeswari)

### Lớp Đệm Cách chấn Địa chấn
Tại các vùng có rủi ro địa chấn cao, việc liên kết ngàm cứng đầu cọc trực tiếp vào đài bè móng sẽ làm tập trung lực cắt quán tính và mô-men uốn cực lớn tại vị trí liên kết đầu cọc:
- **Thiết kế lớp đệm không liên kết:** Bố trí một lớp đệm cấp phối đá dăm gia cố ô địa kỹ thuật hoặc lưới địa kỹ thuật (dày $0{,}5\,\text{m} - 1{,}0\,\text{m}$) giữa đáy bè và đầu cọc.
- **Tách rời quán tính:** Thí nghiệm mô hình ly tâm động và mô phỏng số chứng minh rằng lớp đệm cho phép xảy ra trượt dẻo có kiểm soát khi gia tốc phổ đạt đỉnh, khống chế lực cắt truyền xuống thân cọc.
- **Giảm mô-men uốn:** Mô-men uốn tại đầu cọc giảm từ $50\% - 75\%$ so với móng bè cọc liên kết ngàm cứng truyền thống, loại trừ nguy cơ phá hoại cắt giòn ở cổ cọc trong khi vẫn kiểm soát tốt độ lún dưới tải trọng tĩnh dài hạn.

---

## 5. Quan trắc Rung chấn Nổ mìn Phá dỡ Công trình (A. Anil, T. Naskar, A. Boominathan, A. Joseph)

### Tín hiệu Động lực học Phá dỡ Kết cấu Nặng
Trong quá trình nổ mìn phá dỡ có kiểm soát các công trình công nghiệp quy mô lớn (ống khói nhà máy nhiệt điện, tháp than), năng lượng nổ sinh ra các sóng chấn động tức thời lan truyền qua các tầng địa chất phức tạp:
- **Cảm biến đo vận tốc 3 phương:** Các đầu đo địa chấn geophone trực giao (ngang, đứng, xuyên tâm) ghi nhận vận tốc đỉnh dao động hạt ($PPV$) và phổ tần số dao động.
- **Quy luật suy giảm USBM:** Dữ liệu hiện trường tuân theo phương trình khoảng cách tỷ lệ:
  $$PPV = K \cdot \left( \frac{R}{\sqrt{Q}} \right)^{-B}$$
  trong đó $Q$ là lượng thuốc nổ trên một bước vi sai (kg) và $R$ là cự ly quan trắc (m).
- **Kiểm soát chấn động an toàn:** Hệ thống truyền số liệu từ xa thời gian thực đảm bảo tần số dao động luôn nằm ngoài dải tần số riêng của các công trình lân cận ($> 20\,\text{Hz}$), loại trừ nguy cơ cộng hưởng nguy hiểm.

---

## 6. Ma trận Thiết bị Quan trắc Hiện trường cho Động lực học Đất

| Hiện tượng Động lực học | Thiết bị Quan trắc Chính | Thiết bị Bổ trợ | Đại lượng Kỹ thuật Thu thập |
| :--- | :--- | :--- | :--- |
| **Kích hoạt hóa lỏng địa chấn** | Áp kế dây rung tần số cao (Piezometer) | Cặp gia tốc kế đặt trong lỗ khoan | Áp lực kẽ rỗng tức thời $\Delta u$, biến dạng cắt chu kỳ $\gamma_{cyc}$ |
| **Kiểm chứng rãnh cản sóng** | Đầu thu địa chấn 3 chiều ($4{,}5\,\text{Hz}$) | Máy ghi địa chấn số | Vận tốc đỉnh dao động hạt ($PPV$), phổ tần số FFT |
| **Móng bè cọc không liên kết** | Hộp đo áp lực đất động lực | Cảm biến đo biến dạng dạng thanh (Sister Bar) | Ứng suất tiếp xúc đáy bè, phân bố lực dọc thân cọc |
| **Suy giảm chấn động do đóng cọc**| Gia tốc kế áp điện | Máy đo rung quang học laser Doppler | Gia tốc đỉnh dao động mặt đất ($a_{max}$) |
| **Vận tốc sóng cắt tầng đất nền** | Đầu thu geophone lỗ khoan / Đo ngang xuyên lỗ | Thiết bị địa chấn thả lòng ống P-S | Vận tốc sóng cắt $V_s$, mô-đun trượt biến dạng nhỏ $G_{max}$ |
