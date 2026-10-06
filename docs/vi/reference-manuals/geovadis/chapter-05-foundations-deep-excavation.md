---
lang: vi
lang_alt: reference-manuals/geovadis/chapter-05-foundations-deep-excavation/
---

# Móng Sâu, Hố Đào Sâu & Kết Cấu Chắn Giữ

!!! abstract "Tóm tắt Chuyên đề"
    Phiên 4 của *GeoVadis (GAIC 2025)* quy tụ các nghiên cứu quan trọng về kết cấu móng sâu, hố đào sâu và tường chắn đất đô thị. Nội dung bao gồm đánh giá móng bè cọc chịu tải trọng kết hợp đứng - ngang (V-H), cọc hỗn hợp xi măng - đất, ổn định thành vách hào tường vây (barrette) với các đốt mở rộng, thí nghiệm nén tĩnh cọc tự cân bằng hai chiều (BDSLT / Osterberg cell), tường cọc xi măng đất có cốt thép hình (SMW) chắn giữ hố đào sâu 10m và ứng xử nhiệt của cọc siêu nhỏ (micropile).

---

## 1. Móng Bè Cọc Chịu Tải Trọng Kết Hợp V-H (A. Garg, V.A. Sawant, S. Mehndiratta)

### Phân tích Tương tác Bằng Mô hình Phần tử Hữu hạn 3D
Các công trình cao tầng, tháp cầu và trụ móng tuabin gió truyền tải trọng đồng thời rất lớn theo phương đứng ($V$), phương ngang ($H$) và mô-men uốn ($M$) xuống móng bè cọc. Garg và cộng sự sử dụng mô phỏng 3D đàn dẻo để phân tích sự phân chia tải trọng giữa đáy bản bè và nhóm cọc:
- **Huy động ma sát đáy bản bè:** Dưới tải trọng thẳng đứng thuần túy, bản bè truyền từ $30\% - 45\%$ tổng tải trọng trực tiếp xuống nền đất bề mặt. Khi tải trọng ngang tăng cao ($H/V > 0{,}2$), ma sát trượt đáy bè được kích hoạt nhanh chóng, tiếp nhận tới $40\%$ lực cắt ngang trước khi cọc phát sinh chuyển vị ngang đáng kể.
- **Hiện tượng suy giảm độ cứng P-y của nhóm cọc:** Chuyển vị ngang chu kỳ làm đất bị biến dạng dẻo ở độ sâu từ $3D - 5D$ đầu cọc, làm giảm độ cứng ngang của nhóm cọc từ $25\% - 35\%$.
- **Khuyến nghị thiết kế:** Tối ưu hóa chiều dài cọc (cọc dài hơn ở tâm bè để khống chế độ lún, cọc cứng hơn ở chu vi để chịu lực cắt) giúp giảm thiểu độ lún lệch của bè và ngăn ngừa nứt bê tông.

---

## 2. Cọc Hỗn Hợp Xi Măng - Đất (S. Koga, K. Watanabe, T. Naito, N. Tsuchiya)

### Khái niệm & Thí nghiệm Mô hình Ly tâm
Cọc hỗn hợp xi măng - đất gồm một lõi cọc bê tông đúc sẵn hoặc cọc ống thép đặt đồng tâm bên trong cột đất trộn xi măng đường kính lớn. Koga và Watanabe sử dụng thí nghiệm mô hình ly tâm ($50g$) và mô hình tỷ lệ $1g$ hiện trường để làm sáng tỏ cơ chế truyền tải dọc trục và tải trọng ngang:

```
        Tải trọng thẳng đứng P
                 │
                 ▼
       ┌───────────────────┐
       │ Lõi cọc bê tông   │ ◄─── Lõi cọc độ cứng dọc trục cao (Ec)
       │ hoặc cọc thép     │
       │                   │
       ├─┬───────────────┬─┤
       │ │ Vỏ bọc xi măng│ │ ◄─── Vỏ xi măng đất đường kính lớn (E_sc, D_col)
       │ │ - đất         │ │      Tăng chu vi ma sát & diện tích mũi cọc
       ├─┼───────────────┼─┤
       │ │               │ │
       │ │ Sức kháng cắt │ │ ◄─── Huy động ma sát lớn nhờ bề mặt tiếp xúc
       │ │ của đất nền   │ │      nhám giữa xi măng đất và nền đất tự nhiên
       └─┴───────────────┴─┘
```

### Các Đặc trưng Cơ học Chính
1. **Truyền tải trọng thẳng đứng:** Ứng suất dọc trục ban đầu do lõi cọc có mô-đun đàn hồi cao tiếp nhận, sau đó truyền dần sang lớp vỏ xi măng - đất thông qua ma sát tiếp xúc giữa lõi và vữa. Đường kính cột lớn ($D_{col} = 2 - 3 \times D_{core}$) làm tăng diện tích chịu tải mũi cọc lên từ $400\% - 900\%$.
2. **Sức kháng tải trọng ngang:** Khi chịu lực đẩy ngang, cột xi măng - đất bên ngoài huy động sức kháng bị động lớn của các lớp đất bề mặt, giảm chuyển vị ngang đầu cọc hơn $50\%$ so với cọc đúc sẵn thông thường.

---

## 3. Ổn định Thành Vách Hào Tường Vây với Các Đốt Mở Rộng (A. Iwata, K. Watanabe, T. Watanabe)

### Tường Vây Hào với Tiết diện Mở rộng Dạng Chữ T và Chữ Thập
Để chịu mô-men uốn khổng lồ trong các hố đào sâu đô thị, tường vây (barrette) thường được thiết kế thêm các cánh mở rộng (đốt chữ T, đốt chữ thập). Tuy nhiên, diện tích bề mặt vách hào đào tăng lên làm gia tăng rủi ro sập lở thành vách hào trong quá trình đào:
- **Duy trì áp lực dung dịch giữ thành:** Phân tích cân bằng giới hạn 3D và phần tử hữu hạn chỉ ra rằng cột áp thủy tĩnh của dung dịch bentonite/polymer phải cao hơn mực nước ngầm ít nhất $1{,}5\,\text{m}$ để ngăn chặn hiện tượng sụt trượt dẻo tại các góc hõm.
- **Dung dịch Polymer so với Bentonite:** Dung dịch polymer cải tiến có độ nhớt và tính dẻo nhớt cao giúp tạo màng sét mỏng liên tục trên các thấu kính cát sỏi xen kẹp, ngăn chặn mất dung dịch và giữ ổn định thành vách hào đào.

---

## 4. Tường Cọc Trộn Sâu Cốt Thép Hình (SMW) Chắn Hố Đào Sâu 10m (Z.W. He, J. Si, K.W. Leong)

### Giải pháp Chắn Giữ cho Công trình Đô thị Chật hẹp
He và cộng sự trình bày giải pháp thiết kế và kết quả quan trắc thực tế cho hố đào tầng hầm sâu 10 mét trong tầng đất sét yếu nhạy cảm:
- **Cấu tạo kết cấu:** Các cọc trộn sâu 3 trục chồng mí ($D = 850\,\text{mm}$) được cấy thép hình H chịu lực (phương pháp SMW) cách cột.
- **Hệ neo dầm trong đất:** Bố trí 2 tầng neo dầm cáp ứng suất trước xuyên qua tường cọc vào tầng đất tốt để khống chế chuyển vị ngang.
- **Hiệu quả thực tế:** Ống đo nghiêng (inclinometer) ghi nhận độ dịch chuyển ngang tối đa của tường chỉ đạt $18\,\text{mm}$ ($< 0{,}2\% H$), hoàn toàn nằm trong giới hạn cho phép bảo vệ các tòa nhà lân cận.

---

## 5. Thí nghiệm Nén Tĩnh Cọc Tự Cân Bằng Hai Chiều (BDSLT) (A.K. Chakraborti, S.K. Golchha, A. Uppadhyay)

### Ứng dụng Hộp Gia tải Osterberg (O-cell) cho Cọc Khoan Nhồi Tải Trọng Lớn
Thí nghiệm nén tĩnh gia tải từ đỉnh truyền thống cho cọc khoan nhồi sức chịu tải lớn ($Q_{ult} > 25.000\,\text{kN}$) đòi hỏi hệ dầm phản lực và đối trọng tải trọng khổng lồ hoặc cọc neo kéo phức tạp. Chakraborti và cộng sự đánh giá thí nghiệm sử dụng hộp thủy lực tự cân bằng Osterberg (O-cell) đặt tại đáy cọc:
- **Nguyên lý tự cân bằng:** Hộp O-cell kích đẩy ngược lên trên lấy ma sát thành thân cọc bên trên làm đối trọng, đồng thời kích đẩy xuống dưới tác dụng trực tiếp vào sức kháng mũi cọc và ma sát đoạn cọc bên dưới.
- **Tổng hợp đường cong tải trọng - chuyển vị đỉnh cọc tương đương:** Sử dụng phương pháp tổng hợp Schmertmann / O-cell để chuyển đổi dữ liệu thí nghiệm hai chiều thành đường cong nén tĩnh đỉnh cọc thông thường:
  $$S_{top}(Q) = S_{up}(Q_{shaft}) + S_{elastic\_shortening}$$
- **Bố trí cảm biến đo biến dạng:** Các thanh thép đo biến dạng phụ (Sister Bar) lắp đặt nhiều tầng dọc lồng thép cọc giúp xác định chính xác sự phân bố ma sát thành đơn vị ($f_s$) qua từng lớp địa tầng sét - đá phiến.

---

## 6. Bảng Thiết bị Quan trắc Hiện trường cho Móng & Hố Đào Sâu

| Cấu kiện / Hạng mục | Thiết bị Quan trắc Chính | Thiết bị Bổ trợ | Đại lượng Đo đạc Theo dõi |
| :--- | :--- | :--- | :--- |
| **Móng bè cọc (Piled Raft)** | Hộp đo áp lực đất (đáy bè) | Cảm biến đo biến dạng đầu cọc (Strain gauge) | Tỷ lệ chia sẻ tải trọng bè/cọc, áp lực tiếp xúc |
| **Tường vây (Barrette / Thép H)** | Ống đo nghiêng (Inclinometer thân tường) | Cảm biến đo tải trọng trên đầu neo (Load cell) | Đường cong chuyển vị ngang tường, suy giảm lực neo |
| **Biến dạng đất quanh hố đào** | Thiết bị đo biến dạng sâu (Extensometer) | Cảm biến đo độ nghiêng bề mặt (Tiltmeter nhà lân cận) | Biểu đồ lún phân tầng theo độ sâu, độ nghiêng công trình lân cận |
| **Thí nghiệm nén tĩnh BDSLT** | Cảm biến đo dịch chuyển khe hở O-cell | Thanh thép đo biến dạng phụ (Sister Bar thân cọc) | Độ mở O-cell, phân bố ma sát thành đơn vị $f_s$ |
| **Tường SMW cọc trộn sâu** | Ống đo nghiêng gắn trên thép H | Áp kế dây rung quan trắc sau lưng tường | Chuyển vị ngang tường cừ, hạ thấp mực nước ngầm |
