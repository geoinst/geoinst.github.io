---
lang: vi
lang_alt: reference-manuals/tailings-dam-safety/chapter-11-data-management/
---
# Chương 11 — Thu thập, Quản lý dữ liệu và Cơ sở dữ liệu

## 11.1 Từ số đọc đến hồ sơ

Đầu ra cảm biến thô không phải là thông tin. Chuỗi dữ liệu — thu thập, kiểm định,
lưu trữ và truy xuất — xác định liệu các phép đo có trở thành bằng chứng có thể bảo
vệ về hiệu năng hay không.

## 11.2 Tần suất đọc

Tần suất được đặt bởi:

- **Động lực tham số** (áp lực nước lỗ rỗng và chuyển động trong bão thay đổi
  nhanh; lún chậm).
- **Giai đoạn đời** (đưa vào vận hành và đổ thải đỉnh cần nhiều hơn; vận hành ổn
  định ít hơn).
- **Hạng mục rủi ro** (hậu quả cao hơn → thường xuyên hơn, thường tự động).

Một tần suất tối thiểu được ghi trong kế hoạch; tăng theo sự kiện sau bão, động
đất hoặc bất thường.

## 11.3 Kiểm định và kiểm soát chất lượng

Trước khi dữ liệu vào hồ sơ, nó nên được kiểm tra:

- **Tính hợp lý** (trong dải, không nhảy vọt).
- **Tính liên tục** (khoảng hổng được giải thích, không giấu).
- **Trôi dạt hiệu chuẩn** (so với kiểm tra thủ công và hiệu chuẩn nhà máy).
- **Tương quan môi trường** (ví dụ, loại bỏ hiệu ứng nhiệt độ).

!!! warning "Khoảng hổng cũng là dữ liệu"
    Một số đọc bị thiếu là một phát hiện. Điều tra và ghi chép khoảng hổng thay vì
    nội suy thầm lặng. Một chu kỳ khoảng hổng ở thiết bị trọng yếu bản thân nó là
    một báo động.

## 11.4 Cơ sở dữ liệu và truy xuất

Một cơ sở dữ liệu có cấu trúc (không phải các bảng tính rải rác) hỗ trợ:

- Đồ thị chuỗi thời gian cho mỗi thiết bị và tham số.
- Biểu đồ chéo (ví dụ, chuyển động so với áp lực nước lỗ rỗng).
- Vết kiểm toán và kiểm soát truy cập.
- Tính liên tục dài hạn khi nhân sự và thiết bị thay đổi.

## 11.5 Bảo tồn và bàn giao

Hồ sơ giám sát phải tồn tại lâu hơn bất kỳ cá nhân hay hợp đồng nào. Lưu trữ dữ
liệu thô và đã xử lý, hồ sơ lắp đặt và ghi chú rà soát ở dạng tồn tại qua **đóng
cửa và chuyển giao quyền sở hữu**. Hồ sơ là trí nhớ của cơ sở.

## 11.6 Điểm mấu chốt

- Chất lượng chuỗi dữ liệu xác định liệu số đọc có trở thành bằng chứng.
- Đặt tần suất theo tham số, giai đoạn đời và rủi ro.
- Kiểm định tính hợp lý, tính liên tục và hiệu chuẩn; ghi chép khoảng hổng.
- Lưu trữ dài hạn, qua đóng cửa và thay đổi quyền sở hữu.
