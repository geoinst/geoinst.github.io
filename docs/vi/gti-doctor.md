---
lang: vi
lang_alt: gti-doctor/
---

# GTI Doctor — Trợ lý AI (Bác sĩ GTI)

> 🤖 **Trợ lý AI GTI Doctor (Bác sĩ GTI) hiện đã HOẠT ĐỘNG.** Hãy đặt câu hỏi về thiết bị quan trắc địa kỹ thuật — thông số cảm biến, quy trình lắp đặt, danh mục kiểm tra ứng dụng — và nó sẽ trả lời dựa trên các trích dẫn có căn cứ từ 18 sổ tay tham khảo trong cơ sở tri thức này (5.032 phân đoạn được lập chỉ mục, 12,5 MB văn bản).

**Truy cập**: <https://gti-doctor.henry-phamduc.workers.dev/>

<style>
.chat-iframe-wrapper { width: 100%; min-height: 640px; border: 1px solid var(--md-default-fg-color--lightest); border-radius: 8px; overflow: hidden; background: #fafafa; }
.chat-iframe-wrapper iframe { width: 100%; height: 640px; border: 0; }
.gti-actions { display: flex; gap: 12px; flex-wrap: wrap; margin-bottom: 18px; }
.gti-actions a { display: inline-block; padding: 10px 18px; background: var(--md-primary-fg-color); color: var(--md-primary-bg-color); text-decoration: none; border-radius: 6px; font-weight: 500; }
.gti-actions a:hover { filter: brightness(1.1); }
</style>

<div class="gti-actions">
  <a href="https://gti-doctor.henry-phamduc.workers.dev/" target="_blank">Open full chat ↗</a>
  <a href="#try-inline-chat">Try chat inline ↓</a>
</div>

<a id="try-inline-chat"></a>
<div class="chat-iframe-wrapper">
  <iframe src="https://gti-doctor.henry-phamduc.workers.dev/" title="GTI Doctor chat" loading="lazy"></iframe>
</div>

## Các câu hỏi ví dụ

- *Piezometer (áp kế) dây rung là gì và lắp đặt trong hố khoan như thế nào?*
- *Cho tôi danh mục thiết bị quan trắc ổn định mái dốc từ sổ tay FHWA.*
- *Mạng lưới (mesh) không dây truyền dữ liệu ngược hoạt động thế nào?*
- *Thiết bị nào tôi nên dùng để quan trắc chuyển động ngang trong tường chắn hố đào sâu 30 m?*

## Cách thức hoạt động

| Thành phần | Công nghệ |
| --- | --- |
| LLM | `@cf/meta/llama-3.1-8b-instruct-fp8` (Workers AI, miễn phí) |
| Embeddings | `@cf/baai/bge-m3` (đa ngôn ngữ 1024 chiều) |
| Cơ sở dữ liệu vector | Cloudflare Vectorize (chỉ mục `gti-doctor-embeddings`, 5.032 vector) |
| Môi trường Worker | Cloudflare Workers (kèm liên kết Workers AI + Vectorize) |
| Căn cứ (Grounding) | Quy trình RAG — nhúng truy vấn → 8 phân đoạn hàng đầu → prompt giàu ngữ cảnh |

Trợ lý chỉ được huấn luyện **duy nhất** trên cơ sở tri thức này. Nếu câu hỏi nằm ngoài phạm vi, nó sẽ nói rõ thay vì bịa ra câu trả lời.

## API

| Điểm cuối | Phương thức | Mục đích |
| --- | --- | --- |
| `/api/health` | GET | Tín hiệu hoạt động dịch vụ |
| `/api/info` | GET | Cấu hình Worker |
| `/api/chat` | POST | Chat RAG (truyền phát qua SSE hoặc JSON hàng loạt) |
| `/api/search` | POST | Tìm kiếm ngữ nghĩa thuần túy (không dùng LLM, chỉ lấy K phân đoạn hàng đầu) |

Ví dụ:

```bash
curl -X POST https://gti-doctor.henry-phamduc.workers.dev/api/chat \
  -H "Content-Type: application/json" \
  -d '{"question":"What is a vibrating-wire piezometer?","stream":false}'
```

## Trạng thái

| Thành phần | Trạng thái |
| --- | --- |
| Nạp kho dữ liệu (18 PDF, 5.032 phân đoạn) | ✅ Hoàn tất |
| Đã tạo chỉ mục Vectorize | ✅ `gti-doctor-embeddings` (1024 chiều, cosine) |
| Đã triển khai Cloudflare Worker | ✅ <https://gti-doctor.henry-phamduc.workers.dev/> |
| Điểm cuối chat | ✅ Đã xác minh — 200 OK, câu trả lời có căn cứ kèm trích dẫn |
| Widget chat nhúng trong mạng nội bộ | ✅ Khung iframe trực tiếp ở trên |
