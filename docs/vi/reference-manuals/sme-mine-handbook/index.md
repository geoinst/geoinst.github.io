---
lang: vi
lang_alt: reference-manuals/sme-mine-handbook/
---
# Sổ tay Kỹ thuật Mỏ SME — Thiết bị Quan trắc Địa kỹ thuật (Chương 8.5)

!!! note "Về tài liệu tham khảo này"
    Trang này là **bản tổng hợp mở, nguyên bản** của **Chương 8.5 — *Geotechnical
    Instrumentation*** trong **Sổ tay Kỹ thuật Mỏ SME** (ấn bản lần 3), do **Erik
    Eberhardt** (Đại học British Columbia) và **Doug Stead** (Đại học Simon Fraser)
    biên soạn. Đây là bản tóm lược cấp chương — **không phải** bản sao nguyên văn
    tài liệu có bản quyền. Sổ tay do Hiệp hội Khai khoáng, Luyện kim và Thăm dò
    Hoa Kỳ (SME) xuất bản; chương gốc cùng các hình vẽ vẫn thuộc bản quyền của các
    tác giả và nhà xuất bản. Bản tổng hợp này nhằm mục đích giáo dục và định
    hướng; bản dịch tiếng Việt đầy đủ được cung cấp kèm theo, và bản PDF tiếng Anh
    gốc được tái bản tại đây để tiện đối chiếu.

**Chương 8.5, *Thiết bị Quan trắc Địa kỹ thuật***, là một trong những khảo sát hiện
đại được trích dẫn nhiều nhất về thực hành quan trắc trong khai thác mỏ. Chương
gồm **21 trang** (tr. 551–570), được viết bởi hai trong số những học giả hàng đầu
về cơ học đá, và được tổ chức xoay quanh một ý tưởng duy nhất: thiết bị đo phục vụ
**hai chức năng rất khác nhau** — chức năng *điều tra* (thu thập các thông số đầu
vào mà mô hình thiết kế cần) và chức năng *giám sát* (quan sát cách nền đá thực sự
đáp ứng, và cảnh báo khi nó đi chệch khỏi thiết kế).

Chính cách đặt vấn đề đó làm cho chương này hữu ích. Thay vì một danh mục thiết bị,
nó được viết như một **chuỗi quyết định**: bạn đang cần trả lời câu hỏi gì, thông
số nào trả lời được câu hỏi đó, thiết bị nào đo được thông số ấy với dải đo, độ
phân giải, độ chính xác và độ tin cậy đủ dùng — và làm cách nào để đưa dữ liệu về
một dạng mà con người có thể hành động được.

---

## Phạm vi tài liệu tham khảo này

| # | Phần | Nội dung |
|---|------|----------|
| 1 | **Mở đầu** | Chức năng điều tra và chức năng giám sát; bảy tiêu chí chọn thiết bị — dải đo, độ phân giải, độ chính xác, độ chụm, sự phù hợp, sự bền bỉ, độ tin cậy |
| 2 | **Thiết bị cho công tác điều tra** | Kỹ thuật lỗ khoan (định hướng mẫu lõi, televiewer, địa vật lý lỗ khoan); viễn thám (LiDAR, ảnh số); địa vật lý mặt đất; đặc trưng hóa nước ngầm (áp kế, thử nghiệm dòng chảy); đo ứng suất tại chỗ (overcoring, nứt thủy lực) |
| 3 | **Thiết bị cho công tác giám sát** | Quy trình 20 bước lập kế hoạch của Dunnicliff; các kiểu bộ chuyển đổi; chuyển vị bề mặt (trắc địa/toàn đạc robot, GPS); thiết bị đo biến dạng sâu; cảm biến đo độ nghiêng; chuyển vị trong lỗ khoan (thiết bị đo nghiêng kiểu đầu dò và cố định, thiết bị đo biến dạng sâu trong lỗ khoan, hệ thống đo hội tụ, dãy cảm biến gia tốc định hình, TDR, sợi quang); viễn thám biến dạng (InSAR, radar mái dốc, LiDAR/ảnh số); hộp đo áp lực; vi địa chấn |
| 4 | **Thu thập và trình bày dữ liệu** | Truyền dữ liệu không dây; đắm mình trong dữ liệu và trực quan hóa; mô hình dữ liệu mỏ tích hợp |
| 5 | **Tài liệu tham khảo** | Danh mục 64 mục, trải rộng các phương pháp khuyến nghị của ISRM, các hội thảo ổn định mái dốc của SAIMM và các tạp chí chuyên ngành chính |

Chương được minh họa bằng **14 hình** và **5 bảng**, tất cả đều được đưa vào bản
dịch tiếng Việt bên dưới.

---

## Tài liệu đầy đủ (PDF)

=== "Tiếng Việt — bản dịch đầy đủ (Times New Roman)"

    **Bản dịch tiếng Việt đầy đủ — Chương 8.5** (29 trang, khổ A4).
    Bản dịch trọn vẹn toàn bộ Chương 8.5, gồm **5 bảng** và **14 hình minh họa**,
    kèm toàn bộ danh mục tài liệu tham khảo. Thuật ngữ được chuẩn hóa theo **TCVN**
    (áp kế, thiết bị đo biến dạng sâu, ống đo nghiêng, hộp đo áp lực…), trình bày
    bằng phông **Times New Roman**.

    [:material-file-download: **Tải PDF bản dịch tiếng Việt (đầy đủ)**](https://geoinst.github.io/assets/sme-mine-handbook/sme-mine-handbook-ch85-vietnamese.pdf){ .md-button .md-button--primary }

=== "Tiếng Anh — chương gốc (PDF)"

    **Chương gốc tiếng Anh** — *Sổ tay Kỹ thuật Mỏ SME, Chương 8.5: Thiết bị Quan
    trắc Địa kỹ thuật* (21 trang, tr. 551–570), tác giả Erik Eberhardt và Doug
    Stead. Tài liệu được tái bản ở đây đúng như ấn bản của Hiệp hội Khai khoáng,
    Luyện kim và Thăm dò Hoa Kỳ (SME).

    [:material-file-download: **Tải chương gốc Chương 8.5 (tiếng Anh, PDF)**](https://geoinst.github.io/assets/sme-mine-handbook/sme-mine-handbook-ch85-original-en.pdf){ .md-button }
    &nbsp;
    [Trang nhà xuất bản — SME](https://www.smenet.org/){ target=_blank }

---

## Vì sao chương này quan trọng trong cơ sở tri thức

Chương 8.5 là **phần đối tác phía khai thác mỏ** của toàn bộ tư liệu phía dân dụng
mà thư viện này được xây dựng trên đó:

- **Khung tiêu chí lựa chọn** của nó (dải đo, độ phân giải, độ chính xác, độ chụm,
  sự phù hợp, sự bền bỉ, độ tin cậy) chính là vốn từ vựng mà trang này sử dụng mỗi
  khi đặc tả một thiết bị — xem [Bắt đầu](../../getting-started/index.md).
- **Bảng các kiểu bộ chuyển đổi** (LVDT, dây rung, gia tốc kế, sợi quang, MEMS)
  giải thích *vì sao* mỗi thiết bị lại hành xử như vậy, và là phần bạn đồng hành tự
  nhiên của các bản tổng hợp [Dunnicliff](../dunnicliff/index.md) và
  [FHWA](../fhwa/index.md).
- **Quy trình 20 bước của Dunnicliff** là trục tổ chức đứng sau
  [kiến trúc sáu lớp ADAQS](../../adaqs/index.md) trung lập nhà cung cấp của trang này.
- Các phần về **ứng suất tại chỗ** và **áp kế** cung cấp nền tảng cơ học đá và nước
  ngầm, trong khi [Cơ học đất](../soil-mechanics/index.md) và
  [Kỹ thuật Nền móng](../foundation-engineering/index.md) tiếp cận cùng vấn đề từ
  phía đất.

---

## Cách sử dụng

- **Đọc các tiêu chí lựa chọn trước** (phần 1). Hầu hết các thất bại của thiết bị đo
  là thất bại trong đặc tả kỹ thuật, chứ không phải thất bại của cảm biến.
- Dùng **bảng 20 bước của Dunnicliff** như một bảng kiểm trước khi mua bất cứ thứ
  gì — các bước 1–8 là những bước thường bị bỏ qua nhất.
- Thực hiện **điều tra trước, giám sát sau**: chương nêu rõ rằng giám sát mang tính
  dự báo nên được triển khai sau một giai đoạn giám sát điều tra.
- Đi theo các liên kết chéo sang [Dunnicliff](../dunnicliff/index.md),
  [FHWA](../fhwa/index.md), [Giám sát hiệu năng đập](../monitoring-dam-performance/index.md)
  và [An toàn đập thải](../tailings-dam-safety/index.md) để có chiều sâu phía dân dụng.
- Hỏi [GTI Doctor](../../gti-doctor.md) để trích xuất chi tiết từ kho tư liệu rộng hơn.

> **An toàn và tính thời sự.** Công nghệ viễn thám và cảm biến không dây đã tiến bộ
> đáng kể kể từ khi chương này được viết — chu kỳ lặp lại của InSAR, độ chính xác
> của radar và khả năng cảm biến sợi quang phân bố đều tiếp tục được cải thiện. Hãy
> coi các **nguyên lý và logic lựa chọn** là bền vững, và **kiểm tra đặc tính kỹ
> thuật hiện hành** của thiết bị với nhà cung cấp trước khi dùng cho thiết kế hoặc
> hồ sơ tuân thủ.
