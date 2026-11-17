# Đề luyện tập 06 — Domain 6: Configuration & Knowledge Management (12%)

15 câu · khuyến nghị 30 phút · mỗi câu chọn 1 đáp án.
Đáp án và giải thích nằm trong phần "Xem đáp án" — làm hết rồi mới mở.

> ⚠️ Tên và cách hoạt động của tính năng (Projects, Skills, Memory, Connectors…) có thể thay đổi. Đối chiếu với tài liệu chính thức của Anthropic.

**Bảng trả lời:** 1.__ 2.__ 3.__ 4.__ 5.__ 6.__ 7.__ 8.__ 9.__ 10.__ 11.__ 12.__ 13.__ 14.__ 15.__

---

### Câu 1
Nhóm marketing liên tục phải dán lại hướng dẫn thương hiệu và mô tả sản phẩm vào mỗi cuộc trò chuyện mới. Giải pháp phù hợp nhất là gì?

- A. Dán lại mỗi lần cho chắc
- B. Ghi nhớ trong đầu và gõ lại
- C. Gửi qua email cho Claude
- D. Tạo một Project, tải tài liệu thương hiệu vào Project Knowledge và viết hướng dẫn cho Project

<details><summary>Xem đáp án</summary>

**D.** Project cho phép lưu tài liệu và hướng dẫn dùng chung cho mọi cuộc trò chuyện trong Project, giúp nhất quán và tiết kiệm thời gian.
</details>

### Câu 2
Khác biệt giữa **Project instructions** và **Project Knowledge** là gì?

- A. Instructions là chỉ dẫn về cách Claude làm việc (vai trò, giọng văn, quy tắc); Knowledge là tài liệu tham khảo Claude dùng để trả lời
- B. Hai thứ giống hệt nhau
- C. Instructions chỉ dùng cho code, Knowledge chỉ dùng cho văn bản
- D. Knowledge là lịch sử chat

<details><summary>Xem đáp án</summary>

**A.** Instructions định hướng *cách* Claude hành xử; Knowledge cung cấp *nội dung* để Claude tham chiếu.
</details>

### Câu 3
Claude trong Project thỉnh thoảng trả lời theo chính sách cũ dù đã có tài liệu chính sách mới. Nguyên nhân khả dĩ nhất là gì?

- A. Claude cố tình trả lời sai
- B. Project bị lỗi vĩnh viễn
- C. Cả tài liệu cũ và mới cùng nằm trong Project Knowledge, gây mâu thuẫn; cần xóa hoặc đánh dấu rõ tài liệu đã hết hiệu lực
- D. Cần đổi sang model khác

<details><summary>Xem đáp án</summary>

**C.** Quản lý tri thức cần đảm bảo nguồn là bản mới nhất và không mâu thuẫn. Tài liệu lỗi thời là nguyên nhân phổ biến của câu trả lời sai.
</details>

### Câu 4
Bạn thường xuyên yêu cầu Claude tạo báo cáo theo đúng một quy trình nhiều bước và một định dạng chuẩn của công ty. Tính năng nào giúp đóng gói quy trình này để tái sử dụng?

- A. Web search
- B. Skills (đóng gói hướng dẫn, template, script cho một loại tác vụ)
- C. Tăng context window
- D. Xóa lịch sử chat

<details><summary>Xem đáp án</summary>

**B.** Skills đóng gói hướng dẫn và tài nguyên cho một loại tác vụ lặp lại; Claude dùng Skill khi tác vụ phù hợp.
</details>

### Câu 5
Một người dùng muốn Claude luôn trả lời ngắn gọn, bằng tiếng Việt, ở mọi cuộc trò chuyện, không riêng một Project nào. Nên cấu hình ở đâu?

- A. Mỗi Project một lần
- B. Trong mỗi tin nhắn
- C. Trong phần tùy chọn cá nhân (profile preferences / custom instructions cấp tài khoản) hoặc style
- D. Không thể cấu hình

<details><summary>Xem đáp án</summary>

**C.** Tùy chọn cấp tài khoản áp dụng cho mọi cuộc trò chuyện; Project instructions chỉ áp dụng trong Project đó.
</details>

### Câu 6
Cuộc trò chuyện đã rất dài, Claude bắt đầu "quên" các chi tiết được nhắc ở đầu. Cách xử lý hợp lý nhất là gì?

- A. Tiếp tục hỏi trong cùng cuộc trò chuyện
- B. Đổi sang trình duyệt khác
- C. Viết hoa các yêu cầu
- D. Tóm tắt các điểm chính và quyết định quan trọng, rồi mở cuộc trò chuyện mới với bản tóm tắt đó (hoặc đưa thông tin bền vững vào Project)

<details><summary>Xem đáp án</summary>

**D.** Khi ngữ cảnh quá dài, chất lượng có thể giảm. Bắt đầu lại với một bản tóm tắt gọn hoặc lưu thông tin quan trọng vào Project giúp giữ ngữ cảnh cần thiết.
</details>

### Câu 7
Tài liệu nào **không nên** đưa vào Project Knowledge dùng chung cho cả phòng ban?

- A. Hướng dẫn giọng văn thương hiệu
- B. Bảng lương chi tiết của từng nhân viên
- C. FAQ sản phẩm
- D. Template báo cáo

<details><summary>Xem đáp án</summary>

**B.** Dữ liệu nhạy cảm không nên đặt ở nơi nhiều người truy cập được nếu họ không có quyền xem. Câu này kết hợp với Domain 3.
</details>

### Câu 8
Cách tổ chức tài liệu nào giúp Claude truy xuất thông tin trong Project Knowledge **chính xác hơn**?

- A. Tài liệu có cấu trúc rõ ràng (tiêu đề, mục), tên file mô tả nội dung, mỗi tài liệu một chủ đề, không trùng lặp
- B. Gộp tất cả vào một file khổng lồ không có tiêu đề
- C. Đặt tên file là "doc1", "doc2", "final_final_v3"
- D. Tải lên nhiều bản trùng nhau cho chắc

<details><summary>Xem đáp án</summary>

**A.** Tài liệu rõ ràng, có cấu trúc và không trùng lặp giúp cả Claude và con người tìm đúng thông tin.
</details>

### Câu 9
Tính năng Memory của Claude có tác dụng gì và cần lưu ý gì?

- A. Lưu toàn bộ file trên máy tính
- B. Thay thế hoàn toàn Project Knowledge
- C. Giúp Claude chạy nhanh hơn
- D. Giúp Claude ghi nhớ ngữ cảnh và sở thích qua các cuộc trò chuyện; người dùng nên xem lại, chỉnh sửa và biết cách tắt khi cần, đặc biệt với thông tin nhạy cảm

<details><summary>Xem đáp án</summary>

**D.** Memory giúp cá nhân hóa trải nghiệm, nhưng người dùng cần kiểm soát những gì được ghi nhớ. Memory không thay thế nguồn tài liệu chính thức (B sai).
</details>

### Câu 10
Bạn bật connector Google Drive cho Claude nhưng Claude không tìm thấy một tài liệu cụ thể. Nguyên nhân khả dĩ nhất là gì?

- A. Claude không biết tiếng Việt
- B. Model quá nhỏ
- C. Tài khoản được kết nối không có quyền truy cập tài liệu đó, hoặc tài liệu nằm ngoài phạm vi được chia sẻ
- D. Cần bật extended thinking

<details><summary>Xem đáp án</summary>

**C.** Connector hoạt động theo quyền của tài khoản được kết nối. Kiểm tra quyền truy cập là bước xử lý đầu tiên.
</details>

### Câu 11
Một nhóm cần quy trình để giữ cho Project Knowledge luôn đúng. Thực hành tốt nhất là gì?

- A. Chỉ định người phụ trách nội dung, lịch rà soát định kỳ, ghi rõ ngày cập nhật và loại bỏ tài liệu hết hiệu lực
- B. Ai muốn thêm gì thì thêm
- C. Không bao giờ cập nhật để tránh lỗi
- D. Mỗi tuần xóa hết rồi tải lại toàn bộ

<details><summary>Xem đáp án</summary>

**A.** Quản lý tri thức cần có người chịu trách nhiệm và quy trình bảo trì. Không cập nhật (C) dẫn đến thông tin lỗi thời.
</details>

### Câu 12
Hướng dẫn trong Project nên được viết như thế nào?

- A. Càng mơ hồ càng linh hoạt
- B. Rõ ràng, cụ thể: vai trò, đối tượng phục vụ, giọng văn, định dạng đầu ra, việc nên làm và cần tránh, khi nào cần nói "không biết"
- C. Chỉ một từ: "Giúp đỡ"
- D. Copy toàn bộ tài liệu Knowledge vào phần hướng dẫn

<details><summary>Xem đáp án</summary>

**B.** Các nguyên tắc viết prompt tốt (Domain 4) cũng áp dụng cho Project instructions. Copy tài liệu vào phần hướng dẫn (D) là trùng lặp và lẫn lộn mục đích.
</details>

### Câu 13
Bạn tải lên 10 file PDF dạng ảnh scan chất lượng thấp. Claude trả lời thiếu chính xác về nội dung. Bước cải thiện hợp lý nhất là gì?

- A. Tải lên thêm 10 bản scan nữa
- B. Đổi tên file
- C. Cung cấp bản tài liệu có văn bản rõ ràng (bản gốc dạng text hoặc bản OCR đã kiểm tra) thay cho ảnh scan mờ
- D. Viết prompt dài hơn

<details><summary>Xem đáp án</summary>

**C.** Chất lượng đầu vào ảnh hưởng trực tiếp đến chất lượng đầu ra. Tài liệu rõ ràng giúp Claude đọc đúng nội dung.
</details>

### Câu 14
Khi nào nên tạo **nhiều Project riêng biệt** thay vì một Project chung?

- A. Khi các nhóm, tác vụ hoặc bộ tài liệu khác nhau rõ rệt về mục đích, giọng văn hoặc quyền truy cập
- B. Không bao giờ, một Project là đủ cho cả công ty
- C. Mỗi cuộc trò chuyện tạo một Project
- D. Khi muốn Claude trả lời chậm hơn

<details><summary>Xem đáp án</summary>

**A.** Tách Project theo mục đích và quyền truy cập giúp tri thức tập trung, tránh nhiễu và bảo vệ dữ liệu.
</details>

### Câu 15
Công ty muốn Claude trả lời đúng theo bảng giá mới nhất, cập nhật hằng ngày trong hệ thống nội bộ. Giải pháp phù hợp nhất là gì?

- A. Tải bảng giá vào Project một lần duy nhất
- B. Để Claude tự nhớ giá
- C. Nhắc Claude trong mỗi tin nhắn "giá có thể đã đổi"
- D. Kết nối Claude với nguồn dữ liệu cập nhật (connector/MCP hoặc tích hợp API) để truy xuất giá hiện hành khi trả lời

<details><summary>Xem đáp án</summary>

**D.** Dữ liệu thay đổi thường xuyên nên được truy xuất trực tiếp từ nguồn. Tải lên một lần (A) sẽ nhanh chóng lỗi thời.
</details>

---

## Chấm điểm
- 13–15: Vững
- 10–12: Ôn lại các câu sai, đọc lại [ghi chú Domain 6](../01-domains/06-configuration-knowledge.md)
- < 10: Làm BT3 trong [danh sách bài tập](../02-bai-tap/danh-sach-bai-tap.md), rồi làm lại đề sau 2 ngày

Ghi các câu sai vào [ket-qua.md](ket-qua.md).
