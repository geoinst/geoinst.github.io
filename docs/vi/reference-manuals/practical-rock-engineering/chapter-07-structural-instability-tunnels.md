---
lang: vi
lang_alt: reference-manuals/practical-rock-engineering/chapter-07-structural-instability-tunnels/
---

# Chương 7 — Mất Ổn Định Khống Chế Bởi Cấu Trúc Trong Hầm

## 7.1 Sự Giải Phóng Động Học Của Các Khối Nêm Đa Diện

Trong các đường hầm thi công ở độ sâu từ nông đến trung bình xuyên qua các khối đá dạng khối bị nứt nẻ, sự phá hoại hầu như không phải do nén vỡ đá nguyên vẹn. Thay vào đó, **hiện tượng sập rơi do trọng lực của các nêm đá đa diện** giới hạn bởi các mặt bất liên tục giao cắt nhau là nguy cơ đe dọa sinh mạng hàng đầu.

Để một khối nêm đá có thể tách rời và rơi hoặc trượt vào trong lòng hầm, hai điều kiện tiên quyết sau phải được thỏa mãn:
1. **Khả Năng Động Học Cho Phép (Kinematic Feasibility)**: Hình học không gian của các mặt khe nứt giao nhau phải khép kín tạo thành một khối nêm tứ diện hoặc ngũ diện có đỉnh nêm hướng ra xa lòng hầm, và hướng trượt của nó phải lộ ra ngoài khoảng không hang đào mà không bị cản trở về mặt hình học.
2. **Mất Cân Bằng Giới Hạn (Limit Equilibrium Instability)**: Tổng các lực gây trượt (trọng lượng bản thân khối nêm $W$ và áp lực nước khe nứt $U$) phải vượt quá tổng các lực cản giữ (lực dính khe nứt $c_j$, lực ma sát $\sigma_n' \tan\phi_j$ và sức kháng kéo của hệ neo đá $T$).

---

## 7.2 Phép Chiếu Lập Thể & Phân Tích Động Học

Lưới chiếu lập thể (lưới Wulff bảo giác hoặc lưới Schmidt bảo diện) cho phép biểu diễn các số liệu định hướng không gian 3D (Góc dốc $\psi$ và Hướng dốc $\alpha$) lên một mặt phẳng 2D:

- **Đường Vòng Lớn (Great Circles)**: Biểu diễn các mặt phẳng khe nứt và các mặt vách hang đào.
- **Cực Của Mặt Phẳng (Poles)**: Véc-tơ pháp tuyến vuông góc với mặt phẳng khe nứt.
- **Đường Giao Tuyến ($\vec{I}_{12}$)**: Góc dốc phương ($\beta$) và hướng dốc ($\theta$) của đường thẳng giao nhau tạo bởi hai mặt khe nứt:

$$\vec{I}_{12} = \vec{n}_1 \times \vec{n}_2$$

### Các Chế Độ Trượt Động Học:
- **Rơi Tự Do (Roof Dropouts)**: Đỉnh nêm nằm thẳng đứng phía trên nóc hầm; tất cả các mặt bên của nêm đều dốc đứng hơn góc ma sát trong của khe nứt.
- **Trượt Trên Một Mặt Phẳng**: Đường giao tuyến lộ ra ngoài vách hầm, nhưng khối nêm tách rời khỏi một mặt nứt và trượt hoàn toàn dọc theo mặt nứt dốc hơn còn lại.
- **Trượt Trên Hai Mặt Phẳng (Trượt Dọc Giao Tuyến)**: Khối nêm trượt tịnh tiến dọc theo đường giao tuyến $\vec{I}_{12}$, tiếp xúc đồng thời trên cả hai mặt khe nứt.

```
          Đỉnh Nóc Hầm
     +-----------------+
      \     KHỐI NÊM    /
       \  (Trọng lượng W)
        \    /\     /
         \  /  \   /   Mặt Khe Nứt 2
          \/    \ /   (Góc dốc psi_2)
 Mặt Khe Nứt 1   v
 (Góc dốc psi_1) VÉC-TƠ TRƯỢT (Đường giao tuyến)
```

---

## 7.3 Tính Toán Cân Bằng Giới Hạn: Phương Pháp UNWEDGE

Đối với một khối nêm trượt dọc theo đường giao tuyến của Mặt 1 và Mặt 2 có góc nghiêng $\beta$:

### Lực Gây Trượt ($F_{\text{trượt}}$):

$$F_{\text{trượt}} = W \sin\beta$$

### Lực Pháp Tuyến Trên Hai Mặt Khe Nứt ($N_1, N_2$):
Được xác định từ phương trình cân bằng tĩnh học của khối nêm theo phương vuông góc với đường giao tuyến:

$$N_1 + N_2 = W \cos\beta \cdot f(\text{hình học nêm})$$

### Lực Kháng Trượt ($F_{\text{kháng}}$):

$$F_{\text{kháng}} = (c_1 A_1 + N_1' \tan\phi_1) + (c_2 A_2 + N_2' \tan\phi_2) + \sum T_b \cos\theta_b$$

Trong đó $A_1, A_2$ là diện tích các mặt nêm, $N'$ là lực pháp hữu hiệu sau khi trừ áp lực thủy tĩnh khe nứt, và $T_b$ là sức chịu kéo của các thanh neo đá giao cắt với nêm tạo góc $\theta_b$ so với véc-tơ trượt.

$$FS = \frac{F_{\text{kháng}}}{F_{\text{trượt}}}$$

---

## 7.4 Thiết Kế Chống Giữ Nêm Nóc & Nêm Hông Lò

1. **Nguyên Tắc Chống Giữ Tải Trọng Bản Thân (Dead-Weight Support)**: Hệ vì neo phải có khả năng neo giữ toàn bộ trọng lượng thể tích nêm lớn nhất có thể xuất hiện, với chiều dài phần neo ngàm sâu vào khối đá ổn định tối thiểu $\ge 1,5 - 2,0\text{ m}$.
2. **Khoảng Cách Bố Trí Neo**: Bước neo $s$ phải nhỏ hơn kích thước mặt đáy nhỏ nhất của khối nêm dự báo để ngăn các nêm đá con rơi lọt qua khoảng trống giữa các thanh neo:

$$s \le \frac{1}{2} \text{Kích Thước Khối Nêm}$$

3. **Kết Hợp Bê Tông Phun**: Lớp bê tông phun gia cường sợi thép (SFRS) hoặc lưới thép tạo ra màng bọc bề mặt tức thì, giữ chặt các khối nêm khóa (keyblock) không cho bung ra, ngăn chặn hiện tượng sập đổ dây chuyền của cả vòm hầm.

---

## 7.5 Thuật ngữ Đối chiếu Chuẩn hóa

| Thuật ngữ Tiếng Anh | Thuật ngữ Tiếng Việt Chuẩn hóa | Định nghĩa Kỹ thuật |
|---------------------|--------------------------------|----------------------|
| Kinematic analysis | Phân tích động học | Đánh giá hình học xác định khả năng tách rời tự do của khối nêm đá |
| Stereographic projection | Phép chiếu lập thể cực | Phương pháp biểu diễn góc dốc và hướng dốc 3D lên mặt phẳng 2D |
| Line of intersection | Đường giao tuyến | Đường thẳng không gian tạo bởi sự giao cắt của hai mặt bất liên tục |
| Wedge failure | Phá hoại trượt nêm | Sự sập rơi hoặc trượt của khối đá đa diện bị bao bọc bởi các khe nứt |
| Keyblock | Khối nêm khóa | Khối đá mặt ngoài có vai trò then chốt; nếu rơi ra sẽ làm cả khối đá xung quanh mất ổn định |
