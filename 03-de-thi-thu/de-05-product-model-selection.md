# Đề luyện tập 05 — Domain 5: Product & Model Selection (12%)

15 câu · khuyến nghị 30 phút · mỗi câu chọn 1 đáp án.
Đáp án và giải thích nằm trong phần "Xem đáp án" — làm hết rồi mới mở.

> ⚠️ Danh mục sản phẩm, tên model và tính năng của Claude thay đổi nhanh. Đề này tập trung vào **nguyên tắc chọn lựa**; hãy đối chiếu tên gọi cụ thể với trang chính thức của Anthropic.

**Bảng trả lời:** 1.__ 2.__ 3.__ 4.__ 5.__ 6.__ 7.__ 8.__ 9.__ 10.__ 11.__ 12.__ 13.__ 14.__ 15.__

---

### Câu 1
Một công ty cần phân loại 200.000 tin nhắn khách hàng mỗi ngày thành 5 nhóm đơn giản, ưu tiên tốc độ và chi phí thấp. Lựa chọn model phù hợp nhất là gì?

- A. Model nhỏ, nhanh, chi phí thấp (dòng Haiku), sau khi đã kiểm tra chất lượng trên bộ dữ liệu mẫu
- B. Model lớn nhất (dòng Opus) cho mọi tin nhắn
- C. Nhân viên phân loại thủ công
- D. Bật extended thinking ở mức cao nhất cho từng tin nhắn

<details><summary>Xem đáp án</summary>

**A.** Tác vụ đơn giản, khối lượng lớn, cần nhanh và rẻ phù hợp với model nhỏ. Vẫn cần kiểm tra trên dữ liệu mẫu để xác nhận chất lượng đạt yêu cầu. Model lớn nhất (B) tốn kém không cần thiết.
</details>

### Câu 2
Một nhóm chiến lược cần phân tích sâu một bộ tài liệu phức tạp, suy luận nhiều bước, chất lượng là ưu tiên số một, số lượng yêu cầu ít. Lựa chọn hợp lý nhất là gì?

- A. Model nhỏ nhất để tiết kiệm
- B. Không dùng AI
- C. Model mạnh nhất (dòng Opus), có thể kết hợp extended thinking
- D. Chia tài liệu thành 100 phần nhỏ và dùng model nhỏ

<details><summary>Xem đáp án</summary>

**C.** Khi tác vụ phức tạp, quan trọng và số lượng ít, chất lượng xứng đáng với chi phí cao hơn. Đây là đánh đổi chất lượng – tốc độ – chi phí.
</details>

### Câu 3
Ba yếu tố đánh đổi chính khi chọn giữa các model Claude là gì?

- A. Màu sắc, kích thước, ngôn ngữ
- B. Chất lượng/năng lực, tốc độ phản hồi, chi phí
- C. Số người dùng, số tab, số file
- D. Không có đánh đổi; model mới nhất luôn là lựa chọn tốt nhất

<details><summary>Xem đáp án</summary>

**B.** Model lớn thường mạnh hơn nhưng chậm hơn và đắt hơn; model nhỏ nhanh và rẻ hơn. Chọn model là chọn điểm cân bằng phù hợp với tác vụ, không phải luôn chọn model lớn nhất (D sai).
</details>

### Câu 4
Một lập trình viên muốn Claude đọc toàn bộ codebase, sửa lỗi, chạy test ngay trong terminal của mình. Sản phẩm phù hợp nhất là gì?

- A. Claude.ai bản web, copy-paste từng file
- B. Claude for Excel
- C. Ứng dụng Claude trên điện thoại
- D. Claude Code

<details><summary>Xem đáp án</summary>

**D.** Claude Code được thiết kế cho công việc lập trình: đọc và sửa code, chạy lệnh trong môi trường phát triển. Copy-paste từng file (A) không hiệu quả với codebase lớn.
</details>

### Câu 5
Một công ty muốn tích hợp Claude vào ứng dụng của mình để tự động xử lý đơn hàng. Họ nên dùng gì?

- A. Mỗi nhân viên mở Claude.ai và dán đơn hàng vào
- B. Claude API (Claude Developer Platform), tích hợp trực tiếp vào hệ thống
- C. Ứng dụng Claude trên máy tính
- D. Chụp màn hình đơn hàng gửi qua email

<details><summary>Xem đáp án</summary>

**B.** Tích hợp vào ứng dụng hoặc quy trình tự động là việc của API. Claude.ai (A) phù hợp với người dùng tương tác trực tiếp, không phải tích hợp hệ thống.
</details>

### Câu 6
Một nhóm 30 người cần dùng chung Claude với quản lý tập trung (thanh toán, phân quyền, chia sẻ Project). Gói nào phù hợp hơn?

- A. Gói dành cho tổ chức (Team/Enterprise)
- B. Mỗi người tự đăng ký gói cá nhân Free
- C. Dùng chung một tài khoản cá nhân cho cả 30 người
- D. Chỉ dùng API qua terminal

<details><summary>Xem đáp án</summary>

**A.** Gói tổ chức có quản trị tập trung, chia sẻ và các kiểm soát dành cho doanh nghiệp. Dùng chung tài khoản (C) vi phạm điều khoản và mất khả năng kiểm soát.
</details>

### Câu 7
Người dùng cần Claude trả lời về sự kiện xảy ra tuần trước. Tính năng nào cần thiết?

- A. Tăng độ dài câu trả lời
- B. Đổi sang model lớn hơn
- C. Viết prompt bằng tiếng Anh
- D. Bật tính năng tìm kiếm web (web search), vì kiến thức của model chỉ đến ngày giới hạn huấn luyện

<details><summary>Xem đáp án</summary>

**D.** Model có thời điểm giới hạn kiến thức (knowledge cutoff). Thông tin mới cần lấy từ web search hoặc tài liệu được cung cấp. Model lớn hơn (B) không tự biết sự kiện mới.
</details>

### Câu 8
"Extended thinking" phù hợp nhất với loại tác vụ nào?

- A. Chào hỏi khách hàng
- B. Dịch một câu ngắn
- C. Bài toán phức tạp cần suy luận nhiều bước: phân tích, lập kế hoạch, toán, lập trình khó
- D. Trả lời "có" hoặc "không" cho câu hỏi đơn giản

<details><summary>Xem đáp án</summary>

**C.** Extended thinking cho Claude thêm "thời gian suy nghĩ" trước khi trả lời, hữu ích với tác vụ phức tạp. Với tác vụ đơn giản, nó chỉ làm tăng thời gian và chi phí.
</details>

### Câu 9
Nhân viên tài chính muốn Claude phân tích và chỉnh sửa trực tiếp trong bảng tính đang làm việc. Lựa chọn phù hợp nhất là gì?

- A. Dùng tích hợp Claude dành cho bảng tính (ví dụ Claude for Excel) nếu tổ chức đã được cấp
- B. Chép tay số liệu vào chat
- C. Dùng Claude Code để sửa file Excel thủ công
- D. Không thể dùng Claude với bảng tính

<details><summary>Xem đáp án</summary>

**A.** Dùng công cụ tích hợp ngay trong môi trường làm việc giúp giảm thao tác và sai sót. Chép tay số liệu (B) dễ sai.
</details>

### Câu 10
Một người dùng tải lên hợp đồng 400 trang nhưng Claude báo vượt giới hạn. Khái niệm liên quan là gì?

- A. Tốc độ mạng
- B. Context window (giới hạn ngữ cảnh mà model xử lý được trong một lần)
- C. Số lượng tab trình duyệt
- D. Phiên bản hệ điều hành

<details><summary>Xem đáp án</summary>

**B.** Mỗi model có giới hạn context window. Với tài liệu quá dài, cần chia nhỏ, tóm tắt theo phần, hoặc dùng Project/tri thức để truy xuất phần liên quan. Câu này kết hợp với Domain 6.
</details>

### Câu 11
Một startup đang phát triển chatbot. Ban đầu họ dùng model mạnh nhất cho mọi câu hỏi và chi phí rất cao. Giải pháp tối ưu là gì?

- A. Tắt chatbot
- B. Giới hạn mỗi khách chỉ hỏi 1 câu
- C. Chuyển toàn bộ sang model nhỏ nhất mà không kiểm tra
- D. Phân luồng: câu hỏi đơn giản dùng model nhỏ, câu hỏi phức tạp mới chuyển sang model lớn; đo chất lượng ở từng nhóm

<details><summary>Xem đáp án</summary>

**D.** Định tuyến theo độ phức tạp (routing) giúp cân bằng chi phí và chất lượng. Chuyển toàn bộ sang model nhỏ mà không kiểm tra (C) có thể làm giảm chất lượng ở các câu khó.
</details>

### Câu 12
Bạn cần tạo một trang web tương tác nhỏ (biểu đồ, công cụ tính) ngay trong cuộc trò chuyện để chia sẻ với đồng nghiệp. Tính năng nào phù hợp?

- A. Web search
- B. Extended thinking
- C. Artifacts
- D. Memory

<details><summary>Xem đáp án</summary>

**C.** Artifacts cho phép Claude tạo nội dung độc lập như trang web, biểu đồ, tài liệu để xem và chia sẻ. Các tính năng còn lại phục vụ mục đích khác.
</details>

### Câu 13
Tiêu chí **quan trọng nhất** khi quyết định chọn model cho một use case mới là gì?

- A. Kết quả thử nghiệm thực tế trên dữ liệu đại diện của use case, đối chiếu với yêu cầu về chất lượng, tốc độ và ngân sách
- B. Model nào được nói đến nhiều nhất trên mạng xã hội
- C. Model nào có tên dễ nhớ nhất
- D. Model nào ra mắt gần nhất

<details><summary>Xem đáp án</summary>

**A.** Quyết định nên dựa trên đánh giá thực tế với dữ liệu của chính use case đó. Độ phổ biến (B) hay ngày ra mắt (D) không đảm bảo phù hợp.
</details>

### Câu 14
Người dùng muốn Claude truy cập dữ liệu từ các công cụ khác như Google Drive, Slack, Jira để trả lời câu hỏi. Họ cần gì?

- A. Copy tất cả dữ liệu vào một tin nhắn
- B. Đổi sang model lớn nhất
- C. Bật extended thinking
- D. Dùng connectors (dựa trên Model Context Protocol – MCP) đã được tổ chức phê duyệt

<details><summary>Xem đáp án</summary>

**D.** Connectors (dựa trên MCP) cho phép Claude truy cập dữ liệu và công cụ bên ngoài một cách có kiểm soát. Cần tuân thủ phê duyệt của tổ chức (liên quan Domain 3).
</details>

### Câu 15
Một nhân viên văn phòng (không biết lập trình) muốn dùng Claude để soạn thảo, tóm tắt tài liệu và brainstorm hằng ngày. Lựa chọn phù hợp nhất là gì?

- A. Claude API, tự viết code gọi API
- B. Claude.ai (web, desktop hoặc mobile) qua tài khoản do công ty cấp
- C. Claude Code trong terminal
- D. Tự huấn luyện một model riêng

<details><summary>Xem đáp án</summary>

**B.** Giao diện trò chuyện (Claude.ai và các app) phù hợp nhất cho người dùng không chuyên kỹ thuật với tác vụ hằng ngày. API (A) và Claude Code (C) dành cho nhà phát triển.
</details>

---

## Chấm điểm
- 13–15: Vững
- 10–12: Ôn lại các câu sai, đọc lại [ghi chú Domain 5](../01-domains/05-product-model-selection.md)
- < 10: Làm BT4 trong [danh sách bài tập](../02-bai-tap/danh-sach-bai-tap.md), rồi làm lại đề sau 2 ngày

Ghi các câu sai vào [ket-qua.md](ket-qua.md).
