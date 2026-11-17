# Đề luyện tập 07 — Domain 7: Troubleshooting & Optimization (10%)

15 câu · khuyến nghị 30 phút · mỗi câu chọn 1 đáp án.
Đáp án và giải thích nằm trong phần "Xem đáp án" — làm hết rồi mới mở.

**Bảng trả lời:** 1.__ 2.__ 3.__ 4.__ 5.__ 6.__ 7.__ 8.__ 9.__ 10.__ 11.__ 12.__ 13.__ 14.__ 15.__

---

### Câu 1
Claude liên tục trả lời quá dài so với nhu cầu. Cách sửa hiệu quả nhất là gì?

- A. Đổi sang model lớn hơn
- B. Chỉ định rõ độ dài mong muốn (ví dụ "tối đa 3 câu" hoặc "khoảng 100 từ") và cho ví dụ đầu ra mẫu
- C. Viết "ngắn thôi!!!" bằng chữ in hoa
- D. Tự cắt bớt câu trả lời mỗi lần

<details><summary>Xem đáp án</summary>

**B.** Ràng buộc cụ thể, đo được, kèm ví dụ hiệu quả hơn chỉ dẫn cảm tính. Tự cắt thủ công (D) không giải quyết nguyên nhân.
</details>

### Câu 2
Claude bỏ sót bước 4 trong một quy trình 7 bước được mô tả trong một đoạn văn dài. Cách khắc phục hợp lý nhất là gì?

- A. Lặp lại toàn bộ đoạn văn hai lần
- B. Đổi ngôn ngữ prompt
- C. Bỏ bước 4 khỏi quy trình
- D. Trình bày các bước dưới dạng danh sách đánh số rõ ràng, yêu cầu Claude xác nhận đã hoàn thành từng bước, hoặc chia thành nhiều prompt nối tiếp

<details><summary>Xem đáp án</summary>

**D.** Cấu trúc rõ ràng (danh sách đánh số, checklist) và chia nhỏ tác vụ giúp giảm bỏ sót.
</details>

### Câu 3
Cùng một prompt nhưng mỗi lần chạy Claude cho định dạng đầu ra khác nhau, làm hỏng bước xử lý tự động phía sau. Cách sửa phù hợp nhất là gì?

- A. Chỉ định định dạng chính xác (schema), đưa ví dụ mẫu, và dùng structured output nếu có; thêm bước kiểm tra định dạng tự động
- B. Chạy nhiều lần đến khi đúng
- C. Bỏ bước xử lý tự động
- D. Yêu cầu Claude "nhất quán hơn"

<details><summary>Xem đáp án</summary>

**A.** Định dạng rõ ràng kèm cơ chế kiểm tra giúp đầu ra ổn định. "Nhất quán hơn" (D) quá mơ hồ.
</details>

### Câu 4
Claude trả lời sai một thông tin về sản phẩm của công ty. Bước chẩn đoán **đầu tiên** nên làm là gì?

- A. Đổi sang model khác ngay
- B. Báo cáo lỗi cho Anthropic
- C. Kiểm tra xem Claude có được cung cấp thông tin đúng không (tài liệu nguồn có, có cập nhật, có mâu thuẫn không) và prompt có yêu cầu dựa trên nguồn không
- D. Ngừng dùng Claude

<details><summary>Xem đáp án</summary>

**C.** Phần lớn lỗi thông tin đến từ thiếu nguồn, nguồn lỗi thời hoặc prompt không yêu cầu bám nguồn. Kiểm tra đầu vào trước khi đổi công cụ.
</details>

### Câu 5
Chi phí sử dụng Claude API của một ứng dụng tăng cao. Cách tối ưu **không làm giảm chất lượng** đáng kể là gì?

- A. Rút gọn ngữ cảnh gửi đi (chỉ gửi phần liên quan), dùng model nhỏ hơn cho tác vụ đơn giản, và tận dụng prompt caching cho phần prompt lặp lại
- B. Giảm số người dùng
- C. Chuyển toàn bộ sang model nhỏ nhất ngay
- D. Gửi toàn bộ cơ sở dữ liệu trong mỗi yêu cầu để Claude có đủ thông tin

<details><summary>Xem đáp án</summary>

**A.** Tối ưu ngữ cảnh, định tuyến model theo độ khó và caching là các cách giảm chi phí phổ biến. Gửi toàn bộ dữ liệu (D) làm tăng chi phí.
</details>

### Câu 6
Claude dùng giọng văn quá trang trọng cho bài đăng mạng xã hội hướng đến người trẻ. Cách sửa tốt nhất là gì?

- A. Đổi sang model nhỏ hơn
- B. Tự viết lại toàn bộ
- C. Mô tả rõ đối tượng độc giả và giọng văn mong muốn, kèm 1–2 bài mẫu đúng phong cách
- D. Yêu cầu "viết hay hơn"

<details><summary>Xem đáp án</summary>

**C.** Mô tả đối tượng kèm ví dụ mẫu là cách điều chỉnh giọng văn hiệu quả nhất. "Viết hay hơn" (D) không cho biết hướng sửa.
</details>

### Câu 7
Claude từ chối một yêu cầu công việc hợp lệ (ví dụ: phân tích các phương thức tấn công phishing để đào tạo nhân viên về bảo mật). Cách xử lý phù hợp là gì?

- A. Tìm cách đánh lừa Claude bằng câu chuyện giả
- B. Bổ sung ngữ cảnh rõ ràng và trung thực về mục đích (đào tạo phòng chống) và đối tượng sử dụng
- C. Bỏ cuộc
- D. Lặp lại yêu cầu 10 lần

<details><summary>Xem đáp án</summary>

**B.** Từ chối không cần thiết thường được khắc phục bằng ngữ cảnh rõ ràng, trung thực. Đánh lừa (A) vi phạm sử dụng có trách nhiệm (Domain 3).
</details>

### Câu 8
Một prompt từng hoạt động tốt, nhưng sau khi đổi sang phiên bản model mới thì kết quả khác đi. Cách tiếp cận đúng là gì?

- A. Giữ model cũ mãi mãi
- B. Bỏ qua sự khác biệt
- C. Viết lại prompt từ đầu mà không so sánh
- D. Chạy lại bộ test case chuẩn trên model mới, so sánh kết quả, điều chỉnh prompt nếu cần trước khi chuyển hẳn

<details><summary>Xem đáp án</summary>

**D.** Có bộ test chuẩn (regression test) giúp đánh giá tác động khi đổi model và điều chỉnh có căn cứ.
</details>

### Câu 9
Claude trả lời chậm trong một ứng dụng chat thời gian thực, gây khó chịu cho người dùng. Cách cải thiện hợp lý là gì?

- A. Thêm thông tin vào prompt để Claude hiểu rõ hơn
- B. Bật extended thinking ở mức cao
- C. Dùng model nhanh hơn cho tác vụ này nếu chất lượng vẫn đạt, rút gọn prompt, và hiển thị câu trả lời dạng streaming
- D. Yêu cầu người dùng chờ

<details><summary>Xem đáp án</summary>

**C.** Chọn model nhanh hơn, giảm ngữ cảnh và streaming đều cải thiện trải nghiệm tốc độ. Extended thinking (B) làm tăng thời gian phản hồi.
</details>

### Câu 10
Bạn muốn biết thay đổi prompt có thực sự cải thiện kết quả hay không. Cách làm đúng là gì?

- A. So sánh phiên bản cũ và mới trên cùng một bộ đầu vào đại diện, chấm theo tiêu chí định trước
- B. Thử phiên bản mới một lần, thấy ổn là dùng
- C. Hỏi Claude xem prompt mới có tốt hơn không
- D. Chọn phiên bản dài hơn

<details><summary>Xem đáp án</summary>

**A.** Tối ưu cần đo lường có hệ thống. Thử một lần (B) không đủ vì đầu ra có thể khác nhau giữa các lần chạy. Câu này kết hợp với Domain 1.
</details>

### Câu 11
Claude tóm tắt tài liệu nhưng bỏ qua các con số quan trọng. Cách khắc phục cụ thể nhất là gì?

- A. Yêu cầu "tóm tắt tốt hơn"
- B. Nêu rõ trong prompt các thông tin bắt buộc phải có (ví dụ: doanh thu, tỷ lệ tăng trưởng, thời hạn) và định dạng trình bày chúng
- C. Đổi sang file Word
- D. Tóm tắt bằng tay

<details><summary>Xem đáp án</summary>

**B.** Liệt kê rõ các yếu tố bắt buộc giúp đầu ra đầy đủ theo đúng nhu cầu.
</details>

### Câu 12
Claude trong Project trả lời không theo hướng dẫn đã viết. Các bước kiểm tra hợp lý là gì?

- A. Xóa Project
- B. Đổi tài khoản
- C. Đổi sang model nhỏ hơn
- D. Kiểm tra hướng dẫn có rõ ràng, cụ thể không; có mâu thuẫn với tài liệu trong Knowledge hoặc với yêu cầu trong tin nhắn không; thử điều chỉnh và kiểm tra lại

<details><summary>Xem đáp án</summary>

**D.** Mâu thuẫn hoặc mơ hồ giữa các nguồn chỉ dẫn là nguyên nhân phổ biến. Kiểm tra có hệ thống trước khi thay đổi lớn.
</details>

### Câu 13
Bạn giao một tác vụ lớn (viết báo cáo 30 trang) trong một prompt và chất lượng các phần cuối giảm rõ rệt. Cách tối ưu là gì?

- A. Lập dàn ý trước, sau đó viết từng phần theo dàn ý, rồi rà soát tổng thể
- B. Yêu cầu viết nhanh hơn
- C. Giảm báo cáo xuống còn 1 trang
- D. Chấp nhận chất lượng thấp ở các phần cuối

<details><summary>Xem đáp án</summary>

**A.** Chia tác vụ lớn thành các bước (dàn ý, từng phần, rà soát) giúp duy trì chất lượng đồng đều.
</details>

### Câu 14
Người dùng phàn nàn Claude "hay bịa thông tin" trong chatbot nội bộ. Sau khi điều tra, bạn thấy prompt hệ thống ghi: "Luôn đưa ra câu trả lời đầy đủ cho mọi câu hỏi." Vấn đề nằm ở đâu?

- A. Model quá nhỏ
- B. Người dùng hỏi quá nhiều
- C. Chỉ dẫn này gây áp lực phải trả lời ngay cả khi không có thông tin; cần cho phép Claude nói "không biết" và chỉ trả lời dựa trên nguồn
- D. Thiếu extended thinking

<details><summary>Xem đáp án</summary>

**C.** Chỉ dẫn vô tình khuyến khích bịa thông tin là nguyên nhân phổ biến của hallucination. Sửa ở gốc (prompt) chứ không phải đổi model.
</details>

### Câu 15
Quy trình xử lý sự cố (troubleshooting) hợp lý nhất khi đầu ra của Claude không đạt yêu cầu là gì?

- A. Đổi model, đổi công cụ, rồi bỏ cuộc
- B. Thay đổi nhiều thứ cùng lúc để nhanh có kết quả
- C. Hỏi Claude tại sao nó sai và làm theo đề xuất mà không kiểm tra
- D. Xác định rõ vấn đề bằng ví dụ cụ thể → kiểm tra đầu vào (prompt, nguồn, cấu hình) → thay đổi từng yếu tố một → kiểm tra lại trên bộ test → ghi lại kết quả

<details><summary>Xem đáp án</summary>

**D.** Chẩn đoán có hệ thống, thay đổi từng biến một và đo lường giúp biết chính xác điều gì có tác dụng. Thay đổi nhiều thứ cùng lúc (B) khiến không biết thay đổi nào có hiệu quả.
</details>

---

## Chấm điểm
- 13–15: Vững
- 10–12: Ôn lại các câu sai, đọc lại [ghi chú Domain 7](../01-domains/07-troubleshooting.md)
- < 10: Làm BT6 trong [danh sách bài tập](../02-bai-tap/danh-sach-bai-tap.md), rồi làm lại đề sau 2 ngày

Ghi các câu sai vào [ket-qua.md](ket-qua.md).
