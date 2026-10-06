---
lang: vi
lang_alt: reference-manuals/geovadis/chapter-02-ai-computational-geomechanics/
---

# Trí tuệ Nhân tạo (AI) & Cơ học Địa kỹ thuật Tính toán

!!! abstract "Tóm tắt Chuyên đề"
    Phiên 1 của *GeoVadis (GAIC 2025)* làm nổi bật sự kết hợp mạnh mẽ giữa khoa học dữ liệu và mô phỏng số học cơ học đất. Các chủ đề trọng tâm bao gồm ứng dụng mạng nơ-ron nhân tạo (ANN) dự báo thông số đầm chặt, phân tích vi cơ học bằng phương pháp phần tử rời rạc (DEM) cho neo bản ngầm và dòng chảy hạt, học máy đánh giá khả năng hóa lỏng chu kỳ, giải đoán thông số trạng thái CPT và mô hình hóa cấu động đất sét nhiệt - cơ.

---

## 1. Học máy trong Cơ học Vật liệu Địa kỹ thuật Dạng hạt (H. Hunt, B. Indraratna, et al.)

### Chuyển đổi Phương pháp Luận trong Mô hình Hóa Quan hệ Ứng suất - Biến dạng
Các mô hình môi trường liên tục truyền thống (như Cam-Clay, Mohr-Coulomb, Hypoplasticity) gặp nhiều thách thức trong việc mô tả các hiện tượng quy mô hạt như vỡ hạt, dị hướng cấu trúc, phụ thuộc đường dẫn ứng suất và suy giảm chu kỳ mà không phải đưa vào quá nhiều thông số thực nghiệm phức tạp. Nhóm nghiên cứu của Indraratna đã tổng kết bức tranh ứng dụng học máy:

```
    ┌───────────────────────────┐      ┌───────────────────────────┐
    │ Cơ học Môi trường Liên tục │      │ Vi cơ học Quy mô Hạt     │
    │  • Cam-Clay / Hardening   │      │  • Mạng lưới tiếp xúc DEM │
    │  • Hiệu chỉnh thực nghiệm │      │  • Vỡ hạt / Nghiền nát CR │
    └─────────────┬─────────────┘      └─────────────┬─────────────┘
                  │                                  │
                  ▼                                  ▼
    ┌──────────────────────────────────────────────────────────────┐
    │ Học máy Tích hợp Vật lý (Physics-Informed ML / PIML)          │
    │  • Bảo toàn định luật bảo toàn năng lượng & nhiệt động học   │
    │  • Nhận diện hình học hạt 3D micro-CT & phát xạ âm thanh     │
    │  • Tổng quát hóa theo nhiều đường dẫn ứng suất phức tạp      │
    └──────────────────────────────────────────────────────────────┘
```

### Các Kết luận then chốt & Giới hạn
1. **Thiếu hụt dữ liệu & Hiện tượng quá khớp (Overfitting):** Dù các mô hình đạt hệ số tương quan rất cao ($R^2 > 0{,}95$) trên tập dữ liệu phòng thí nghiệm, khả năng tổng quát hóa trên hiện trường đòi hỏi các ràng buộc vật lý nghiêm ngặt (như tính nhất quán nhiệt động lực học và tiêu tán năng lượng dẻo không âm).
2. **Tích hợp hình học hạt 3D:** Kết hợp các chỉ số hình học hạt từ chụp cắt lớp vi tính (micro-CT) (độ tròn, độ cầu, độ nhám bề mặt) vào mạng nơ-ron tích chập giúp cải thiện vượt bậc độ chính xác khi dự báo góc ma sát trạng thái tới hạn ($\phi'_{cs}$).

---

## 2. Cơ chế Kháng Nhổ của Neo Bản Ngang Sâu bằng DEM (R.S. Sowmya, R. Gopika, T.K. Sudheesh)

### Độ sâu Chôn Neo và Cơ chế Phá hoại Cắt
Neo bản ngang đặt sâu được sử dụng rộng rãi cho móng trụ tháp truyền tải điện, hệ thống neo công trình biển và tường chắn đất. Sowmya và cộng sự sử dụng mô hình phần tử rời rạc 3D (DEM) để làm rõ chuyển vị vi mô của đất phía trên bản neo ở các tỷ số chôn sâu ($H/B$) khác nhau:

- **Ứng xử neo nông ($H/B < 3$):** Mặt trượt phá hoại phát triển liên tục lên tận mặt đất, biểu hiện cơ chế phá hoại cắt tổng thể và gây trồi đất bề mặt rõ rệt.
- **Ứng xử neo sâu ($H/B \ge 5$):** Vùng dải dẻo trượt và bóng nén chặt hình thành cục bộ ngay phía trên tấm neo. Phá hoại bị chi phối bởi hiện tượng nở khoang rỗng cục bộ và hiệu ứng vòm đất, không xuất hiện mặt trượt lộ lên mặt đất.

### Hệ số Kháng Nhổ
Hệ số kháng nhổ $N_\gamma = Q_u / (\gamma A H)$ tiệm cận giá trị ổn định khi đạt độ sâu chôn lớn:

$$Q_u = A \cdot \left[ \gamma H N_\gamma + c' N_c \right]$$

Biểu đồ chuỗi lực tiếp xúc trong mô hình DEM cho thấy các chuỗi lực nén mạnh phát tỏa chéo từ mép tấm neo, chuyển đổi lực kéo nhổ thẳng đứng thành các vòm nén hông tựa vào khối đất xung quanh.

---

## 3. Dự báo Thông số Đầm chặt Đất bằng ANN (H. Paneru, N.P. Bhandary)

### Tối ưu hóa Công tác Kiểm soát Đầm chặt Hiện trường
Thí nghiệm đầm chặt tiêu chuẩn (Standard Proctor) và đầm chặt cải tiến (Modified Proctor) đòi hỏi nhiều thời gian và công sức tại hiện trường. Paneru và Bhandary đã xây dựng mô hình mạng nơ-ron nhiều lớp (MLP) để dự báo độ ẩm tối ưu ($OMC$) và dung trọng khô lớn nhất ($MDD$) từ các chỉ tiêu phân loại đất cơ bản:
- **Biến đầu vào:** Giới hạn chảy ($LL$), Giới hạn dẻo ($PL$), Chỉ số dẻo ($PI$), Hàm lượng hạt sét ($CF$), Hàm lượng hạt cát ($SF$), Khối lượng riêng hạt ($G_s$).
- **Thuật toán huấn luyện:** Thuật toán lan truyền ngược Levenberg-Marquardt kết hợp điều chuẩn Bayes.
- **Độ chính xác:** Mô hình ANN đạt hệ số tương quan $R^2 = 0{,}93$ đối với $MDD$ và $R^2 = 0{,}91$ đối với $OMC$, giúp sàng lọc nhanh chất lượng đất đắp nền đường giao thông.

---

## 4. Học máy Đánh giá Khả năng Hóa lỏng Chu kỳ (S. Sah, V. Bherde, U. Balunaini)

### Huấn luyện trên Dữ liệu Thí nghiệm Ba trục Chu kỳ
Đánh giá kích hoạt hóa lỏng dưới tác động địa chấn phức tạp theo phương pháp truyền thống dựa trên đường cong tỷ số ứng suất chu kỳ ($CSR$) và số chu kỳ tải trọng ($N_L$). Sah và cộng sự huấn luyện các mô hình Rừng ngẫu nhiên (Random Forest) và Vectơ hỗ trợ (SVM) trên cơ sở dữ liệu thí nghiệm ba trục chu kỳ:
- **Bộ đặc trưng:** Ứng suất giam giữ hữu hiệu trung bình ban đầu ($\sigma'_{m0}$), tỷ số ứng suất chu kỳ ($CSR$), độ chặt tương đối ($D_r$), hàm lượng hạt mịn ($FC$) và tần số gia tải ($f$).
- **Tỷ số áp lực nước lỗ rỗng ($r_u$):** Mô hình dự báo chính xác thời điểm chuyển pha từ trạng thái linh động chu kỳ ổn định ($r_u < 0{,}6$) sang trạng thái hóa lỏng phá hủy đột ngột ($r_u \to 1{,}0$).

---

## 5. Giải đoán Thông số Trạng thái CPT trong Cát (B. Dalnayak, V. Singh, S. Chatterjee)

### Nghịch đảo Trạng thái Cơ lý Hiện trường
Thí nghiệm xuyên côn (CPT) cung cấp số đo liên tục về sức kháng mũi côn ($q_c$) và ma sát thành ($f_s$). Sử dụng mô phỏng số biến dạng lớn (phương pháp ALE / CEL), Dalnayak và cộng sự mô phỏng quá trình xuyên ổn định của mũi côn $60^\circ$ trong cát để hiệu chuẩn thông số trạng thái ($\psi = e - e_c$):

$$Q_{p} = \frac{q_c - \sigma_{v0}}{\sigma'_{v0}} = k \cdot \exp(-m \cdot \psi)$$

trong đó $k$ và $m$ là các hệ số hiệu chuẩn riêng của từng loại cát. Phương pháp số học này giúp loại bỏ sai số trong việc ước tính độ chặt tương đối và sức kháng hóa lỏng hiện trường mà không cần lấy mẫu cát nguyên dạng đóng băng tốn kém.

---

## 6. Bảng Tương quan Giữa Mô hình Tính toán & Thiết bị Quan trắc Hiện trường

| Mô hình Tính toán / Trí tuệ Nhân tạo | Bài toán Địa kỹ thuật Vật lý | Thiết bị Quan trắc Hiện trường Hiệu chuẩn |
| :--- | :--- | :--- |
| **Mô hình cấu động PIML / Nơ-ron** | Suy giảm chu kỳ đất nền móng | Cột cộng hưởng (Resonant column), Mảng địa chấn lỗ khoan |
| **Mô hình DEM nhổ neo bản** | Sức kháng nhổ neo bản / cọc mini | Cảm biến đo tải trọng (Load cell), Cảm biến đo chuyển vị LVDT |
| **Mô hình ANN đầm chặt đất** | Kiểm soát đầm chặt nền đắp đường | Thiết bị đo độ chặt phóng xạ, Rót cát, Bàn nén hiện trường |
| **Mô hình Học máy phân loại hóa lỏng** | Kích hoạt hóa lỏng do động đất | Áp kế dây rung đo áp lực kẽ rỗng ($r_u = \Delta u / \sigma'_0$) |
| **Mô hình FE biến dạng lớn (CPT)** | Lập biểu đồ thông số trạng thái ($\psi$) | Xuyên côn đo áp lực nước lỗ rỗng (CPTu: $q_t$, $u_2$) |
