---
lang: vi
lang_alt: reference-manuals/geotechnical-engineers-handbook/chapter-02-soil-properties/
---
# Chương 2 — Tính chất xây dựng của đất nền

Chương II là phần cơ học đất cốt lõi của sách. Sách định nghĩa "đất xây dựng", rồi
xây dựng từ ba thành phần của đất tới các chỉ tiêu vật lý, và cuối cùng là các lý
thuyết cơ học mà người thiết kế cần.

## 2.1 Định nghĩa đất xây dựng

Đất xây dựng là một **hệ ba thành phần**: hạt rắn, nước và khí.

- Nếu nước chiếm đầy mọi lỗ rỗng, đất **bão hoà**.
- Nếu lỗ rỗng chỉ chứa khí, đất **khô**.
- Nếu lỗ rỗng chứa khí nhưng bị bịt kín khỏi khí quyển, khí đó là **khí bị nhốt**.

Hạt rắn tạo thành **khung cốt liệu** của đất. Các loại đất đặc biệt — đất hữu cơ, than
bùn, bùn — chứa vật liệu hữu cơ bị phân huỷ theo thời gian, khiến chúng có độ nén rất
cao và sức kháng rất thấp.

## 2.2 Cấu trúc đất

### 2.2.1 Phân loại hạt rắn

Sách dùng cách phân loại cỡ hạt theo **tiêu chuẩn Anh (BS)**:

| Cấp hạt | Cỡ hạt $D$ |
| --- | --- |
| Tảng, hòn | $D > 200$ mm |
| Cuội sỏi | $20 < D < 200$ mm |
| Dăm sạn | $2 < D < 20$ mm |
| Cát | $0.06 < D < 2$ mm |
| Bụi | $0.002 < D < 0.06$ mm |
| Sét | $D < 0.002$ mm |

Các hệ phân loại khác lấy ranh giới sét/bụi ở 0,005 mm hoặc 0,002 mm, và ranh giới
bụi/cát ở 0,075 mm hoặc 0,06 mm — các ranh giới này chỉ mang tính quy ước. Ngoài cỡ
hạt, còn hai yếu tố quan trọng: **hình dạng hạt** (tròn, sắc cạnh, nửa tròn) và
**thành phần khoáng vật** của hạt.

### 2.2.2 Nước lỗ rỗng và cấu trúc trong đất

Nước trong lỗ rỗng và cách sắp xếp các hạt thành cấu trúc chi phối tính nén, tính thấm
và sức kháng của đất.

## 2.3 Tính chất vật lý

### 2.3.1 Các thông số tính chất vật lý

Độ ẩm $w$, hệ số rỗng $e$, độ rỗng $n$, các dung trọng $\gamma$, $\gamma_d$,
$\gamma_{sat}$, tỷ trọng hạt $G_s$ — bộ chỉ tiêu tiêu chuẩn.

### 2.3.2 Mối quan hệ giữa các thông số

Các chỉ tiêu không độc lập: sách trình bày trọn bộ quan hệ (quan hệ pha) cho phép suy
ra chỉ tiêu này từ một vài chỉ tiêu đo được. Đây cũng chính là các đồng nhất thức được
lập bảng trong tài liệu [Cơ học đất](../soil-mechanics/chapter-02-composition-index.md)
của trang.

## 2.4 Khái quát tính chất cơ học

### 2.4.1 Lý thuyết đàn hồi áp dụng trong đất

Đất được coi như bán không gian đàn hồi để xác định phân bố ứng suất.

### 2.4.2 Phân bố ứng suất quanh một điểm — vòng tròn Mohr

Trạng thái ứng suất tại một điểm được biểu diễn bằng **vòng tròn Mohr**, cho ứng suất
pháp và ứng suất cắt trên một mặt bất kỳ qua điểm đó. Đây là cơ sở của tiêu chuẩn sức
kháng dùng xuyên suốt cuốn sách.

![Figure: soil-mechanics-mohr-coulomb](../../../assets/figures/soil-mechanics-mohr-coulomb.svg)

**Hình.** Đường bao phá hoại Mohr–Coulomb và vòng tròn Mohr (theo FHWA-NHI-06-088).

### 2.4.3 Lý thuyết biến dạng dẻo áp dụng cho đất

Ngoài miền đàn hồi, đất biến dạng dẻo; sách trình bày khung lý thuyết dẻo dùng để mô
tả chảy dẻo và phá hoại.

### 2.4.4 Đất với lý thuyết cố kết Terzaghi

**Cố kết** là quá trình nén theo thời gian của đất bão hoà khi áp lực nước lỗ rỗng dư
tiêu tán và ứng suất hữu hiệu tăng lên. Lý thuyết cố kết một chiều của Terzaghi là nền
tảng để dự báo lún theo thời gian.

![Figure: soil-mechanics-consolidation](../../../assets/figures/soil-mechanics-consolidation.svg)

**Hình.** Cố kết: đường cong $e$–$\log\sigma'$ và đường cong thời gian–lún (theo USACE EM 1110-1-1904).

### 2.4.5 Lý thuyết Menard cho thí nghiệm nén ngang

Thiết bị **nén ngang** mở rộng một đầu đo hình trụ trong hố khoan và ghi lại quan hệ
áp lực–thể tích; lý thuyết Menard chuyển quan hệ đó thành **mô đun nén ngang** $E_p$ và
áp lực giới hạn $P_l$ — những thông số dùng cho phân tích móng và lún ở Chương 5–6.

## 2.5 Thuật ngữ

| Tiếng Anh | Tiếng Việt (sách dùng) |
| --- | --- |
| three-phase system | hệ ba thành phần (hạt rắn, nước, khí) |
| saturated / dry soil | đất bão hoà / đất khô |
| occluded air | khí bị nhốt |
| soil skeleton | khung cốt liệu |
| grain-size distribution | phân loại hạt (theo cỡ hạt) |
| water content | độ ẩm |
| void ratio | hệ số rỗng |
| porosity | độ rỗng |
| unit weight (bulk / dry / saturated) | dung trọng (tự nhiên / khô / bão hoà) |
| specific gravity | tỷ trọng |
| Mohr circle | vòng tròn Mohr |
| consolidation | cố kết |
| effective stress | ứng suất hữu hiệu |
| pressuremeter modulus | mô đun nén ngang |

## 2.6 Các điểm then chốt

- Đất là **hệ ba thành phần**; khung cốt liệu chịu tải, nước lỗ rỗng chịu áp lực.
- Các ranh giới cỡ hạt chỉ là **quy ước** — ở đây dùng bộ BS.
- Các chỉ tiêu vật lý tạo thành **một hệ quan hệ khép kín**; vài số đo cho ra phần còn
  lại.
- **Vòng tròn Mohr** biểu diễn ứng suất tại một điểm; đường bao **Mohr–Coulomb** cho
  sức kháng.
- **Cố kết Terzaghi** giải thích lún theo thời gian; **lý thuyết Menard** biến đường
  cong nén ngang thành thông số thiết kế.
