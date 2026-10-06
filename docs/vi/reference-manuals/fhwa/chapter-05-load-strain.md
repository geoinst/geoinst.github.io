---
lang: vi
lang_alt: reference-manuals/fhwa/chapter-05-load-strain/
---
# Chương 5 — Tải, Ứng biến & Nhiệt độ

## 5.1 Giới thiệu

Chương này bàn về thiết bị đo **tải trọng** mà một cấu kiện chịu, **ứng biến** (và
do đó ứng suất) trong cấu kiện, cùng **nhiệt độ** ảnh hưởng đến cả hai. Những số đo
này then chốt với thí nghiệm tải móng sâu ([Chương 8](chapter-08-deep-foundations.md))
và với quan trắc thanh chống, neo và thanh giằng trong kết cấu chắn đất
([Chương 9](chapter-09-earth-retaining.md)).

## 5.2 Load cell

**Load cell** đo lực trong một cấu kiện mà nó được chèn vào hoặc đặt dưới:

- **Load cell thủy lực** — một tấm chứa đầy chất lỏng; tải tác dụng làm tăng áp lực
  chất lỏng, đọc bằng đồng hồ hoặc cảm biến. Bền và đơn giản.
- **Load cell điện trở** — tenzo dán lên cấu kiện chuyển tải thành tín hiệu điện.
- **Kích thủy lực có lỗ xuyên tâm đã hiệu chuẩn** — dùng để căng và đo tải trong các
  thao tác kéo căng (ví dụ neo và neo đá). Lưu ý: tải xác định từ áp lực chất lỏng
  trong kích có thể mang **sai số hệ thống** do ma sát, nên kích phải được **hiệu
  chuẩn**.

![Figure: dunnicliff-load-cell-strain-gage](../../../assets/figures/dunnicliff-load-cell-strain-gage.svg)

**Hình.** Load cell và tenzo: load cell thủy lực và điện đo lực cấu kiện, còn tenzo dán và dây rung đo ứng biến (theo FHWA-HI-98-034, Ch. 5).

## 5.3 Tenzo gắn trên bề mặt

- **Tenzo cơ học** — ví dụ tenzo **Demec**, đo sự thay đổi khoảng cách giữa hai đĩa
  chuẩn trên một bề mặt.
- **Tenzo dây rung gắn bề mặt** — hàn hoặc dán lên cấu kiện thép; bền và phù hợp quan
  trắc lâu dài.
- **Tenzo điện trở gắn bề mặt** — lá dán cho số đo ngắn hạn, độ phân giải cao.

**Quan hệ ứng biến–ứng suất:** chuyển ứng biến đo được thành ứng suất cần **mô đun
đàn hồi** của cấu kiện ($\sigma = E\varepsilon$). Phép chuyển đổi này là nguồn sai số
phổ biến và phải được xử lý minh bạch.

## 5.4 Tenzo chôn trong bê tông

- **Tenzo dây rung chôn** — đúc vào bê tông để đo ứng biến nội bộ lâu dài.
- **Tenzo điện trở chôn** — cho số đo ngắn hạn hơn.
- **Quan hệ ứng biến–ứng suất** — như trên, nhưng với bê tông cần lưu ý mô đun, từ
  biến và hiệu ứng nhiệt.

## 5.5 Thanh chị em (sister bar)

**Thanh chị em** là một đoạn thép gia cường ngắn được gắn tenzo dây rung, buộc song
song với cốt thép chính. Nó đo ứng biến của cốt thép tại vị trí đó, từ đó ước lượng
tải mà tiết diện bê tông chịu — một kỹ thuật chuẩn cho thí nghiệm tải và quan trắc
các tiết diện được lắp thiết bị.

## 5.6 Nhiều telltale để xác định ứng suất

**Nhiều telltale** — các neo ở nhiều độ sâu tham chiếu về một đầu chuẩn — phân giải
chuyển vị tương đối giữa các điểm, từ đó xác định **ứng biến** trong mỗi đoạn (và do
đó phân bố tải).

## 5.7 Đo nhiệt độ

Nhiệt độ ảnh hưởng đến thiết bị dây rung và thiết bị đo ứng biến, và chuyển vị nhiệt
có thể lấn át biến dạng đo được. Nhiệt độ được đo bằng:

- **Thermistor và cảm biến nhiệt điện trở (RTD)** — chính xác, dễ ghi log.
- **Cặp nhiệt điện (thermocouple)** — dải rộng, độ chính xác tuyệt đối thấp hơn.
- **Cảm biến nhiệt dây rung** — thuận tiện khi dùng chung bộ ghi với thiết bị ứng
  biến.

Thiết bị và bộ ghi nên ghi nhiệt độ cùng lúc với ứng biến để áp được **hiệu chỉnh
nhiệt**.

## 5.8 Các điểm then chốt cần ghi nhớ

- **Load cell** đo lực cấu kiện; **tenzo** đo ứng biến, chuyển thành ứng suất qua **mô
  đun đàn hồi**.
- **Hiệu chuẩn kích thủy lực** — số đọc áp lực chất lỏng mang sai số ma sát.
- **Thanh chị em** và **nhiều telltale** là cách thực tế để lắp thiết bị cho cốt thép
  và phân giải phân bố tải.
- Luôn ghi **nhiệt độ** cùng dữ liệu tải/ứng biến để hiệu chỉnh.
