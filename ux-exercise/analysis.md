# UX exercise — Vietnam Airlines Chatbot NEO

## Sản phẩm: Vietnam Airlines — Chatbot NEO (hỗ trợ khách hàng)

## 4 paths

### 1. AI đúng
- User hỏi đúng keyword (VD: quy định hành lý) → Bot trả lời đầy đủ thông tin trọng lượng vs kích thước + link tham khảo
- Trải nghiệm tự động xử lý tốt, đầy đủ thông tin

### 2. AI không chắc
- User gõ "chec in nhu nao?" (sai typo / ko dấu) → Bot không đoán được intent
- Bot báo "chưa có thông tin" và đẩy trách nhiệm cho user alo cho tổng đài
- Vấn đề: Xử lý kém, không có cơ chế hỏi lại user để làm rõ ý

### 3. AI sai
- User nhập sai mã đặt chỗ → Bot chỉ báo không hợp lệ mà không có correction path
- Khi gặp 2 intent ("đi SG" và "xách nhiều đồ") → Bot bị phân vân và bỏ qua ý mua vé, chỉ tư vấn mua thêm ghế chở 75kg đồ
- Sửa bằng cách nào: Không rõ ràng, user phải tự gõ lại luồng từ đầu

### 4. User mất niềm tin
- User trong trạng thái khẩn cấp ("Chuyến bay của hãng delay làm tôi bị lỡ chuyến chuyển tiếp, đền bù gấp!") → Bot không nhận diện được sự tức giận
- Thay vì đưa exit path như CTA để gọi nhân viên thật → Bot ném đoạn văn pháp lý dài khiến user càng tức hơn
- Đây là path tệ nhất, không có fallback thân thiện

## Path yếu nhất: Path 4
- Xử lý máy móc, thuần FAQ, mù EQ và không có CTA khẩn cấp
- Không có lối thoát (exit path) khi user đang trong tình trạng bức xúc

## Gap marketing vs thực tế
- Marketing: "Tra cứu nhanh chóng, hỗ trợ tìm giá vé tốt nhất, cung cấp thông tin quan trọng" - hứa hẹn AI liền mạch.
- Thực tế: Trải nghiệm cực tệ khi NLP không hiểu từ khoá, gây trả lời sai, vòng lặp, fallback về yêu cầu cung cấp thông tin đặt chỗ và mã chuyến bay.
- Gap lớn nhất: Thực tế không khác gì auto-bot rule-based. Không có UX xử lý graceful failure và gãy luồng chat hoàn toàn ở nhịp khó.

## Sketch
(Ảnh đính kèm: sketch.jpg hoặc sketch.pdf)
- As-is: user nhập tình huống khẩn cấp / tức giận → bot trả lời template pháp lý / không hiểu context → user mắc kẹt
- To-be: user nhập tình huống khẩn cấp / tức giận → bot nhận diện sentiment báo "Xin lỗi quý khách về trải nghiệm này..." → hiện ngay CTA kết nối Agent thực / Hotline / Email kèm việc transfer toàn bộ lịch sử chat
