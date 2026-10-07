---
lang: vi
lang_alt: reference-manuals/practical-rock-engineering/chapter-08-rock-slopes-mining/
---

# Chương 8 — Mái Dốc Đá Trong Công Trình Dân Dụng & Khai Thác Mỏ

## 8.1 Phổ Quy Mô Kích Thước Bờ Dốc Mỏ Lộ Thiên

Các bờ dốc đá trong khai trường mỏ lộ thiên hoạt động đồng thời trên ba cấp quy mô hình học khác nhau:

1. **Cấp Bờ Tầng Đơn Lẻ (Chiều cao $10 - 30\text{ m}$)**: Độ ổn định bị khống chế bởi các phá hoại động học trượt phẳng, trượt nêm và trượt lật dọc theo các khe nứt đơn lẻ. Chức năng chính là tạo bề rộng cơ tầng hứng đá ($b \ge 0,2 H + 4,5\text{ m}$) để giữ lại các khối đá lăn rơi từ tầng trên.
2. **Cấp Liên Tầng / Cụm Tầng (Chiều cao $50 - 200\text{ m}$)**: Bị khống chế bởi các đới đứt gãy kéo dài, áp lực nước ngầm đọng sau vách tầng và yêu cầu bảo vệ đường vận tải chính của mỏ.
3. **Cấp Toàn Mỏ (Chiều sâu $300 - 1.000\text{ m}$)**: Ổn định tổng thể khổng lồ phụ thuộc vào cơ chế phá hoại cắt trượt phi tuyến của toàn bộ khối đá (tiêu chuẩn Hoek-Brown), các hệ thống đứt gãy khu vực và chế độ thủy văn nước ngầm lưu vực.

---

## 8.2 Các Cơ Chế Phá Hoại Chủ Đạo Của Mái Dốc Đá

```
A. TRƯỢT PHẲNG               B. TRƯỢT NÊM                 C. TRƯỢT LẬT ĐỔ
    |  /                         |   / \                      | ||||
    | / (Góc dốc psi_p)          |  /   \ (Giao tuyến)        | |||| (Khe nứt dốc
    |/                           | /     \                    |/////  cắm vào trong)
```

### 1. Phá Hoại Trượt Phẳng (Planar Failure)
Xảy ra dọc theo một mặt khe nứt liên tục duy nhất có phương vị song song ($\pm 20^\circ$) với mặt dốc và góc dốc mặt nứt nhỏ hơn góc dốc mái tầng nhưng lớn hơn góc ma sát ($\phi < \psi_p < \psi_f$):

$$FS = \frac{c A + (W \cos\psi_p - U - V \sin\psi_p) \tan\phi}{W \sin\psi_p + V \cos\psi_p}$$

Trong đó:
- $W$ = trọng lượng bản thân khối đá trượt
- $A$ = diện tích mặt trượt đáy
- $U$ = lực đẩy nổi của nước lỗ rỗng trên mặt trượt: $U = \frac{1}{2} \gamma_w z_w A$
- $V$ = lực đẩy thủy tĩnh ngang của nước đọng trong vết nứt tách đỉnh dốc: $V = \frac{1}{2} \gamma_w z_w^2$

### 2. Phá Hoại Trượt Nêm (Wedge Failure)
Xảy ra dọc theo đường giao tuyến của hai mặt khe nứt khi đường giao tuyến này lộ ra ngoài mái dốc và dốc hơn góc ma sát tổng hợp.

### 3. Phá Hoại Trượt Lật Đổ (Toppling Failure)
Xảy ra khi hệ khe nứt dốc đứng cắm ngược *vào bên trong* sườn dốc ($\psi_d + \psi_f \ge 90^\circ + \phi$). Mô men trọng lực làm các cột đá cao bị nghiêng đổ ra ngoài, làm toác các khe nứt chân cột và lật nhào xuống dưới đáy moong.

### 4. Phá Hoại Cung Tròn / Khối Đá Liên Tục
Xảy ra trong các khối đá bị nứt nẻ vụn nát, phong hóa mạnh hoặc biến chất nhiệt dịch ($GSI < 40$) nơi không có một mặt trượt cấu trúc ưu tiên nào chiếm ưu thế. Được tính toán bằng các phương pháp cân bằng giới hạn Bishop, Morgenstern-Price hoặc mô hình số giảm cường độ kháng cắt (SSR).

---

## 8.3 Tác Động Phá Hoại Khôn Lường Của Nước Ngầm

Nước ngầm là tác nhân kích hoạt lớn nhất gây nên các vụ sạt lở thảm khốc tại các mỏ lộ thiên:
1. **Làm Suy Giảm Ứng Suất Hữu Hiệu**: Áp lực nước lỗ rỗng ($u$) trừ trực tiếp vào ứng suất pháp ép chặt: $\sigma' = \sigma - u$.
2. **Lực Đẩy Thủy Tĩnh Trong Vết Nứt Tách Đỉnh ($V$)**: Nước mưa chảy đầy vào các vết nứt tách sau đỉnh dốc tạo ra một lực đẩy ngang khổng lồ thúc khối đá lao xuống moong.
3. **Thúc Đẩy Quá Trình Phong Hóa Hóa Học**: Làm trương nở và làm mềm các lớp sét chèn nhét khe nứt, khiến góc ma sát dư tụt từ $25^\circ$ xuống chỉ còn $8^\circ$.

### Thiết Kế Hệ Thống Khoan Tháo Khô Hạ Áp
- Các lỗ khoan thoát nước gần nằm ngang (đường kính $75 - 100\text{ mm}$, đặt ống PVC đục lỗ lọc nước) khoan sâu $50 - 150\text{ m}$ vào vách moong sẽ hạ thấp mạnh mẽ đường bão hòa nước ngầm, giúp tăng hệ số an toàn $FS$ của bờ dốc lên $20 - 40\%$ mà không cần phải bóc bỏ hàng triệu khối đất đá tốn kém.

---

## 8.4 Chế Độ Quan Trắc Mái Dốc Mỏ Lộ Thiên

| Hệ Thống Quan Trắc | Đại Lượng Đo Đạc | Vai Trò Trong Cảnh Báo Sớm |
|--------------------|------------------|-----------------------------|
| **Radar Quan Trắc Mái Dốc (SSR)** | Chuyển vị dọc theo tia ngắm (LOS) | Quét liên tục 24/7 toàn bộ bờ moong; vẽ bản đồ nhiệt vận tốc biến dạng ($mm/giờ$) theo thời gian thực |
| **Trạm Toàn Đạc Robot (RTS)** | Véc-tơ tọa độ 3 chiều $(x,y,z)$ | Đo đạc độ chính xác cao mạng lưới lăng kính gắn trên đường vận tải và mép bờ tầng |
| **Áp Kế Dây Rung (VWP)** | Áp lực nước lỗ rỗng sâu ($u$) | Kiểm chứng hiệu quả hạ mực nước ngầm của các hàng khoan thoát nước và giếng bơm hạ mực nước |
| **Ống Đo Nghiêng Cố Định (IPI)** | Dịch chuyển ngang theo chiều sâu | Xác định chính xác độ sâu đáy mặt trượt ngầm phía dưới đáy moong khai thác |

---

## 8.5 Thuật ngữ Đối chiếu Chuẩn hóa

| Thuật ngữ Tiếng Anh | Thuật ngữ Tiếng Việt Chuẩn hóa | Định nghĩa Kỹ thuật |
|---------------------|--------------------------------|----------------------|
| Catch berm | Cơ tầng lưu giữ đá rơi | Cơ tầng nằm ngang bố trí giữa các tầng dốc để hứng giữ đá lăn |
| Planar failure | Phá hoại trượt phẳng | Sự trượt của khối đá dọc theo một mặt phẳng liên tục duy nhất |
| Toppling failure | Phá hoại trượt lật | Sự lật nhào quay quanh chân của các cột đá dốc cắm vào trong sườn dốc |
| Tension crack | Vết nứt tách đỉnh | Vết nứt kéo mở toác sau đỉnh dốc trước khi xuất hiện trượt lở |
| Depressurization drain | Lỗ khoan tháo khô hạ áp | Lỗ khoan gần nằm ngang khoan vào vách đá để tiêu thoát áp lực nước |
