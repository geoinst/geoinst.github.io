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

## 5.2 Cảm biến đo tải trọng (Load Cell)

**Cảm biến đo tải trọng (Load Cell)** đo lực trong một cấu kiện mà nó được chèn vào hoặc đặt dưới:

- **Cảm biến đo tải trọng thủy lực** — một tấm chứa đầy chất lỏng; tải tác dụng làm tăng áp lực
  chất lỏng, đọc bằng đồng hồ hoặc cảm biến. Bền và đơn giản.
- **Cảm biến đo tải trọng điện trở** — cảm biến đo biến dạng (strain gauge) dán lên cấu kiện chuyển tải thành tín hiệu điện.
- **Kích thủy lực có lỗ xuyên tâm đã hiệu chuẩn** — dùng để căng và đo tải trong các
  thao tác kéo căng (ví dụ neo và neo đá). Lưu ý: tải xác định từ áp lực chất lỏng
  trong kích có thể mang **sai số hệ thống** do ma sát, nên kích phải được **hiệu
  chuẩn**.

![Figure: dunnicliff-load-cell-strain-gage](../../../assets/figures/dunnicliff-load-cell-strain-gage.svg)

**Hình.** Cảm biến đo tải trọng và cảm biến đo biến dạng: cảm biến đo tải trọng đo lực cấu kiện, còn cảm biến đo biến dạng dán và dây rung đo biến dạng (theo FHWA-HI-98-034, Ch. 5).

## 5.3 Cảm biến đo biến dạng gắn trên bề mặt

- **Cảm biến đo biến dạng cơ học** — ví dụ **cảm biến đo biến dạng Demec (Demec Gauge)**, đo sự thay đổi khoảng cách giữa hai đĩa
  chuẩn gắn trên bề mặt kết cấu.
- **Cảm biến đo biến dạng dây rung gắn bề mặt** — hàn hoặc dán lên cấu kiện thép; bền và phù hợp quan
  trắc lâu dài.
- **Cảm biến đo biến dạng điện trở gắn bề mặt** — lá điện trở dán cho số đo ngắn hạn, độ phân giải cao.

**Quan hệ biến dạng–ứng suất:** chuyển biến dạng đo được thành ứng suất cần **mô đun
đàn hồi** của cấu kiện ($\sigma = E\varepsilon$). Phép chuyển đổi này là nguồn sai số
phổ biến và phải được xử lý minh bạch.

## 5.4 Cảm biến đo biến dạng chôn trong bê tông

- **Cảm biến đo biến dạng dây rung chôn** — đúc trực tiếp vào bê tông để đo biến dạng nội bộ lâu dài.
- **Cảm biến đo biến dạng điện trở chôn** — dùng cho các phép đo ngắn hạn hơn.
- **Quan hệ biến dạng–ứng suất** — như trên, nhưng với bê tông cần lưu ý mô đun đàn hồi, từ
  biến và hiệu ứng nhiệt độ.

## 5.5 Thanh thép đo biến dạng phụ (Sister Bar)

**Thanh thép đo biến dạng phụ (Sister Bar)** là một đoạn thép gia cường ngắn có kích thước và đặc tính cơ lý tương đương cốt thép chủ của công trình, được gắn sẵn cảm biến đo biến dạng dây rung (vibrating wire strain gauge) ở chính giữa. Khi lắp đặt, thanh thép phụ này được buộc song song và áp sát vào thanh cốt thép chủ trong lồng thép trước khi đổ bê tông. Nó cùng chịu biến dạng với cốt thép chủ tại vị trí đó, từ đó giúp kỹ sư tính toán chính xác ứng suất và tải trọng mà tiết diện bê tông đang gánh chịu — một kỹ thuật tiêu chuẩn cho thí nghiệm tải móng sâu và quan trắc tường vây, cọc khoan nhồi, vỏ hầm.

## 5.6 Nhiều thanh truyền chuyển vị (telltale) để xác định biến dạng và tải trọng

**Cụm thanh truyền chuyển vị (Multiple Telltales)** — các mỏ neo ở nhiều độ sâu tham chiếu về một đầu chuẩn ở miệng cọc — phân giải
chuyển vị tương đối giữa các đoạn cọc, từ đó xác định **biến dạng** trong mỗi đoạn (và do
đó xác định được phân bố truyền tải dọc trục).

## 5.7 Đo nhiệt độ

Nhiệt độ ảnh hưởng đến thiết bị dây rung và cảm biến đo biến dạng, và biến dạng do nhiệt
có thể lấn át biến dạng do tải trọng. Nhiệt độ được đo bằng:

- **Thermistor và cảm biến nhiệt điện trở (RTD)** — chính xác, dễ kết nối bộ ghi dữ liệu.
- **Cặp nhiệt điện (thermocouple)** — dải đo rộng, độ chính xác tuyệt đối thấp hơn.
- **Cảm biến nhiệt tích hợp trong đầu đo dây rung** — thuận tiện khi dùng chung kênh đo với tín hiệu biến dạng.

Thiết bị và bộ ghi dữ liệu nên ghi nhiệt độ cùng lúc với biến dạng để áp dụng **hiệu chỉnh
nhiệt độ**.

## 5.8 Các điểm then chốt cần ghi nhớ

- **Cảm biến đo tải trọng (Load Cell)** đo lực cấu kiện; **cảm biến đo biến dạng (strain gauge)** đo biến dạng, chuyển thành ứng suất qua **mô
  đun đàn hồi** ($E$).
- **Hiệu chuẩn kích thủy lực** — số đọc áp lực chất lỏng luôn mang sai số ma sát nội bộ.
- **Thanh thép đo biến dạng phụ (Sister Bar)** và **thanh truyền chuyển vị (telltale)** là phương pháp tiêu chuẩn để lắp thiết bị cho cốt thép
  và phân giải phân bố truyền tải dọc thân cọc.
- Luôn ghi nhận **nhiệt độ** đồng thời với dữ liệu tải/biến dạng để hiệu chỉnh nhiệt.
