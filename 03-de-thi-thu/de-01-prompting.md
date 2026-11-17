# Đề luyện tập 01 — Domain 4: Prompting & Task Execution

15 câu · khuyến nghị 30 phút · mỗi câu chọn 1 đáp án.
Đáp án và giải thích nằm trong phần "Xem đáp án" — làm hết rồi mới mở.

**Bảng trả lời:** 1.__ 2.__ 3.__ 4.__ 5.__ 6.__ 7.__ 8.__ 9.__ 10.__ 11.__ 12.__ 13.__ 14.__ 15.__

---

### Câu 1
Một nhân viên marketing nhờ Claude: *"Viết bài về sản phẩm mới."* Kết quả chung chung, không dùng được. Cách cải thiện **hiệu quả nhất** là gì?

- A. Chuyển sang model lớn hơn
- B. Viết prompt bằng chữ IN HOA để nhấn mạnh
- C. Bổ sung đối tượng độc giả, mục đích bài, độ dài, giọng văn và các điểm chính cần nêu
- D. Yêu cầu Claude viết lại nhiều lần cho đến khi ưng

<details><summary>Xem đáp án</summary>

**C.** Đầu ra chung chung thường là do prompt thiếu ngữ cảnh. Cung cấp độc giả, mục đích, ràng buộc và nội dung chính là cách cải thiện trực tiếp nhất. Đổi model (A) không bù được ngữ cảnh còn thiếu. In hoa (B) không giúp prompt rõ hơn. Viết lại nhiều lần (D) tốn thời gian mà không giải quyết nguyên nhân.
</details>

### Câu 2
Bạn cần Claude phân tích một hợp đồng dài 30 trang và trả lời 3 câu hỏi. Cách sắp xếp prompt nào được khuyến nghị?

- A. Đặt hợp đồng (bọc trong thẻ như `<contract>`) ở đầu, câu hỏi và chỉ dẫn ở cuối
- B. Đặt 3 câu hỏi lên đầu, hợp đồng ở cuối
- C. Chia hợp đồng thành 30 tin nhắn riêng
- D. Chỉ dán phần mục lục để tiết kiệm token

<details><summary>Xem đáp án</summary>

**A.** Với tài liệu dài, nên đặt tài liệu lên đầu và câu hỏi/chỉ dẫn ở cuối, đồng thời dùng thẻ XML để tách tài liệu khỏi chỉ dẫn. Cách này thường cho chất lượng trả lời tốt hơn. Chỉ dán mục lục (D) thì mất thông tin cần thiết.
</details>

### Câu 3
Mục đích chính của việc dùng thẻ XML (ví dụ `<email>`, `<instructions>`) trong prompt là gì?

- A. Để Claude trả lời bằng XML
- B. Bắt buộc phải có để Claude hiểu tiếng Việt
- C. Mã hóa dữ liệu nhạy cảm
- D. Tách bạch rõ ràng các phần: dữ liệu, chỉ dẫn, ví dụ, giúp Claude không nhầm lẫn

<details><summary>Xem đáp án</summary>

**D.** Thẻ XML giúp cấu trúc prompt: Claude phân biệt được đâu là dữ liệu cần xử lý, đâu là chỉ dẫn. Thẻ không bắt buộc (B) và không có tác dụng bảo mật hay mã hóa (C).
</details>

### Câu 4
Đội CSKH muốn Claude phân loại email thành 4 nhãn nhưng kết quả không nhất quán. Bước nên làm **đầu tiên** là gì?

- A. Bỏ AI, quay lại phân loại thủ công
- B. Thêm vài ví dụ mẫu (few-shot) cho từng nhãn, kèm định nghĩa rõ mỗi nhãn
- C. Tăng độ dài email đầu vào
- D. Yêu cầu Claude "cố gắng hơn"

<details><summary>Xem đáp án</summary>

**B.** Ví dụ mẫu kèm định nghĩa nhãn rõ ràng là cách hiệu quả để Claude phân loại nhất quán. "Cố gắng hơn" (D) không cho Claude thêm thông tin gì. Bỏ AI (A) là quá vội khi chưa thử cải thiện prompt.
</details>

### Câu 5
Khi đưa ví dụ mẫu (few-shot), điều nào **nên** làm?

- A. Dùng một ví dụ duy nhất, lặp lại 5 lần
- B. Chỉ dùng ví dụ dễ để Claude không bị rối
- C. Dùng các ví dụ đa dạng, sát với tình huống thực tế, bao gồm cả trường hợp khó
- D. Không cần ví dụ khớp với định dạng đầu ra mong muốn

<details><summary>Xem đáp án</summary>

**C.** Ví dụ nên đa dạng, sát thực tế và có cả trường hợp biên, để Claude không bám vào một khuôn duy nhất. Ví dụ cũng nên đúng định dạng đầu ra mong muốn (nên D sai).
</details>

### Câu 6
Một nhà phân tích cần Claude giải một bài toán định giá nhiều bước. Kết quả hay sai ở bước trung gian. Kỹ thuật nào phù hợp nhất?

- A. Yêu cầu chỉ trả về con số cuối cùng
- B. Giảm độ dài prompt
- C. Dùng model nhỏ nhất để chạy nhanh
- D. Cho Claude suy luận từng bước (chain of thought) hoặc bật extended thinking trước khi đưa kết luận

<details><summary>Xem đáp án</summary>

**D.** Với bài toán nhiều bước, để Claude suy luận từng bước (hoặc bật extended thinking) giúp tăng độ chính xác và giúp người dùng dễ kiểm tra từng bước. Chỉ lấy con số cuối (A) làm mất khả năng kiểm tra.
</details>

### Câu 7
Gán vai trò ("Bạn là chuyên gia pháp lý về hợp đồng thương mại…") có tác dụng chính là gì?

- A. Định hướng giọng văn, góc nhìn và mức độ chuyên môn của câu trả lời
- B. Biến Claude thành luật sư có chứng chỉ, nên không cần người duyệt
- C. Vô hiệu hóa các chính sách an toàn
- D. Không có tác dụng gì

<details><summary>Xem đáp án</summary>

**A.** Gán vai trò giúp định hướng chuyên môn và giọng văn. Nó **không** thay thế việc chuyên gia thật duyệt lại (B sai), và cũng không bỏ qua được chính sách an toàn (C sai).
</details>

### Câu 8
Bạn muốn Claude trả về JSON để đưa vào hệ thống khác, nhưng đôi khi Claude thêm lời dẫn trước JSON. Cách xử lý tốt nhất là gì?

- A. Nhờ một người xóa lời dẫn thủ công mỗi lần
- B. Chỉ định rõ schema mong muốn, cho ví dụ JSON mẫu và yêu cầu chỉ trả về JSON (hoặc dùng structured output nếu có)
- C. Yêu cầu trả về dạng bảng thay vì JSON
- D. Tăng nhiệt độ (temperature)

<details><summary>Xem đáp án</summary>

**B.** Chỉ định rõ định dạng, cho ví dụ mẫu và dùng tính năng structured output (nếu có) là cách đảm bảo đầu ra đúng định dạng. Tăng temperature (D) chỉ làm đầu ra kém ổn định hơn.
</details>

### Câu 9
Một tác vụ gồm: (1) trích xuất dữ liệu từ báo cáo, (2) phân tích xu hướng, (3) viết email tóm tắt cho sếp. Chất lượng kém khi gộp tất cả vào một prompt. Nên làm gì?

- A. Viết prompt dài gấp đôi
- B. Bỏ bước phân tích
- C. Chạy cùng prompt 3 lần rồi chọn bản tốt nhất
- D. Chia thành chuỗi prompt (prompt chaining), đầu ra bước trước làm đầu vào bước sau, kiểm tra ở từng bước

<details><summary>Xem đáp án</summary>

**D.** Prompt chaining giúp mỗi bước tập trung vào một việc, dễ kiểm tra và dễ sửa lỗi ở đúng chỗ.
</details>

### Câu 10
Cách viết chỉ dẫn nào **tốt hơn**?

- A. "Đừng viết dài dòng, đừng dùng markdown."
- B. "KHÔNG ĐƯỢC dài!!!"
- C. "Viết thành 2–3 đoạn văn xuôi ngắn gọn, không dùng gạch đầu dòng."
- D. "Viết sao cũng được."

<details><summary>Xem đáp án</summary>

**C.** Nói rõ điều **cần làm** (kèm con số cụ thể) hiệu quả hơn chỉ nói điều cần tránh. C cho Claude một mục tiêu cụ thể để làm theo.
</details>

### Câu 11
Người dùng muốn Claude viết email từ chối khách hàng một cách lịch sự. Thông tin nào **quan trọng nhất** cần cung cấp thêm?

- A. Lý do từ chối, mối quan hệ với khách, giọng văn mong muốn và hướng giải quyết thay thế (nếu có)
- B. Logo công ty
- C. Lịch sử phát triển của Claude
- D. Tên model đang dùng

<details><summary>Xem đáp án</summary>

**A.** Đây là ngữ cảnh ảnh hưởng trực tiếp đến nội dung và giọng văn của email.
</details>

### Câu 12
Bạn dùng một prompt mẫu cho báo cáo hằng tuần, mỗi tuần chỉ thay số liệu. Cách tổ chức nào hợp lý?

- A. Viết prompt mới hoàn toàn mỗi tuần
- B. Nhờ Claude tự đoán số liệu
- C. Copy nguyên đầu ra của tuần trước
- D. Tạo template cố định với các biến (ví dụ `{{doanh_thu}}`), lưu vào Project hoặc Skill để tái sử dụng

<details><summary>Xem đáp án</summary>

**D.** Template có biến giúp kết quả nhất quán qua các tuần và dễ bảo trì. Để Claude tự đoán số liệu (B) dẫn đến hallucination.
</details>

### Câu 13
Sau khi nhận đầu ra chưa đạt, cách lặp (iterate) hiệu quả là gì?

- A. Xóa hội thoại, gửi lại đúng prompt cũ
- B. Trả lời "chưa được, làm lại"
- C. Phản hồi cụ thể điều gì chưa đạt và cần sửa thế nào ("Phần 2 quá kỹ thuật; viết lại cho người không chuyên, tối đa 100 từ")
- D. Đổi sang công cụ AI khác

<details><summary>Xem đáp án</summary>

**C.** Phản hồi cụ thể, nói rõ cần sửa gì, giúp Claude chỉnh đúng chỗ. Phản hồi mơ hồ (B) cho kết quả khó đoán.
</details>

### Câu 14
Khi muốn Claude trả lời câu hỏi dựa trên tài liệu nội bộ và **giảm hallucination**, chỉ dẫn nào phù hợp nhất?

- A. "Trả lời thật tự tin."
- B. "Chỉ dựa trên tài liệu được cung cấp; trích dẫn đoạn liên quan; nếu tài liệu không có thông tin, hãy nói rõ là không tìm thấy."
- C. "Dùng kiến thức chung nếu tài liệu thiếu, không cần nói."
- D. "Trả lời ngắn nhất có thể."

<details><summary>Xem đáp án</summary>

**B.** Buộc trả lời dựa trên tài liệu, kèm trích dẫn và cho phép nói "không biết", là ba kỹ thuật chính để giảm hallucination. Câu này cũng liên quan đến Domain 1.
</details>

### Câu 15
Một nhân viên dán dữ liệu bảng lương của toàn công ty vào Claude để "viết báo cáo nhanh". Phản ứng phù hợp nhất về mặt quy trình là gì?

- A. Kiểm tra chính sách dữ liệu của công ty và gói Claude đang dùng; ẩn danh hoặc tổng hợp dữ liệu trước nếu không được phép đưa dữ liệu cá nhân
- B. Không sao, miễn prompt viết tốt
- C. Đổi sang prompt tiếng Anh
- D. Chia dữ liệu làm hai lần dán

<details><summary>Xem đáp án</summary>

**A.** Một prompt tốt không thay thế được tuân thủ quản trị dữ liệu. Câu này kết hợp Domain 4 với Domain 3: đề thi hay gộp nhiều domain vào một câu tình huống.
</details>

---

## Chấm điểm
- 13–15: Vững, chuyển sang domain tiếp theo
- 10–12: Ôn lại các câu sai
- < 10: Đọc lại tài liệu prompt engineering, rồi làm lại đề sau 2 ngày

Ghi các câu sai vào [ket-qua.md](ket-qua.md).
