---
lang: vi
lang_alt: reference-manuals/practical-rock-engineering/chapter-02-intact-rock-strength/
---

# Chương 2 — Cường độ Đá Nguyên vẹn & Thí nghiệm Phòng

## 2.1 Các Thí nghiệm Cơ học Tiêu chuẩn cho Đá Nguyên vẹn

Nắm bắt cường độ của đá nguyên vẹn là bước thiết lập biên trên cơ bản cho mọi bài toán đánh giá cường độ khối đá. Các thí nghiệm phòng được tiêu chuẩn hóa bởi Hiệp hội Cơ học Đá Quốc tế (ISRM) và ASTM bao gồm:

1. **Cường độ Nén Đơn trục (UCS / $\sigma_{ci}$)**: Thực hiện trên các mẫu trụ tròn có tỷ lệ chiều dài trên đường kính $L/D = 2,0 - 2,5$. Hai mặt đầu mẫu đá phải được mài phẳng đạt độ chính xác trong vòng $0,02\text{ mm}$ để chống hiện tượng nứt vỡ mép sớm do tiếp xúc cục bộ không đều.

$$\sigma_{ci} = \frac{P_{\text{phá hoại}}}{A}$$

2. **Thí nghiệm Ép chẻ Kéo gián tiếp Brazil ($\sigma_t$)**: Nén một đĩa đá tròn dọc theo đường kính tạo ra một trường ứng suất kéo thuần túy đồng đều theo phương vuông góc tại tâm đĩa đá:

$$\sigma_t = \frac{2 P}{\pi D t}$$

   Trong đó $D$ là đường kính mẫu đĩa và $t$ là chiều dày của đĩa đá. Với đa số các loại đá giòn, cường độ chịu kéo đơn trục chỉ bằng khoảng $1/10$ đến $1/20$ cường độ nén đơn trục ($\sigma_t \approx 0,05 - 0,10 \sigma_{ci}$).

3. **Thí nghiệm Nén Ba trục (Triaxial Compressive Test)**: Mẫu đá hình trụ được bọc màng cao su kín không thấm nước và đặt vào buồng áp lực để chịu áp lực giam hãm chất lỏng đồng đều ($\sigma_2 = \sigma_3$), sau đó tăng dần lực dọc trục ($\sigma_1$) cho đến khi mẫu đá bị phá hủy trượt.

---

## 2.2 Tiêu chuẩn Bền Phá hoại Hoek-Brown cho Đá Nguyên vẹn

Vào năm 1980, Evert Hoek và E.T. Brown đã công bố phương trình thực nghiệm phi tuyến liên kết giữa ứng suất chính lớn nhất và ứng suất chính nhỏ nhất tại thời điểm phá hoại đỉnh cho đá nguyên vẹn:

$$\sigma_1' = \sigma_3' + \sigma_{ci} \left( m_i \frac{\sigma_3'}{\sigma_{ci}} + 1 \right)^{0,5}$$

Trong đó:
- $\sigma_1'$ = ứng suất chính lớn nhất hữu hiệu tại thời điểm phá hủy
- $\sigma_3'$ = ứng suất chính nhỏ nhất hữu hiệu (áp lực giam hãm)
- $\sigma_{ci}$ = cường độ nén đơn trục của mẫu đá nguyên vẹn
- $m_i$ = thông số thực nghiệm thạch học phản ánh thành phần khoáng vật, độ cài răng lược của hạt khoáng và cấu trúc đá

### Giá trị Điển hình của Thông số $m_i$ cho các Loại Đá Phổ biến
| Nhóm Đá | Tên Đá | Giá trị $m_i \pm \text{độ lệch chuẩn}$ |
|---------|--------|----------------------------------------|
| **Magma** | Đá hoa cương (Granite) | $32 \pm 3$ |
| | Đá bazan (Basalt) | $25 \pm 5$ |
| | Đá anđêzit (Andesite) | $25 \pm 5$ |
| **Trầm tích** | Đá cát kết (Sandstone) | $17 \pm 4$ |
| | Đá bột kết (Siltstone) | $7 \pm 2$ |
| | Đá sét kết (Shale) | $6 \pm 2$ |
| | Đá vôi (Limestone) | $12 \pm 3$ |
| **Biến chất**| Đá thạch anh kết (Quartzite) | $20 \pm 3$ |
| | Đá phiến kết (Schist) | $12 \pm 3$ |
| | Đá gơnai (Gneiss) | $28 \pm 5$ |
| | Đá hoa (Marble) | $9 \pm 3$ |

---

## 2.3 Lý thuyết Nứt nẻ Griffith & Sự Phát triển Vi nứt Giòn

Vì sao đường bao phá hoại của đá lại có dạng phi tuyến cong parabol trong thí nghiệm nén ba trục? Nhà vật lý A.A. Griffith (1921, 1924) đã chứng minh rằng sự phá hủy giòn bắt nguồn từ các vi nứt nẻ elip hình thành từ trước và các lỗ rỗng vi mô giữa các ranh giới hạt khoáng.

Dưới tác động của trường ứng suất nén:
1. Ứng suất cắt dọc theo mép các vi nứt gây ra sự tập trung ứng suất kéo cục bộ rất lớn tại hai đầu mút của vết nứt.
2. Khi ứng suất kéo cục bộ vượt quá lực liên kết phân tử, các vết nứt dạng cánh (wing cracks) bắt đầu phát triển ổn định theo phương song song với phương ứng suất chính lớn nhất ($\sigma_1$).
3. **Ngưỡng khởi phát vi nứt ($\sigma_{ci,\text{khởi phát}} \approx 0,4 - 0,5 \sigma_{ci}$)**: Phát xạ âm thanh bắt đầu gia tăng; biến dạng ngang bắt đầu lệch khỏi quy luật tuyến tính đàn hồi.
4. **Ngưỡng tổn thương nứt nẻ ($\sigma_{cd} \approx 0,7 - 0,85 \sigma_{ci}$)**: Các vi nứt bắt đầu liên kết lại với nhau tạo thành các dải cắt vĩ mô, biến dạng thể tích chuyển từ giai đoạn nén co lại sang hiện tượng giãn nở thể tích (volumetric dilation).
5. **Thời điểm phá hoại đỉnh ($\sigma_1 = \sigma_{\text{đỉnh}}$)**: Mẫu đá trượt vỡ hoàn toàn dọc theo mặt trượt cắt vĩ mô.

---

## 2.4 Thuật ngữ Đối chiếu Chuẩn hóa

| Thuật ngữ Tiếng Anh | Thuật ngữ Tiếng Việt Chuẩn hóa | Định nghĩa Kỹ thuật |
|---------------------|--------------------------------|----------------------|
| Uniaxial compressive strength (UCS) | Cường độ nén đơn trục | Ứng suất nén phá hủy lớn nhất khi không có áp lực giam hãm ($\sigma_3 = 0$) |
| Brazilian tensile test | Thí nghiệm ép chẻ kéo Brazil | Thí nghiệm kéo gián tiếp bằng cách nén mẫu đĩa đá theo đường kính |
| Confining pressure | Áp lực giam hãm | Ứng suất chính nhỏ nhất ($\sigma_3$) tác dụng theo phương ngang |
| Intact rock parameter $m_i$ | Thông số vật liệu đá nguyên vẹn $m_i$ | Hằng số thực nghiệm trong phương trình Hoek-Brown phụ thuộc nguồn gốc đá |
| Volumetric dilation | Giãn nở thể tích | Sự tăng thể tích của đá khi bị cắt trượt do sự mở rộng của các vi nứt |
