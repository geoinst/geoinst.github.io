---
lang: vi
lang_alt: reference-manuals/geotechnical-engineers-handbook/chapter-12-geo-informatics/
---
# Chương 12 — Công nghệ thông tin ứng dụng trong địa kỹ thuật

Chương XII khép lại cuốn sách bằng vai trò của công nghệ thông tin —
*géo-informatique* — trong công tác địa kỹ thuật. Thông điệp của chương rất chừng mực:
công nghệ thông tin đã thay đổi cách xử lý số liệu, nhưng không thể thay thế người kỹ sư.

!!! note "Về các mục bổ sung kỹ thuật 12.3 và 12.4"
    Ngoài phần tóm lược nội dung sách, chương này có thêm hai mục do ban biên tập soạn
    nhằm mô tả **chi tiết hơn về công nghệ thông tin** đứng sau một hệ quan trắc tự động
    và sau một chương trình phân tích. Nội dung bổ sung mang tính kỹ thuật chung, **không
    gắn với bất kỳ nhà cung cấp, thương hiệu hay sản phẩm cụ thể nào**.

## 12.1 Luận điểm

Trong mấy thập kỷ gần đây, công nghệ thông tin phát triển mạnh mẽ và thâm nhập vào mọi
lĩnh vực, địa kỹ thuật cũng không phải ngoại lệ. Nhưng **đất là vật liệu rất phức tạp** —
nhiều yếu tố tác động lẫn nhau, không đồng nhất, dị hướng. Các bài toán địa kỹ thuật, cả
trong khảo sát (thí nghiệm, thu thập số liệu, đánh giá và lựa chọn đặc trưng) lẫn trong
phân tích (tương tác đất – kết cấu), **không thể giải bằng một mô hình hay một công thức
duy nhất**. Có những chương trình phân tích tổng quát, nhưng chúng luôn cần sự can thiệp
của nhà chuyên môn địa kỹ thuật.

Lời cảnh báo của sách: máy tính làm cho việc xử lý số liệu nhanh chóng, thuận tiện và
chính xác, đưa nhiều kết quả ra chỉ một lần bấm menu — nhưng **chỉ có kiến thức, kinh
nghiệm và sự nắm bắt kỹ thuật mới tìm ra giải pháp tốt nhất** và chọn được thông số đại
diện. Phần mềm hoàn thành nhanh một ý tưởng tốt; nó không tạo ra ý tưởng.

## 12.2 Ứng dụng công nghệ thông tin trong khảo sát đất nền

### 12.2.1 Khái quát về tiến trình khảo sát đất nền

Một đợt khảo sát là một **chuỗi chuyển hoá dữ liệu**: hiện trường → mẫu → thí nghiệm →
chỉ tiêu → thông số thiết kế. Mỗi mắt xích đều có thể được tin học hoá, nhưng sai số sinh
ra ở mắt xích nào thì các mắt xích sau không sửa được.

### 12.2.2 Các loại công việc liên quan đến sử dụng tin học

Có thể chia thành bốn nhóm:

1. **Thu thập** — nhập số liệu hiện trường, nhật ký hố khoan, kết quả thí nghiệm.
2. **Quản lý** — cơ sở dữ liệu khảo sát, liên kết mẫu ↔ hố khoan ↔ lớp đất ↔ thí nghiệm.
3. **Xử lý và trình bày** — vẽ biểu đồ, hiệu chỉnh, nội suy, lập mặt cắt.
4. **Phân tích** — tương quan giữa các loại thí nghiệm, thống kê đặc trưng, chọn thông số.

### 12.2.3 Những ứng dụng của công nghệ thông tin

**a) Nhập liệu và chuẩn hoá.** Biểu mẫu điện tử thay cho sổ tay giấy: mỗi trường dữ liệu
có kiểu, đơn vị và miền giá trị hợp lệ, nên lỗi đơn vị (kN/m² ↔ kPa ↔ T/m²) bị chặn ngay
khi nhập thay vì phát hiện khi đã thiết kế xong.

**b) Cơ sở dữ liệu khảo sát.** Đơn vị dữ liệu cơ bản là **hố khoan**, liên kết với các
**lớp đất**, **mẫu**, **thí nghiệm hiện trường** và **thí nghiệm trong phòng**. Khi dữ liệu
được tổ chức theo quan hệ như vậy, cùng một nguồn số liệu có thể xuất ra: mặt cắt địa chất,
bảng tổng hợp chỉ tiêu, biểu đồ phân bố, và hồ sơ bàn giao — mà không phải nhập lại.

**c) Vẽ và phân tích biểu đồ.** Tin học hoá khâu vẽ giải phóng người kỹ sư khỏi công việc
thủ công, nhưng đồng thời tạo ra một cám dỗ mới: **vẽ nhiều thứ mà không kiểm tra**. Biểu
đồ càng đẹp càng dễ khiến người đọc quên rằng nó chỉ đúng bằng số liệu đầu vào.

**d) Tương quan giữa các loại thí nghiệm.** Tương quan thực nghiệm (ví dụ $N_{SPT}$ ↔
$s_u$ ↔ $q_c$) là công cụ mạnh, nhưng mỗi tương quan chỉ đúng trong **phạm vi đất và điều
kiện đã xây dựng nên nó**. Phần mềm có thể tính tương quan cho mọi loại đất; người kỹ sư
phải biết khi nào tương quan đó vô nghĩa.

**e) Số hoá tài liệu cũ.** Quét và nhập lại hồ sơ khảo sát cũ cho phép tái sử dụng dữ liệu
lịch sử — thường là tài sản kỹ thuật có giá trị nhất mà một dự án thừa hưởng, và thường
cũng là thứ dễ thất lạc nhất.

## 12.3 Công nghệ thu thập dữ liệu tự động — sáu lớp của một hệ quan trắc

*(Mục bổ sung — mô tả chi tiết kỹ thuật, không gắn với sản phẩm cụ thể.)*

Giá trị của một hệ quan trắc tự động **không nằm ở cảm biến**, mà nằm ở khả năng đo đúng,
truyền về đủ, phát hiện bất thường sớm và lưu được bằng chứng. Có thể mô tả hệ thống như
một chuỗi sáu lớp, mỗi lớp trả lời một câu hỏi kỹ thuật riêng.

```mermaid
flowchart LR
    L1["1 · Cảm biến<br/>biến đại lượng vật lý<br/>thành tín hiệu điện"]
    L2["2 · Thu thập<br/>đầu ghi dữ liệu<br/>kích thích · lấy mẫu · đệm"]
    L3["3 · Truyền dẫn<br/>hữu tuyến / vô tuyến<br/>định tuyến · gửi lại"]
    L4["4 · Nền tảng dữ liệu<br/>chuỗi thời gian<br/>kiểm tra chất lượng"]
    L5["5 · Phân tích<br/>ngưỡng · xu hướng<br/>cảnh báo tự động"]
    L6["6 · Hồ sơ<br/>báo cáo · nhật ký<br/>bằng chứng tuân thủ"]
    L1 --> L2 --> L3 --> L4 --> L5 --> L6
```

### 12.3.1 Lớp 1 — Cảm biến và giao diện tín hiệu

Đây là lớp quyết định **độ chính xác có thể đạt được**; các lớp sau chỉ giữ nguyên hoặc
làm mất đi độ chính xác đó. Bốn họ giao diện tín hiệu thường gặp:

| Giao diện | Nguyên lý | Ưu điểm | Điểm cần lưu ý |
| --- | --- | --- | --- |
| **Dây rung** (vibrating wire) | Tần số dao động của dây căng thay đổi theo biến dạng | Tín hiệu **tần số**, ít suy hao trên cáp dài; ổn định lâu dài | Cần xung kích thích; phải **bù nhiệt** |
| **Cầu điện trở** (strain gauge) | Điện trở thay đổi theo biến dạng | Độ chính xác cao, dải đo rộng | Nhạy nhiễu; cáp nên ngắn; cần bù nhiệt |
| **4–20 mA** | Dòng điện tỷ lệ với đại lượng đo | Chuẩn công nghiệp, chống nhiễu tốt, truyền xa | Cần nguồn vòng; chỉ đo một chiều |
| **Số / bus** (SDI-12, Modbus, RS-485) | Truyền số trực tiếp, nhiều cảm biến trên một bus | Chống nhiễu, ghép nối đơn giản, có địa chỉ hoá | Cần quản lý địa chỉ và giao thức |

Hai họ ít gặp hơn nhưng đáng biết: **cảm biến quang** (cách tử Bragg / tán xạ, chống nhiễu
điện từ hoàn toàn và đo được phân tán dọc tuyến — phù hợp công trình dài như đập, đường
hầm) và **MEMS** (nhỏ, rẻ, dùng cho đo nghiêng và gia tốc, nhưng **trôi điểm không** nên
phải hiệu chuẩn định kỳ).

Một yêu cầu bị bỏ qua nhiều nhất: **mỗi cảm biến phải có mã định danh duy nhất và chứng
chỉ hiệu chuẩn**. Không có hai thứ đó thì dữ liệu đúng vẫn không dùng được làm bằng chứng.

### 12.3.2 Lớp 2 — Thu thập: đầu ghi dữ liệu

Đầu ghi là nơi các quyết định kỹ thuật biến thành thông số cấu hình:

- **Số kênh và kiểu kênh** — một thiết bị thường trộn nhiều loại kênh (dây rung, cầu điện
  trở, 4–20 mA, đếm xung, nhiệt điện trở).
- **Tần số lấy mẫu** — phải đủ dày để không bỏ sót biến động nhanh. Trong tình huống khẩn
  cấp, tần suất có thể lên tới **4 lần/giờ**; nếu hệ thống chỉ ghi 1 lần/ngày thì đã cấu
  hình sai ngay từ đầu.
- **Độ phân giải và thời gian lấy trung bình** — lấy trung bình nhiều mẫu làm giảm nhiễu
  nhưng **san phẳng đỉnh**; với bài toán cảnh báo, đỉnh mới là thứ cần thấy.
- **Đồng bộ thời gian** — không đồng bộ thì dữ liệu của nhiều thiết bị không so sánh được.
- **Chống sét lan truyền**, **pin dự phòng** và **bộ nhớ đệm**. Bộ nhớ đệm là chi tiết nhỏ
  nhưng quyết định: mất dữ liệu thường xảy ra **đúng vào lúc sự cố** — khi mất điện hoặc
  mất kết nối.

### 12.3.3 Lớp 3 — Truyền dẫn

| Phương thức | Khoảng cách | Băng thông | Chi phí | Lưu ý |
| --- | --- | --- | --- | --- |
| **Hữu tuyến** (RS-485, cáp quang) | ~1,2 km mỗi đoạn | Trung bình – cao | Thấp – trung bình | Ổn định nhất; khó thi công qua địa hình phức tạp; phải chống sét |
| **Vô tuyến VHF/UHF** | 1 – 20 km (tuỳ địa hình) | Thấp – trung bình | Trung bình | Phụ thuộc địa hình; có thể cần giấy phép tần số |
| **Mạng lưới** (mesh) | Mở rộng theo số nút | Thấp | Trung bình | Tự chữa lành khi một nút hỏng; cấu hình phức tạp hơn |
| **Di động 4G/LTE** | Nơi có phủ sóng | Cao | Thấp (theo gói dữ liệu) | Phụ thuộc nhà mạng; tốn điện, cần nguồn ổn định |
| **Vệ tinh** | Mọi nơi | Thấp | Cao | Dùng ở vùng không có hạ tầng mặt đất; độ trễ lớn |

Hai yêu cầu kỹ thuật tối thiểu: **cơ chế gửi lại** khi truyền thất bại, và **lưu đệm tại
chỗ** để dữ liệu không mất khi đường truyền gián đoạn.

### 12.3.4 Lớp 4 — Nền tảng dữ liệu

Dữ liệu quan trắc là **chuỗi thời gian**, và phải được lưu như chuỗi thời gian — không phải
như bảng tính. Bốn chức năng bắt buộc:

1. **Gắn dấu thời gian đồng bộ** cho mọi giá trị.
2. **Kiểm tra chất lượng tự động**: giá trị vượt dải, nhảy bậc vô lý, **khoảng trống dữ
   liệu**, **trôi điểm không** theo thời gian.
3. **Lưu và xuất được dữ liệu thô** — không chỉ giá trị đã hiệu chỉnh. Đến kỳ kiểm định
   định kỳ mà không còn chuỗi số liệu gốc thì không thể phân tích lại.
4. **Sao lưu và nhật ký hoạt động** (ai sửa gì, khi nào) — vừa để phục hồi, vừa để làm bằng
   chứng.

Một nguyên tắc thiết kế nên đặt ra ngay từ đầu: **dữ liệu phải xuất được ra định dạng mở**
(CSV, JSON) và **không bị khoá trong một phần mềm duy nhất**. Nếu chỉ nhà cung cấp phần mềm
đọc được dữ liệu của chính mình, thì chủ công trình không thực sự sở hữu dữ liệu.

### 12.3.5 Lớp 5 — Phân tích và cảnh báo

- **Ngưỡng** nên đặt theo ba cách khác nhau, không chỉ một: theo **giá trị tuyệt đối**, theo
  **tốc độ thay đổi** (mm/ngày), và **theo cao độ mực nước** (vì cùng một số đọc có ý nghĩa
  rất khác nhau ở mực nước thấp và mực nước cao).
- **Phân tích xu hướng** — hồi quy theo thời gian và theo tải trọng/mực nước để tách biến
  động bình thường khỏi biến đổi bất thường.
- **Đánh giá ổn định lưới mốc chuẩn** theo mỗi chu kỳ. Nếu mốc chuẩn dịch chuyển mà không
  biết, **toàn bộ số liệu sai một cách hệ thống** — và sai một cách rất khó phát hiện.
- **Cảnh báo đa kênh** (SMS, email, còi tại chỗ) kèm **ma trận leo thang**: ai được thông
  báo ở mức nào, và sau bao lâu thì leo lên cấp tiếp theo.

### 12.3.6 Lớp 6 — Hồ sơ và bằng chứng

Lớp cuối là lớp dễ bị coi nhẹ nhất và cũng là lớp quyết định giá trị pháp lý của toàn bộ hệ
thống: báo cáo định kỳ đúng hạn, **nhật ký cảnh báo và biên bản xử lý**, và hồ sơ bàn giao
lưu trữ lâu dài. Một hệ thống đo rất tốt nhưng không xuất được hồ sơ theo mẫu thì vẫn
không đáp ứng được yêu cầu tuân thủ.

!!! tip "Liên hệ với trang ADAQS của cơ sở tri thức này"
    Sáu lớp trên được trình bày chi tiết hơn, kèm đối chiếu với từng nhóm nghĩa vụ tuân
    thủ, tại [Hệ thống thu thập dữ liệu tự động (ADAQS)](../../../adaqs/index.md).

## 12.4 Ứng dụng công nghệ thông tin trong phân tích địa kỹ thuật

### 12.4.1 Một số đặc điểm trong phân tích địa kỹ thuật

Phân tích địa kỹ thuật khác phân tích kết cấu ở ba điểm, và cả ba đều chống lại việc "tự
động hoá hoàn toàn":

- **Thông số không phải là hằng số vật liệu.** Mô đun đàn hồi của đất phụ thuộc **mức biến
  dạng**; sức kháng cắt phụ thuộc **đường ứng suất**. Cùng một loại đất cho nhiều bộ thông
  số khác nhau, tuỳ bài toán.
- **Mô hình là lựa chọn, không phải kết quả.** Chọn mô hình nào (tuyến tính, Mohr–Coulomb,
  mô hình tới hạn, mô hình đất yếu có cố kết) là một quyết định kỹ thuật, không phải một
  bước nhập liệu.
- **Tương tác đất – kết cấu là bài toán hai chiều.** Kết cấu làm thay đổi ứng xử của đất, và
  đất làm thay đổi nội lực trong kết cấu; giải một phía rồi bỏ qua phía kia thường sai.

### 12.4.2 Nhận xét về ứng dụng công nghệ thông tin trong phân tích

Các chương trình phân tích tổng quát dùng trong thực hành — lời giới thiệu của sách nêu ví
dụ **Geo-Slope** và **Plaxis** — chỉ là công cụ; **mô hình, thông số và diễn giải** vẫn là
trách nhiệm của người kỹ sư.

Về mặt công nghệ, các chương trình này chia thành hai họ phương pháp số: **phần tử hữu hạn
(FEM)** và **sai phân hữu hạn (FDM)**, cùng với các phương pháp cân bằng giới hạn cho bài
toán ổn định mái dốc. Mỗi họ có điểm mạnh riêng — FEM/FDM mô phỏng được **trình tự thi
công** và biến dạng, còn cân bằng giới hạn cho **hệ số an toàn** nhanh và ổn định. Biết
chương trình nào trả lời câu hỏi nào là một phần của năng lực kỹ sư, không phải của phần
mềm.

Một cám dỗ công nghệ đáng cảnh báo: **độ chính xác hình thức**. Kết quả xuất ra với bốn chữ
số thập phân gợi cảm giác chính xác mà bản thân thông số đầu vào (vốn chỉ chính xác trong
khoảng ±20–30 %) không hề có.

### 12.4.3 Trao đổi về ý tưởng địa kỹ thuật cho phân tích

Sách kết ở đây: trước khi bấm máy, phải **hình dung được cơ chế phá hoại**. Nếu không nói
được bằng lời khối đất sẽ chuyển vị theo hướng nào, mặt trượt nằm ở đâu, và cái gì tăng
cái gì giảm khi đào hoặc gia tải — thì kết quả phân tích chỉ là con số, không phải kết luận.

## 12.5 Thuật ngữ

| Tiếng Anh | Tiếng Việt (sách dùng) |
| --- | --- |
| geoinformatics | công nghệ thông tin ứng dụng địa kỹ thuật (géo-informatique) |
| site-investigation process | tiến trình khảo sát đất nền |
| database | cơ sở dữ liệu |
| data processing | xử lý số liệu |
| analysis program | chương trình phân tích |
| soil–structure interaction | tương tác đất – kết cấu |
| parameter selection | lựa chọn thông số |
| data acquisition | thu thập dữ liệu |
| data logger | đầu ghi dữ liệu |
| signal conditioning | điều hoà tín hiệu |
| telemetry | truyền dẫn dữ liệu từ xa |
| time series | chuỗi thời gian |
| threshold / alert | ngưỡng / cảnh báo |
| finite element method (FEM) | phương pháp phần tử hữu hạn |
| limit equilibrium | cân bằng giới hạn |

## 12.6 Các điểm then chốt

- Công nghệ thông tin đã thay đổi **cách xử lý số liệu** trong khảo sát và phân tích.
- Đất phức tạp, không đồng nhất và dị hướng; **không một mô hình nào phù hợp cho mọi
  trường hợp**.
- Phần mềm nhanh nhưng cần **kiến thức, kinh nghiệm và phán đoán kỹ thuật**.
- Một hệ quan trắc tự động là **chuỗi sáu lớp**; độ chính xác do **lớp cảm biến** quyết
  định, còn giá trị pháp lý do **lớp hồ sơ** quyết định.
- **Dữ liệu phải xuất được ở định dạng mở** — nếu không, chủ công trình không thực sự sở
  hữu dữ liệu của mình.
- **Đồng bộ thời gian**, **bộ nhớ đệm** và **kiểm tra ổn định mốc chuẩn** là ba chi tiết
  nhỏ hay bị bỏ qua nhưng có thể vô hiệu hoá toàn bộ hệ thống.
- Các chương trình phân tích tổng quát là **công cụ** — mô hình và thông số là trách
  nhiệm của kỹ sư.
- Sách khép lại có chủ đích ở điểm này: **phán đoán là hằng số** xuyên suốt mười hai
  chương.
