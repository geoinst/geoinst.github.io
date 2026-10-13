---
lang: vi
lang_alt: reference-manuals/fhwa-mse-walls/
---
# Tường đất có cốt (MSE) & Mái dốc đất có cốt — Hướng dẫn Thiết kế & Thi công (FHWA)

!!! note "Về tài liệu tham khảo này"
    Đây là một **tài liệu tham khảo kỹ thuật mở, nguyên bản** về tường đất có cốt
    (MSE) và mái dốc đất có cốt (RSS), được viết bằng ngôn ngữ kỹ thuật giản dị.
    Tài liệu được phóng tác theo phạm vi chủ đề và cấu trúc của sổ tay
    **FHWA-NHI-00-043, *Mechanically Stabilized Earth Walls and Reinforced Soil
    Slopes — Design & Construction Guidelines*** (tháng 3 năm 2001), do
    **Victor Elias, P.E.; Barry R. Christopher, Ph.D., P.E.; và Ryan R. Berg,
    P.E.** biên soạn cho **Viện Đường cao tốc Quốc gia (NHI)** thuộc Cục Quản lý
    Đường cao tốc Liên bang Hoa Kỳ (Khóa học NHI số 132042, Phòng Công nghệ Cầu).
    Tài liệu nguồn là **công trình của chính phủ Hoa Kỳ thuộc phạm vi công cộng**
    (*Tuyên bố phân phối: Không hạn chế*); tuy vậy trang này là một bản phóng tác
    độc lập, **không** sao chép nguyên văn. Tài liệu phục vụ mục đích giáo dục và
    sử dụng hiện trường, và mỗi dự án là duy nhất: nội dung ở đây nhằm xây dựng
    phán đoán kỹ thuật, không đặt ra tiêu chuẩn tối thiểu. Toàn bộ sổ tay đã được
    lập chỉ mục trong trợ lý AI [GTI Doctor](../../../gti-doctor.md) để tra cứu
    sâu hơn.

Sổ tay **FHWA *Mechanically Stabilized Earth Walls and Reinforced Soil Slopes***
là tài liệu tham khảo về thiết kế và thi công, đưa công nghệ đất có cốt từ các
nguyên lý cơ bản đến một kết cấu đường bộ có thể xây dựng được. Nếu [sổ tay quan
trắc FHWA](../fhwa/index.md) hướng dẫn cách *theo dõi* một kết cấu đất, thì sổ tay
này hướng dẫn cách *thiết kế và thi công* kết cấu đó: cách kết hợp đất ma sát với
cốt gia cường chịu kéo thành một khối hỗn hợp ứng xử như một khối trọng lực, và
cách khối hỗn hợp ấy được định hình, cấu tạo, đặc thù hóa và nghiệm thu trong một
dự án giao thông.

Sổ tay là văn bản tham chiếu cho khóa học NHI cùng tên. Nó được viết để kỹ sư có
thể nhận diện và đánh giá các ứng dụng tường MSE và mái dốc RSS như một phương án
thay thế cho thi công truyền thống, với phạm vi đủ rộng để phục vụ cả người soạn
định mức kỹ thuật, giám sát thi công và nhân sự hợp đồng, chứ không riêng người
thiết kế.

Tài liệu này đi theo mạch của sổ tay: **đánh giá dự án** (khi nào và vì sao dùng
đất có cốt); **nguyên lý cốt gia cường đất** (cách khối hỗn hợp chịu tải); **thiết
kế** tường MSE, tường hình học phức tạp và mái dốc có cốt; **phương thức hợp đồng
và định mức kỹ thuật**; và **kiểm tra hiện trường cùng quan trắc hiệu năng** — khép
lại bằng năm phụ lục về hệ số nhổ, ngoại suy từ biến, chi phí, kích thước cốt thép
và một phân tích mái dốc RSS đã giải.

---

## Phạm vi của tài liệu này

Sổ tay gồm chín chương cùng danh mục tài liệu tham khảo và năm phụ lục. Tài liệu
này cô đọng cấu trúc đó thành các trang sau:

| # | Chương | Nội dung |
|---|---------|----------------|
| 1 | [Giới thiệu](chapter-01-introduction.md) | Mục tiêu, phạm vi, tài liệu nguồn, thuật ngữ và quá trình phát triển của đất có cốt |
| 2 | [Hệ thống & Đánh giá dự án](chapter-02-systems-project-evaluation.md) | Ứng dụng, ưu nhược điểm, chi phí tương đối, các loại hệ thống và mặt tường, loại cốt, đất đắp và đánh giá khu đất |
| 3 | [Nguyên lý cốt gia cường đất & Thông số thiết kế](chapter-03-soil-reinforcement-principles.md) | Khái niệm đất có cốt, sức kháng nhổ và cắt mặt tiếp giáp, thông số nền/đất đắp/đất lưng tường, cường độ, ăn mòn, từ biến và các hệ số giảm độ bền |
| 4 | [Thiết kế tường MSE](chapter-04-design-mse-walls.md) | Ổn định ngoài và trong, lực kéo và nhổ, mối nối, mặt tường, cấu tạo chi tiết cùng ví dụ tính toán cốt thép dải và cốt địa kỹ thuật |
| 5 | [Tường MSE hình học phức tạp](chapter-05-complex-geometries.md) | Mố cầu, tường xếp lớp và tường lưng tựa lưng, móng bậc, tải nghiêng và ví dụ thiết kế mố cầu |
| 6 | [Mái dốc đất có cốt (RSS): Đánh giá dự án](chapter-06-rss-project-evaluation.md) | Ứng dụng RSS, dạng phá hoại, khái niệm thiết kế, thi công, xử lý mặt dốc và các nghiên cứu tình huống |
| 7 | [Thiết kế mái dốc đất có cốt](chapter-07-design-rss.md) | Quy trình thiết kế RSS từng bước, cân bằng giới hạn có cốt, ổn định ngoài và trong, và thiết kế động đất |
| 8 | [Phương thức hợp đồng & Định mức kỹ thuật](chapter-08-contracting-specifications.md) | Hợp đồng theo phương pháp so với theo kết quả, thiết kế sơ bộ và cuối cùng, thiết kế chuẩn, thẩm tra và định mức kỹ thuật mẫu |
| 9 | [Kiểm tra hiện trường & Quan trắc hiệu năng](chapter-09-field-inspection-monitoring.md) | Thẩm tra trước thi công, kiểm tra vật liệu, kiểm soát thi công và dung sai, chương trình quan trắc giới hạn và toàn diện |
| 10 | [Tài liệu tham khảo & Phụ lục](chapter-10-references-appendices.md) | Nguồn tài liệu, cùng Phụ lục A–E: hệ số nhổ, hệ số từ biến, dữ liệu chi phí, kích thước cốt thép và một phân tích mái dốc RSS |

---

## Cách sử dụng tài liệu này

- **Bắt đầu từ Chương 2 nếu đang chọn hệ thống**, và Chương 3 nếu cần phần cơ học.
  Các Chương 4, 5 và 7 là các quy trình thiết kế.
- **Sau đó đọc chương tương ứng với kết cấu của bạn.** Tường MSE (Chương 4–5) và
  mái dốc đất có cốt (Chương 6–7) là hai kết cấu khác nhau với dạng phá hoại khác
  nhau, dù cùng chia sẻ nguyên lý cốt gia cường.
- **Dùng kèm với phần còn lại của cơ sở tri thức.** Các chương thiết kế liên kết
  chéo sang phần [Kỹ thuật Móng](../foundation-engineering/index.md) về áp lực đất
  và tường chắn, cùng [sổ tay quan trắc FHWA](../fhwa/index.md) và
  [Dunnicliff](../dunnicliff/index.md) cho công tác quan trắc mà Chương 9 yêu cầu.
- **Hỏi [GTI Doctor](../../../gti-doctor.md).** Trợ lý AI có thể trả lời các câu
  hỏi theo từng loại kết cấu dựa trên toàn bộ kho tư liệu FHWA.

---

## Tài liệu nguồn (PDF)

=== "Tiếng Anh — sổ tay gốc (PDF)"

    **Sổ tay gốc tiếng Anh** — *Mechanically Stabilized Earth Walls and Reinforced
    Soil Slopes: Design & Construction Guidelines* (394 trang), FHWA-NHI-00-043,
    tháng 3 năm 2001. Là **công trình của chính phủ Hoa Kỳ thuộc phạm vi công
    cộng** (phân phối không hạn chế). Được đăng tải tại đây để bản 2001 (đã được
    thay thế) vẫn có thể trích dẫn song song với bản GEC-11 hiện hành. Trang bìa
    của bên phân phối thứ ba đã được gỡ bỏ, nên tệp bắt đầu từ trang bìa của FHWA.

    [:material-file-download: **Tải sổ tay gốc (tiếng Anh, PDF)**](https://geoinst.github.io/assets/fhwa-mse-walls/fhwa-nhi-00-043-original.pdf){ .md-button }

    **Ấn bản hiện hành.** Sổ tay đã được tái bản thành **GEC-11**, *Design and
    Construction of Mechanically Stabilized Earth Walls and Reinforced Soil
    Slopes* — **FHWA-NHI-10-024** (Tập I) và **FHWA-NHI-10-025** (Tập II), do
    Phòng Cầu và Kết cấu FHWA phát hành.

=== "Tiếng Việt — bản dịch"

    Đây là **bản dịch tiếng Việt** của tài liệu tóm lược: toàn bộ chín chương cùng
    phần phụ lục được trình bày song song với bản tiếng Anh
    [tại đây](../../../reference-manuals/fhwa-mse-walls/index.md).

---

## Ý tưởng cốt lõi

Đất có cốt không phải là một bức tường có mặt ốp; nó là một **vật liệu hỗn hợp**.
Một loại đất đắp có ma sát — gần như không chịu được kéo — được kết hợp với các
phần tử cốt gia cường — gần như không chịu được nén. Kết hợp lại, chúng tạo thành
một khối ứng xử như thể có *lực dính biểu kiến* — đủ mạnh để đứng ở góc dốc lớn,
hoặc thẳng đứng như một bức tường, mà không cần khối bê tông lớn hay các phần tử
kết cấu nặng nề của tường chắn thông thường.

> **Ma sát mang tải trọng.** Cốt gia cường không được neo vào một kết cấu cứng;
> nó được *đất giữ lại*. Mọi phương trình thiết kế trong sổ tay này — sức kháng
> nhổ, cường độ mối nối, ổn định nội bộ — suy cho cùng đều là phát biểu về việc
> huy động ma sát giữa đất và cốt gia cường.
