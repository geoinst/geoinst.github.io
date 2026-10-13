---
lang: vi
---
# Chương 19 — Áp lực đất

Chương này gom các bảng về **áp lực đất**: phân bố, hệ số áp lực tại chỗ K₀ và biến
thiên theo OCR, chuyển động liên quan, áp lực chủ động/bị động, và ma sát tường.

## 19.1 Áp lực đất

Bảng của mục này giới thiệu **ba trạng thái** áp lực đất — **tại chỗ (at-rest)**, **chủ
động (active)**, **bị động (passive)** — và quan hệ với **chuyển động của tường**.

## 19.2 Phân bố áp lực đất

Bảng của mục này so **phân bố dạng tam giác** (lý thuyết) với **phân bố thực tế** (có
thể tập trung ở đỉnh hoặc đáy tường) — quan trọng cho thiết kế tường cao.

## 19.3 Hệ số áp lực đất tại chỗ

**Bảng 19.3 — Hệ số áp lực tại chỗ K₀.**

| Loại đất | K₀ điển hình |
|---|---|
| Cát, cố kết thường | 0,4 – 0,5 |
| Sét, cố kết thường | 0,5 – 0,7 |
| Sét, cố kết trước | 0,8 – 2,0 |
| Đất đắp đầm chặt | 0,5 – 1,0 |

Công thức **Jaky**: **K₀ = 1 − sin φ′** cho đất cố kết thường.

## 19.4 Biến thiên áp lực tại chỗ theo OCR

**K₀(OCR) = K₀(NC) · OCR^sin φ′** — đất cố kết trước có **K₀ cao hơn nhiều**; sét cố
kết trước mạnh có thể có **K₀ > 1** (áp lực ngang lớn hơn áp lực đứng).

## 19.5 Biến thiên áp lực tại chỗ theo OCR dùng hệ số đàn hồi

Bảng của mục này dùng **cách tiếp cận đàn hồi** để suy K₀ cho đất cố kết trước — một
phương pháp kiểm tra chéo với công thức Jaky.

## 19.6 Chuyển động liên quan đến áp lực đất

**Bảng 19.6 — Chuyển động cần để đạt trạng thái.**

| Trạng thái | Chuyển động tường (Δ/H) |
|---|---|
| Tại chỗ → chủ động | 0,001 – 0,005 |
| Chủ động → bị động | 0,02 – 0,10 |
| Cát chặt | Ít hơn |
| Sét mềm | Nhiều hơn |

Tường cần **dịch chuyển** mới đạt áp lực chủ động — nếu tường được giữ cứng, áp lực
là **tại chỗ**, cao hơn đáng kể.

## 19.7 Áp lực đất chủ động và bị động

**Ka = tan²(45° − φ/2)** và **Kp = tan²(45° + φ/2)** — với **φ** cho đất hạt rời, hoặc
**phân tích ứng suất hữu hiệu** cho đất dính.

## 19.8 Phân bố áp lực đất

Bảng của mục này đưa **hình dạng phân bố** cho từng trạng thái và từng loại tường
(tường cứng, tường mềm, tường neo).

## 19.9 Áp dụng điều kiện tại chỗ và chủ động

Bảng của mục này hướng dẫn **khi nào dùng tại chỗ vs. chủ động**: tường cứng dùng tại
chỗ; tường cho phép xoay dùng chủ động.

## 19.10 Áp dụng áp lực bị động

Bảng của mục này hướng dẫn dùng **áp lực bị động** (rất lớn) — chỉ huy động được khi
tường dịch chuyển đủ, thường dùng cho **phần ngàm sâu** của tường.

## 19.11 Sử dụng ma sát tường

Bảng của mục này đưa **hệ số ma sát tường δ** theo **loại vật liệu tường và đất** —
ma sát tường làm giảm áp lực chủ động và tăng áp lực bị động.

## 19.12 Giá trị áp lực đất chủ động

**Bảng 19.12 — Áp lực chủ động điển hình.**

| Loại đất | φ′ | Ka | Áp lực (kN/m²/m) |
|---|---|---|---|
| Cát rời | 30° | 0,33 | 0,33 γH |
| Cát chặt | 38° | 0,24 | 0,24 γH |
| Sét mềm | — | 1,0 | γH − 2Cu |
| Sét cứng | — | 0,5 | 0,5 γH |

## 19.13 Giá trị áp lực đất bị động

Bảng của mục này đưa **áp lực bị động điển hình** — lớn hơn nhiều lần áp lực chủ
động (Kp/Kₐ ≈ 3–10 lần).

## Ghi nhớ của chương

- **Trạng thái áp lực đất phụ thuộc chuyển động tường** (mục 19.6) — tường cứng nhận
  áp lực **tại chỗ**, không phải chủ động.
- **K₀ = 1 − sin φ′** (mục 19.3); đất **cố kết trước** có K₀ cao hơn nhiều và có thể
  **> 1** (mục 19.4).
- **Ka và Kp** (mục 19.7) chênh nhau lớn — huy động bị động cần dịch chuyển lớn.
- **Ma sát tường** (mục 19.11) làm giảm áp lực chủ động — có thể giảm **10–30%**.
