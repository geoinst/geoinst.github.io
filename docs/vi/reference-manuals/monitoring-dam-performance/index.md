---
lang: vi
lang_alt: reference-manuals/monitoring-dam-performance/
---
# Monitoring Dam Performance: Instrumentation and Measurements

!!! note "Về tài liệu tham khảo này"
    Đây là một **tài liệu kỹ thuật mở, nguyên bản** về giám sát hiệu năng đập
    (dam-performance monitoring), được viết bằng ngôn ngữ kỹ thuật đơn giản, và
    được chuyển soạn từ cấu trúc cũng như phạm vi chủ đề của *Monitoring Dam
    Performance: Instrumentation and Measurements* — **ASCE Manual of Practice
    No. 135 (2019)**, do Ban Nhiệm vụ ASCE/EWRI về Thiết bị Quan trắc và Giám sát
    Đập và Đê biên soạn. Nó **không** phải là bản sao chép của văn bản ASCE được
    bảo hộ bản quyền. Tài liệu được cung cấp phục vụ giáo dục và sử dụng tại hiện
    trường, và mỗi con đập đều là duy nhất: hướng dẫn ở đây nhằm xây dựng năng lực
    phán đoán kỹ thuật, chứ không để thiết lập các tiêu chuẩn tối thiểu.

**An toàn đập** (dam safety) phụ thuộc vào việc hiểu rõ con đập thực sự vận hành
như thế nào. Giám sát là môn khoa học đo lường hành vi đó — thông qua cả quan sát
của con người lẫn thiết bị — và chuyển những phép đo đó thành các quyết định kịp
thời, có thể bảo vệ được. Tài liệu tham khảo này đi qua toàn bộ vòng đời của một
chương trình giám sát: từ xác định những gì có thể xảy ra sai sót, đến lựa chọn
và lắp đặt thiết bị, đến thu thập, đánh giá và hành động dựa trên dữ liệu.

---

## Phạm vi của tài liệu tham khảo này

Cuốn sách này bao quát các nguyên lý cơ bản và thực tiễn hiện hành về giám sát
hiệu năng của các con đập (và mở rộng ra, các công trình phụ trợ, nền móng và hồ
chứa của chúng). Nó được tổ chức thành các chương sau:

| # | Chương | Nội dung bao quát |
|---|---------|----------------|
| 1 | [Giới thiệu: Mục đích, Phạm vi và Cấu trúc](chapter-01-introduction.md) | Tại sao giám sát quan trọng; tài liệu này được tổ chức như thế nào |
| 2 | [Hiệu năng Đập và Các Hình thức Hư hỏng Tiềm năng](chapter-02-failure-modes.md) | Cách đập hư hỏng và những dấu hiệu nào báo trước sự hư hỏng |
| 3 | [Triết lý Giám sát: Giám sát Trực quan và Thiết bị Quan trắc](chapter-03-philosophy.md) | Hai trụ cột của giám sát và cách chúng bổ trợ cho nhau |
| 4 | [Lập kế hoạch Chương trình Giám sát Đập](chapter-04-planning.md) | Một quy trình có cấu trúc để xác định cái gì, ở đâu, và tại sao cần giám sát |
| 5 | [Các Họ Thiết bị Quan trắc cho Đập](chapter-05-instruments.md) | Khảo sát, địa kỹ thuật, thủy văn và cảm biến kết cấu trong nháy mắt |
| 6 | [Áp kế (Piezometer) & Giám sát Áp lực Nước Lỗ rỗng](chapter-06-piezometers.md) | Bão hòa, lắp đặt và đọc áp lực nước lỗ rỗng |
| 7 | [Giám sát Thấm, Rò rỉ và Bề mặt Thấm (Phreatic)](chapter-07-seepage.md) | Định lượng và diễn giải sự thấm |
| 8 | [Giám sát Biến dạng: Khảo sát và Cảm biến Địa kỹ thuật](chapter-08-deformation.md) | Mốc khảo sát, inclinometer, extensometer, tiltmeter |
| 9 | [Hệ thống Tự động, Từ xa và Thời gian Thực](chapter-09-automated.md) | Bộ ghi dữ liệu, viễn thông, ngưỡng và báo động |
| 10 | [Lắp đặt, Vận hành và Bảo trì](chapter-10-iom.md) | Có được dữ liệu tin cậy suốt tuổi thọ thiết bị |
| 11 | [Thu thập, Quản lý Dữ liệu và Cơ sở Dữ liệu](chapter-11-data-management.md) | Tần suất, kiểm thực và các hệ thống dữ liệu |
| 12 | [Đánh giá, Trình bày và Diễn giải Dữ liệu](chapter-12-evaluation.md) | Biểu đồ, đường cơ sở và tách tín hiệu khỏi nhiễu |
| 13 | [Đánh giá Hiệu năng và Ra quyết định](chapter-13-decisions.md) | Từ bất thường đến hành động |
| 14 | [Các Bài học Lịch sử (Case Histories)](chapter-14-case-histories.md) | Bài học từ các chương trình giám sát thực tế |

---

## Cách sử dụng tài liệu tham khảo này

- **Bắt đầu với Chương 2 và Chương 4.** Các hình thức hư hỏng và một kế hoạch có
  cấu trúc là nền tảng của mọi chương trình giám sát tốt.
- **Liên kết với phần còn lại của kho kiến thức.** Chương [Các Họ Thiết bị](chapter-05-instruments.md)
  tham chiếu chéo với các tài liệu [Dunnicliff](../dunnicliff/index.md) và
  [FHWA](../fhwa/index.md) về các quy trình lắp đặt chi tiết.
- **Hãy hỏi [GTI Doctor](../../gti-doctor.md).** Trợ lý AI có thể trả lời các câu
  hỏi giám sát từ kho ngữ liệu rộng hơn.

---

## Ghi chú về đơn vị và thuật ngữ

Cả đơn vị SI và đơn vị thông dụng của Mỹ đều xuất hiện trong thực tế; tài liệu này
sử dụng hệ đơn vị phổ biến nhất cho từng chủ đề và nêu rõ sự quy đổi khi cần
thiết. "Performance" (hiệu năng) nghĩa là hành vi quan sát được của con đập so
với hành vi kỳ vọng của nó.

> **An toàn là trên hết.** Dữ liệu thiết bị hỗ trợ, nhưng không bao giờ thay thế,
> việc kiểm tra trực quan có đủ năng lực và phán đoán kỹ thuật của một kỹ sư đập
> có đủ năng lực hoặc chương trình an toàn đập của chủ đầu tư.
