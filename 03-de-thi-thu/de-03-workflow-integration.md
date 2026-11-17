# Đề luyện tập 03 — Domain 2: Workflow Integration & Solution Design (16%)

15 câu · khuyến nghị 30 phút · mỗi câu chọn 1 đáp án.
Đáp án và giải thích nằm trong phần "Xem đáp án" — làm hết rồi mới mở.

**Bảng trả lời:** 1.__ 2.__ 3.__ 4.__ 5.__ 6.__ 7.__ 8.__ 9.__ 10.__ 11.__ 12.__ 13.__ 14.__ 15.__

---

### Câu 1
Giám đốc muốn "áp dụng Claude cho toàn công ty ngay tuần này". Bước khởi đầu hợp lý nhất là gì?

- A. Mua license cho tất cả nhân viên và để mọi người tự dùng
- B. Chọn 1–2 quy trình cụ thể, tốn thời gian và rủi ro thấp, chạy thử với một nhóm nhỏ, đo lường kết quả rồi mới mở rộng
- C. Tự động hóa ngay quy trình quan trọng nhất của công ty
- D. Chờ đến khi AI hoàn hảo rồi mới áp dụng

<details><summary>Xem đáp án</summary>

**B.** Bắt đầu bằng thí điểm (pilot) ở quy trình rủi ro thấp, có tiêu chí đo lường, rồi mở rộng dựa trên kết quả. Tự động hóa ngay quy trình trọng yếu (C) rủi ro cao. Triển khai đại trà không định hướng (A) khó tạo ra giá trị đo được.
</details>

### Câu 2
Quy trình nào **phù hợp nhất** để đưa Claude vào làm trước?

- A. Phê duyệt khoản vay cuối cùng cho khách hàng
- B. Quyết định sa thải nhân viên
- C. Ký hợp đồng thay mặt công ty
- D. Soạn bản nháp email trả lời các câu hỏi thường gặp, có nhân viên xem lại trước khi gửi

<details><summary>Xem đáp án</summary>

**D.** Tác vụ lặp lại, khối lượng lớn, rủi ro thấp và có người duyệt là điểm khởi đầu lý tưởng. Các quyết định A, B, C ảnh hưởng lớn đến con người hoặc pháp lý, cần con người quyết định.
</details>

### Câu 3
"Human-in-the-loop" trong thiết kế quy trình có AI nghĩa là gì?

- A. Con người tham gia ở những điểm then chốt (duyệt, quyết định, xử lý ngoại lệ) trong quy trình có AI
- B. Con người làm toàn bộ, AI chỉ quan sát
- C. AI giám sát con người
- D. Con người chỉ tham gia khi hệ thống bị lỗi

<details><summary>Xem đáp án</summary>

**A.** Human-in-the-loop là thiết kế có chủ đích các điểm con người kiểm soát, đặc biệt ở bước quyết định và bước có rủi ro. Không phải chỉ khi có lỗi (D).
</details>

### Câu 4
Nhóm sales muốn Claude: đọc ghi chú cuộc gọi, cập nhật CRM, soạn email follow-up và gửi luôn cho khách. Thiết kế nào hợp lý nhất?

- A. Cho Claude tự động làm hết, kể cả gửi email
- B. Không dùng Claude vì quy trình quá phức tạp
- C. Claude trích xuất thông tin và soạn bản nháp; nhân viên kiểm tra thông tin CRM và duyệt email trước khi gửi
- D. Claude chỉ được sửa lỗi chính tả trong ghi chú

<details><summary>Xem đáp án</summary>

**C.** AI làm phần tốn công (trích xuất, soạn nháp); con người giữ quyền ở bước tác động ra bên ngoài (gửi email cho khách). Tự động hoàn toàn (A) có rủi ro gửi sai thông tin cho khách.
</details>

### Câu 5
Trước khi thí điểm Claude cho bộ phận kế toán, việc quan trọng nhất cần xác định là gì?

- A. Tiêu chí thành công đo được (thời gian xử lý, tỷ lệ lỗi, mức hài lòng) và mức hiện tại để so sánh
- B. Màu giao diện ưa thích của nhân viên
- C. Model nào mới nhất
- D. Số lượng prompt tối đa mỗi ngày

<details><summary>Xem đáp án</summary>

**A.** Không có tiêu chí và mốc so sánh (baseline) thì không thể chứng minh giải pháp có hiệu quả hay không.
</details>

### Câu 6
Một tác vụ phức tạp: đọc 20 đơn khiếu nại, phân loại, tìm nguyên nhân gốc, đề xuất cải tiến. Thiết kế quy trình nào tốt nhất?

- A. Một prompt duy nhất xử lý tất cả 20 đơn và đưa ra đề xuất
- B. Giao hết cho một nhân viên mới
- C. Chia thành các bước: phân loại từng đơn → tổng hợp theo nhóm → phân tích nguyên nhân → đề xuất; có người kiểm tra ở các bước then chốt
- D. Chỉ đọc 5 đơn đầu tiên cho nhanh

<details><summary>Xem đáp án</summary>

**C.** Chia nhỏ tác vụ (task decomposition) giúp mỗi bước dễ kiểm tra và chất lượng cao hơn. Lấy mẫu 5 đơn (D) có thể bỏ sót vấn đề quan trọng.
</details>

### Câu 7
Trường hợp nào **không nên** dùng Claude làm giải pháp chính?

- A. Soạn bản nháp tài liệu đào tạo
- B. Tính toán bảng lương chính xác đến từng đồng cho hàng nghìn nhân viên, trong khi hệ thống phần mềm tính lương đã có sẵn
- C. Tóm tắt phản hồi khảo sát khách hàng
- D. Brainstorm ý tưởng chiến dịch marketing

<details><summary>Xem đáp án</summary>

**B.** Tác vụ tính toán xác định, cần chính xác tuyệt đối và đã có công cụ chuyên dụng thì không nên thay bằng AI tạo sinh. Một giải pháp tốt là chọn đúng công cụ cho đúng việc, không phải dùng AI cho mọi thứ.
</details>

### Câu 8
Sau 1 tháng thí điểm, nhóm nhận thấy thời gian soạn báo cáo giảm 40% nhưng tỷ lệ lỗi tăng nhẹ. Bước tiếp theo hợp lý nhất là gì?

- A. Dừng ngay dự án
- B. Mở rộng ra toàn công ty vì đã tiết kiệm thời gian
- C. Bỏ qua tỷ lệ lỗi vì không đáng kể
- D. Phân tích các lỗi để tìm nguyên nhân, cải thiện prompt hoặc bổ sung bước kiểm tra, rồi đo lại trước khi mở rộng

<details><summary>Xem đáp án</summary>

**D.** Cải tiến lặp lại dựa trên dữ liệu: giữ lợi ích, xử lý vấn đề, rồi mới mở rộng. Mở rộng khi chất lượng chưa ổn (B) sẽ nhân rủi ro lên.
</details>

### Câu 9
Nhân viên lo ngại "AI sẽ thay thế công việc của tôi" và không muốn dùng Claude. Cách tiếp cận nào hiệu quả nhất?

- A. Bắt buộc sử dụng, ai không dùng sẽ bị đánh giá thấp
- B. Bỏ qua mối lo ngại
- C. Giải thích rõ vai trò của AI là hỗ trợ, đào tạo cách dùng, cho nhân viên tham gia thiết kế quy trình và thấy lợi ích thực tế
- D. Chỉ cho quản lý dùng AI

<details><summary>Xem đáp án</summary>

**C.** Quản lý thay đổi (change management) bằng đào tạo, minh bạch và cho người dùng tham gia giúp tăng mức độ áp dụng bền vững.
</details>

### Câu 10
Một quy trình cần Claude trả lời câu hỏi nội bộ dựa trên sổ tay nhân viên 200 trang, cập nhật mỗi quý. Thiết kế phù hợp nhất là gì?

- A. Đưa sổ tay vào Project Knowledge (hoặc nguồn kết nối), chỉ định Claude chỉ trả lời từ đó, và có quy trình cập nhật tài liệu mỗi quý
- B. Để Claude trả lời từ kiến thức chung
- C. Mỗi nhân viên tự dán sổ tay vào mỗi lần hỏi
- D. In sổ tay ra giấy

<details><summary>Xem đáp án</summary>

**A.** Có nguồn tri thức tập trung, câu trả lời dựa vào nguồn đó, và có quy trình bảo trì nội dung. Tự dán mỗi lần (C) không nhất quán và dễ dùng bản cũ.
</details>

### Câu 11
Khi thiết kế giải pháp, "điểm leo thang" (escalation point) là gì?

- A. Lúc tăng gói đăng ký Claude
- B. Lúc chuyển sang model lớn hơn
- C. Lúc Claude trả lời dài hơn
- D. Điều kiện mà khi gặp phải, tác vụ được chuyển từ AI sang con người xử lý (ví dụ: khách hàng tức giận, yêu cầu ngoài chính sách, độ tin cậy thấp)

<details><summary>Xem đáp án</summary>

**D.** Xác định rõ khi nào AI chuyển việc cho người là một phần cốt lõi của thiết kế quy trình an toàn.
</details>

### Câu 12
Một nhóm 5 người dùng Claude viết nội dung, nhưng mỗi người dùng prompt khác nhau nên chất lượng và giọng văn không đồng đều. Giải pháp tốt nhất là gì?

- A. Mỗi người tự cải thiện prompt của mình
- B. Chuẩn hóa: dùng chung Project có hướng dẫn giọng văn, template prompt và ví dụ mẫu; chia sẻ cách làm tốt
- C. Chỉ cho một người dùng Claude
- D. Đổi sang model khác

<details><summary>Xem đáp án</summary>

**B.** Chuẩn hóa cấu hình và tri thức dùng chung giúp đầu ra nhất quán trong nhóm. Câu này kết hợp với Domain 6.
</details>

### Câu 13
Đâu là cách đo **giá trị kinh doanh** của giải pháp Claude tốt nhất?

- A. So sánh các chỉ số kinh doanh trước và sau (thời gian xử lý, chi phí, chất lượng, mức hài lòng) cho cùng một quy trình
- B. Đếm số lượng prompt đã gửi
- C. Đếm số nhân viên đã đăng nhập
- D. Hỏi Claude giải pháp có hiệu quả không

<details><summary>Xem đáp án</summary>

**A.** Giá trị nằm ở kết quả kinh doanh, không ở mức độ sử dụng. Số prompt hay số lần đăng nhập (B, C) chỉ là chỉ số hoạt động, không phải giá trị.
</details>

### Câu 14
Bạn thiết kế quy trình để Claude hỗ trợ trả lời ticket kỹ thuật. Thứ tự nào hợp lý nhất?

- A. Triển khai cho toàn bộ khách hàng, sau đó mới viết hướng dẫn
- B. Viết prompt, triển khai ngay, không cần thử
- C. Xác định phạm vi và tiêu chí → chuẩn bị nguồn tri thức → thiết kế prompt và điểm leo thang → thử trên ticket cũ → thí điểm có người duyệt → đo lường → mở rộng
- D. Chọn model trước, rồi tìm việc để model làm

<details><summary>Xem đáp án</summary>

**C.** Quy trình bắt đầu từ vấn đề và tiêu chí, kiểm thử trên dữ liệu thật trước, rồi mở rộng có kiểm soát. Chọn công cụ trước rồi mới tìm vấn đề (D) là ngược.
</details>

### Câu 15
Claude được dùng để soạn bản đề xuất gửi khách hàng. Ai chịu trách nhiệm cuối cùng về nội dung bản đề xuất?

- A. Claude
- B. Anthropic
- C. Bộ phận IT đã cài đặt công cụ
- D. Người hoặc bộ phận gửi bản đề xuất đi, sau khi đã kiểm tra và phê duyệt

<details><summary>Xem đáp án</summary>

**D.** AI là công cụ hỗ trợ; trách nhiệm về đầu ra được sử dụng luôn thuộc về con người hoặc tổ chức sử dụng. Câu này kết hợp với Domain 3 (Governance).
</details>

---

## Chấm điểm
- 13–15: Vững
- 10–12: Ôn lại các câu sai, đọc lại [ghi chú Domain 2](../01-domains/02-workflow-integration.md)
- < 10: Đọc lại ghi chú, rồi làm lại đề sau 2 ngày

Ghi các câu sai vào [ket-qua.md](ket-qua.md).
