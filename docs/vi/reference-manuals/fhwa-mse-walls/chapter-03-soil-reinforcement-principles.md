---
lang: vi
lang_alt: reference-manuals/fhwa-mse-walls/chapter-03-soil-reinforcement-principles/
---
# Chương 3 — Nguyên lý Cốt gia cường Đất & Thông số Thiết kế

## 3.1 Tổng quan

Chương này là cầu nối giữa việc chọn hệ thống và việc thiết kế nó. Nó trả lời hai
câu hỏi:

1. **Vì sao đất có cốt hoạt động được?** — cơ học tương tác.
2. **Những thông số nào đi vào các phương trình?** — các thông số đất, cốt gia cường
   và độ bền mà các chương thiết kế sử dụng.

## 3.2 Khái niệm đất có cốt

Một loại đất đắp có ma sát chịu được ứng suất nén và cắt, nhưng gần như không chịu
được kéo. Một phần tử cốt gia cường chịu được kéo, nhưng gần như không chịu được nén.
Kết hợp chúng, khối hỗn hợp có thể chịu một ứng suất *kéo* mà nó không thể chịu khi
đứng riêng — đó là lý do khối đất có cốt ứng xử như thể có **lực dính biểu kiến**, và
có thể đứng ở góc dốc hơn góc ma sát của đất đắp cho phép.

Hai cơ chế truyền tải mang tải trọng giữa đất và cốt gia cường:

- **Ma sát (và lực dính)** dọc theo bề mặt cốt — chi phối với dải liên tục và vải địa
  kỹ thuật.
- **Chịu ép bị động** của đất lên các thanh ngang — chi phối với lưới, lưới thanh và
  dải có gờ, và đóng góp đáng kể với lưới địa kỹ thuật.

Hệ quả thiết kế là **cơ chế nhổ**: cốt gia cường được đất giữ trên một *chiều dài
neo hữu hiệu* phía sau mặt trượt tiềm tàng, và lực kéo mà nó chịu bị giới hạn bởi ma
sát và sức chịu ép mà chiều dài đó huy động được.

## 3.3 Tương tác đất–cốt gia cường bằng các khái niệm chuẩn hóa

**Đánh giá hiệu năng nhổ.** Sức kháng nhổ được chuẩn hóa để so sánh được các hình học
cốt khác nhau. Sức kháng nhổ của một lớp được biểu diễn:

$$P_r = F^{*}\ \alpha\ \sigma_v\ L_e\ C\ R_c$$

trong đó $F^{*}$ là **hệ số ma sát nhổ** (đại lượng không thứ nguyên đo tương tác
đất–cốt), $\alpha$ là **hệ số hiệu chỉnh tỷ lệ**, $\sigma_v$ là ứng suất hữu hiệu
thẳng đứng, $L_e$ là chiều dài neo hữu hiệu phía sau mặt trượt, $C$ là chu vi cốt
(hay chu vi hữu hiệu), và $R_c$ là **tỷ số phủ** (phần chiều rộng cốt thực sự tiếp
xúc với đất, nhỏ hơn 1 với lưới và lưới địa kỹ thuật có lỗ).

**Hệ số ma sát nhổ** $F^{*}$ thu được theo kinh nghiệm từ góc ma sát đo được của đất
và loại cốt, hoặc theo thực nghiệm từ thí nghiệm nhổ (Phụ lục A):

- **Cốt không dãn được (thép)** — $F^{*}$ suy ra từ góc ma sát của đất, với dải có gờ
  cộng thêm thành phần chịu ép bị động.
- **Cốt dãn được (địa kỹ thuật tổng hợp)** — $F^{*}$ kết hợp ma sát bề mặt với chịu
  ép bị động lên các thanh ngang; **hệ số hiệu chỉnh tỷ lệ** $\alpha$ kể đến việc cốt
  dãn được huy động ít hơn toàn bộ ma sát của nó trên chiều dài neo dài. $\alpha = 1.0$
  với cốt không dãn được; với vật liệu địa kỹ thuật tổng hợp, $\alpha$ lấy bằng 1.0
  gần bề mặt và giảm theo độ sâu (giá trị mặc định khoảng 0.8 thường được dùng).

**Ước lượng sức kháng nhổ trong kết cấu RSS và MSE.** Cùng biểu thức $P_r$ được dùng
cho cả hai kết cấu, nhưng *chiều dài neo hữu hiệu* $L_e$ được đo phía sau một mặt
trượt khác nhau — mặt trượt nội bộ với tường MSE và mặt trượt tới hạn với mái dốc có
cốt. Sức kháng sẵn có sau đó được so với lực kéo huy động:

$$FS_{(PO)} = \frac{P_r}{T_{max}}$$

với hệ số an toàn tối thiểu do tiêu chí thiết kế đặt ra (thường $FS_{(PO)} \ge 1.5$).

**Cắt mặt tiếp giáp.** Khi cốt gia cường cắt qua một mặt *trượt trực tiếp*, hoặc khi
mặt tiếp giáp giữa mặt tường và đất đắp có cốt phải truyền tải, thì **cường độ cắt
mặt tiếp giáp** chi phối. Nó được đặc trưng bằng một góc ma sát mặt tiếp giáp, thường
nhỏ hơn góc ma sát của chính đất, và phải được dùng ở mọi nơi có cơ chế trượt dọc một
mặt phẳng cốt là khả tín.

## 3.4 Thiết lập thông số kỹ thuật từ khảo sát và thí nghiệm hiện trường

**Đất nền.** Nền bên dưới khối đất có cốt chịu trọng lượng của toàn bộ kết cấu và
phải thỏa mãn điều kiện chịu tải, trượt, lún và ổn định tổng thể. Thông số cần thiết:
trọng lượng đơn vị, cường độ kháng cắt (thoát nước và không thoát nước), tính nén và
độ sâu tới tầng chịu tải tốt.

**Đất đắp có cốt.** Đất đắp có cốt là một **vật liệu kết cấu**, không chỉ là đất đắp.
Nó phải có ma sát và thoát nước tự do. Định mức kỹ thuật thường giới hạn:

- **Hàm lượng hạt mịn** và **chỉ số dẻo** (hạt mịn dẻo làm giảm ma sát và thoát nước
  kém).
- **Độ hạt** (để đảm bảo thoát nước và khả năng thi công).
- **Đầm chặt** (để đạt góc ma sát thiết kế và hạn chế lún).

Một loại đất hạt rời điển hình có thể có góc ma sát 34°–40°; giá trị thiết kế phải
được chứng minh bằng thí nghiệm, không được giả định.

**Đất lưng tường.** Đất phía sau vùng có cốt sinh ra áp lực đất mà kết cấu phải chống
lại. Trọng lượng đơn vị và góc ma sát của nó là thông số đầu vào cho ổn định ngoài,
và khả năng thoát nước của nó quyết định có phải cộng thêm áp lực thủy tĩnh hay không.

**Tính điện hóa.** Với cốt **thép**, tính xâm thực của đất đắp chi phối chiều dày ăn
mòn và yêu cầu lớp phủ; sổ tay giới hạn pH, điện trở suất, clorua, sunphat và hàm
lượng hữu cơ. Với cốt **địa kỹ thuật tổng hợp**, tính hóa học chi phối độ bền polyme,
và các giới hạn cũng được áp dụng. Những giới hạn này là lý do "đất hạt rời nào cũng
được" là chưa đủ.

## 3.5 Thiết lập thông số thiết kế kết cấu

**Đặc trưng hình học.** Chiều rộng cốt, khoảng cách (đứng và ngang), chiều dài, diện
tích mặt cắt, và (với lưới) hình học lỗ và kích thước thanh. Với thép, mặt cắt bị
giảm trong tuổi thọ thiết kế do ăn mòn (xem dưới).

**Đặc trưng cường độ.** Cường độ thiết kế của cốt là cường độ **dài hạn**, không phải
cường độ cực hạn ngắn hạn:

- **Thép** — cường độ kéo thiết kế là cường độ chảy của mặt cắt *còn lại* sau khi trừ
  **tổn thất ăn mòn hy sinh** trong tuổi thọ thiết kế. Phải kể cả tổn thất lớp mạ kẽm
  lẫn tổn thất thép cacbon, với tốc độ phụ thuộc tính điện hóa của đất đắp.
- **Địa kỹ thuật tổng hợp** — cường độ kéo cho phép là cường độ cực hạn giảm bởi các
  hệ số thành phần:

$$T_{allow} = \frac{T_{ult}}{RF_{CR}\ \cdot\ RF_{ID}\ \cdot\ RF_{D}}$$

trong đó $RF_{CR}$ là hệ số giảm do **từ biến**, $RF_{ID}$ do **hư hại khi thi công**,
và $RF_{D}$ do **độ bền** (lão hóa hóa học/sinh học). Sổ tay cung cấp các giá trị mặc
định (Bảng 11) chỉ được dùng khi cốt và đất đắp đạt các yêu cầu tối thiểu quy định;
nếu không, các hệ số phải được xác lập bằng thí nghiệm — từ biến bằng ngoại suy ứng
suất–phá hoại (Phụ lục B), hư hại khi thi công bằng thí nghiệm hư hại hiện trường, và
độ bền bằng thí nghiệm ngâm.

**Cường độ mối nối.** Khi cốt được nối cơ học với mặt tường, **cường độ mối nối**
(có thể thấp hơn cường độ của chính cốt) sẽ chi phối, và phải được xác lập bằng thí
nghiệm mối nối — xem [Chương 4](chapter-04-design-mse-walls.md) và Phụ lục A.

## 3.6 Các điểm then chốt cần ghi nhớ

- Khối hỗn hợp hoạt động được vì **ma sát và chịu ép bị động** giữ cốt; mọi phương
  trình cường độ đều là phát biểu về lực giữ đó.
- Chuẩn hóa sức kháng nhổ thành $P_r = F^{*}\alpha\sigma_v L_e C R_c$, và kiểm
  $FS_{(PO)} = P_r/T_{max}$ theo giá trị tối thiểu thiết kế.
- **Đất đắp có cốt là vật liệu kết cấu** — phải đặc thù hóa độ hạt, độ dẻo, đầm chặt
  và tính điện hóa.
- Dùng cường độ cốt **dài hạn**: thép mất mặt cắt do ăn mòn; vật liệu địa kỹ thuật
  tổng hợp mất cường độ do từ biến, hư hại khi thi công và lão hóa.
- Xác lập các hệ số giảm bằng **thí nghiệm**, trừ khi thỏa mãn các điều kiện tiên
  quyết để dùng giá trị mặc định.
