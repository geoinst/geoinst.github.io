---
lang: vi
lang_alt: reference-manuals/fhwa-mse-walls/chapter-10-references-appendices/
---
# Chương 10 — Tài liệu Tham khảo & Phụ lục

## Tài liệu tham khảo

Danh mục tài liệu tham khảo của sổ tay trải rộng khắp văn liệu đất có cốt: công trình
đất có cốt nguyên thủy của Vidal; các tập *Reinforced Soil Structures* của FHWA;
*AASHTO Bridge Design Specifications*; hướng dẫn thiết kế địa kỹ thuật tổng hợp; và văn
liệu nghiên cứu về nhổ, từ biến, độ bền và cường độ mối nối. Đây là điểm khởi đầu cho
mọi thông số phải được chứng minh ngoài các bảng của chính sổ tay.

## Phụ lục A — Xác định các hệ số sức kháng nhổ

**A.1 Thủ tục kinh nghiệm để xác định $F^{*}$ và $\alpha$.** Với thiết kế thông thường,
hệ số ma sát nhổ $F^{*}$ và hệ số hiệu chỉnh tỷ lệ $\alpha$ được lấy từ góc ma sát của
đất và loại cốt, dùng các biểu đồ kinh nghiệm của sổ tay. Đây là lối mặc định khi không
cần thí nghiệm nhổ.

**A.2 Thủ tục thực nghiệm để xác định $F^{*}$ và $\alpha$.** Khi tổ hợp đất–cốt không
thông thường, hoặc khi giá trị kinh nghiệm không thiên về an toàn, **thí nghiệm nhổ** được
thực hiện: cốt được neo trong đất đắp ứng viên và được kéo nhổ dưới một ứng suất pháp đã
biết, rồi $F^{*}$ (và, với cốt dãn được, $\alpha$) được tính ngược từ sức kháng đo được.
Phụ lục trình bày cách bố trí thí nghiệm, cách diễn giải và cách chuẩn hóa.

**A.3 Sức kháng và cường độ mối nối.** Mối nối giữa cốt và mặt tường có thể là **mắt
yếu nhất** của hệ thống. Phụ lục mô tả các thí nghiệm mối nối cho mối nối khối phân đoạn
ma sát toàn phần và bán phần với cốt, và cách suy ra cường độ mối nối thiết kế từ dữ liệu
tải–chuyển vị và phá hoại.

## Phụ lục B — Xác định hệ số giảm cường độ do từ biến

**B.1 Cơ sở.** Cốt địa kỹ thuật tổng hợp bị từ biến — nó biến dạng liên tục dưới tải duy
trì — nên cường độ dài hạn của nó thấp hơn cường độ ngắn hạn. **Hệ số giảm do từ biến**
$RF_{CR}$ định lượng tổn thất đó.

**B.2 Quy trình từng bước để ngoại suy dữ liệu ứng suất–phá hoại.** Vì kết cấu phải làm
việc hàng chục năm, không thể đo trực tiếp cường độ dài hạn. Phụ lục đưa quy trình chuẩn:
chạy **thí nghiệm ứng suất–phá hoại** ở nhiệt độ cao, dùng **nguyên lý chồng nhiệt độ–thời
gian** (các hệ số dịch chuyển) để dựng đường cong chủ, và **ngoại suy** đường cong đó tới
tuổi thọ thiết kế để tìm tải giới hạn từ biến.

**B.3 Dùng dữ liệu từ biến của các sản phẩm "tương tự".** Khi không có dữ liệu riêng cho
sản phẩm, có thể dùng dữ liệu từ các polyme và kết cấu tương tự kèm lý giải.

**B.4 Các ví dụ ngoại suy từ biến.** Hai ví dụ ngoại suy đã giải trọn — một cho vật liệu
địa kỹ thuật tổng hợp **PET** (polyeste) và một cho **polyolefin** (polypropylen/
polyetylen) — đưa dữ liệu ứng suất–phá hoại thô qua bước dịch chuyển và ngoại suy tới tải
giới hạn từ biến, rồi tới $RF_{CR}$.

## Phụ lục C — Khoảng chi phí gần đúng của vải và lưới địa kỹ thuật

Các khoảng chi phí đã cũ cho cốt địa kỹ thuật tổng hợp, dùng để ước lượng bậc độ lớn. Phải
quy đổi về giá hiện hành tại địa phương trước khi dùng.

## Phụ lục D — Kích thước điển hình của cốt thép

Mặt cắt, kích thước và diện tích tiêu chuẩn của dải thép, lưới thanh và lưới hàn dùng
trong các hệ cốt kim loại — dữ liệu dạng bảng đứng sau phép tính chiều dày ăn mòn ở
[Chương 3](chapter-03-soil-reinforcement-principles.md).

## Phụ lục E — Ví dụ phân tích mái dốc đất có cốt bằng chương trình RSS

Một phân tích mái dốc có cốt đã giải trọn vẹn dùng chương trình RSS của FHWA: hình học và
thông số đất đầu vào, bố trí cốt, tìm kiếm mặt trượt tới hạn, và hệ số an toàn kết quả —
bản tương ứng máy tính với các ví dụ tính tay ở [Chương 7](chapter-07-design-rss.md).

## Các điểm then chốt cần ghi nhớ

- **Hệ số nhổ** lấy từ biểu đồ theo mặc định, từ **thí nghiệm** khi tổ hợp không thông
  thường — Phụ lục A.
- **Cường độ từ biến** phải được **ngoại suy** từ thí nghiệm gia tốc, không được giả định
  — Phụ lục B.
- **Cường độ mối nối** có thể chi phối; phải thí nghiệm — Phụ lục A.3.
- Dữ liệu chi phí (Phụ lục C) và kích thước tiêu chuẩn (Phụ lục D) là **dữ liệu tham khảo
  đã cũ** — phải quy đổi và kiểm chứng lại trước khi dùng.
- Phụ lục E là **phân tích máy tính đã giải** khép vòng thiết kế.

---

## Đọc thêm trong cơ sở tri thức này

- [Sổ tay thiết bị quan trắc địa kỹ thuật FHWA](../fhwa/index.md) — các họ thiết bị mà
  chương trình quan trắc của Chương 9 lựa chọn.
- [Dunnicliff — Thiết bị quan trắc địa kỹ thuật](../dunnicliff/index.md) — triết lý lập
  kế hoạch có hệ thống đứng sau chương trình quan trắc.
- [Kỹ thuật Móng](../foundation-engineering/index.md) — áp lực đất, tường chắn và ổn định
  mái dốc theo kho tư liệu công cộng USACE/FHWA.
- [Cơ học đá thực hành](../practical-rock-engineering/index.md) — phần tương ứng phía đá
  cho mái dốc đá, neo và bê tông phun.
- [Giám sát hiệu năng đập](../monitoring-dam-performance/index.md) — cách dữ liệu chuyển
  vị và áp lực nước lỗ rỗng trở thành quyết định.
- [ADAQS](../../adaqs/index.md) — quan trắc tự động và các mức kích hoạt cho giám sát
  dài hạn.
