# Bài tập UX: phân tích sản phẩm AI thật

**Thời gian:** 40 phút | **Cá nhân** | **Output:** sketch giấy, nộp cuối bài

---

## Chọn 1 sản phẩm

| Sản phẩm | AI feature | Truy cập |
|----------|-----------|---------|
| MoMo — Trợ thủ AI Moni | Phân loại chi tiêu, chatbot tài chính | App MoMo |
| Vietnam Airlines — Chatbot NEO | Chatbot hỗ trợ khách hàng, tra cứu chuyến bay | vietnamairlines.com hoặc Zalo VNA |
| V-App — Trợ lý ảo V-AI | Trợ lý voice/text, gợi ý theo context | App V-App |

---

## Phần 1 — Khám phá (15 phút)

**Trước khi dùng:** tìm hiểu sản phẩm marketing AI feature này thế nào — website, app store, bài PR. Sản phẩm hứa gì?

**Rồi dùng thử:** tải app / mở web, thử các tính năng AI. Quan sát kỹ: AI phản ứng thế nào? UI thay đổi gì? Có nút gì xuất hiện / biến mất?

### Kết quả khám phá

**Marketing hứa hẹn:**
- Tra cứu nhanh chóng
- Hỗ trợ tìm giá vé tốt nhất
- Cung cấp thông tin quan trọng

**Trải nghiệm thực tế:**
- Trải nghiệm cực tệ khi NLP không hiểu từ khoá, gây trả lời sai, vòng lặp, fallback về yêu cầu cung cấp thông tin đặt chỗ và mã chuyến bay. Gần như thuần FAQ chatbot rule-based.

## Phần 2 — Phân tích 4 paths (10 phút)

Dùng framework 4 paths để mổ xẻ sản phẩm:

| Path | Câu hỏi | Đánh giá hiện trạng |
| :--- | :--- | :--- |
| **Khi AI đúng** | User thấy gì? | Khi hỏi đúng keyword (VD: quy định hành lý), bot trả lời đầy đủ thông tin trọng lượng vs kích thước + link tham khảo |
| **Khi AI không chắc** | Hệ thống xử lý thế nào? | Xử lý kém. User gõ "chec in nhu nao?" (sai typo / ko dấu), bot ko đoán được intent mà báo "chưa có thông tin" và đẩy trách nhiệm cho user alo cho tổng đài, ko hỏi lại user. |
| **Khi AI sai** | Sửa bằng cách nào? | Khi user nhập sai mã đặt chỗ, bot chỉ báo ko hợp lệ mà ko có correction path; khi gặp 2 intent ("đi SG" và "xách nhiều đồ"), bot bị phân vân và bỏ qua ý mua vé và chỉ tư vấn mua thêm ghế chở 75kg đồ. |
| **Khi user mất tin** | Có exit ko? | Đây là path tệ nhất, khi user đang trong state khẩn cấp ("Chuyến bay của hãng delay làm tôi bị lỡ chuyến chuyển tiếp, đền bù gấp!"), bot ko nhận diện đc sự tức giận. Thay vì đưa exit path như CTA để gọi nhân viên thật thì nó lại ném đoạn văn pháp lý dài khiến user tức lên. |

**Tự phân tích:**
- **Path xử lý tốt nhất:** Path 1 (Khi đúng luồng kịch bản định sẵn) - Đầy đủ thông tin và link.
- **Path xử lý yếu nhất:** Path 4 - Xử lý máy móc, thuần FAQ, mù EQ và ko có CTA khẩn cấp.
- **Gap giữa marketing và thực tế:** Lớn - Hứa hẹn AI liền mạch nhưng trải nghiệm thực tế ko khác gì auto-bot rule-based. Ko có UX xử lý graceful failure và exit path khi đứt gãy luồng chat.

## Phần 3 — Sketch "làm tốt hơn" (10 phút)

Chọn **1 path yếu nhất** mà mình tìm được. Sketch trên giấy:

- **As-is** (bên trái): user journey hiện tại → đánh dấu chỗ gãy
- **To-be** (bên phải): user journey đề xuất → vẽ kế bên
- Ghi rõ: thêm gì? Bớt gì? Đổi gì?

Không cần đẹp. Cần rõ.

## Phần 4 — Share + vote (5 phút)

Chia sẻ sketch với nhóm. Mỗi người trình bày ngắn (30 giây). Nhóm vote sketch hay nhất → **bonus điểm**.

---

## Nộp bài

Mỗi người nộp sketch giấy + ghi chú phân tích 4 paths. Đây là **điểm cá nhân**.

**Nice to have:** screenshot màn hình app + annotate (khoanh, ghi chú) chỗ hay / chỗ gãy. Nộp kèm sketch.

---

## Tiêu chí chấm (10 điểm + bonus)

| Tiêu chí | Điểm |
|----------|------|
| Phân tích 4 paths đủ + nhận xét path yếu nhất | 4 |
| Sketch as-is + to-be rõ ràng | 4 |
| Nhận xét gap marketing vs thực tế | 2 |
| **Bonus:** nhóm vote sketch hay nhất | +bonus |

---

*Bài tập UX — Ngày 5 — VinUni A20 — AI Thực Chiến · 2026*
