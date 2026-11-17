# Đề luyện tập 02 — Domain 1: Output Evaluation & Validation (21%)

15 câu · khuyến nghị 30 phút · mỗi câu chọn 1 đáp án.
Đáp án và giải thích nằm trong phần "Xem đáp án" — làm hết rồi mới mở.

**Bảng trả lời:** 1.__ 2.__ 3.__ 4.__ 5.__ 6.__ 7.__ 8.__ 9.__ 10.__ 11.__ 12.__ 13.__ 14.__ 15.__

---

### Câu 1
Claude viết báo cáo thị trường, trong đó trích dẫn "một nghiên cứu của McKinsey năm 2024 cho thấy 67% doanh nghiệp…". Bạn không cung cấp nghiên cứu này cho Claude. Việc nên làm trước khi dùng báo cáo là gì?

- A. Giữ nguyên vì con số nghe hợp lý
- B. Xóa hết mọi con số trong báo cáo
- C. Hỏi lại Claude "Bạn có chắc không?" và tin vào câu trả lời
- D. Tìm và đối chiếu nguồn gốc của nghiên cứu; nếu không xác minh được thì loại bỏ hoặc ghi rõ là chưa xác minh

<details><summary>Xem đáp án</summary>

**D.** Trích dẫn cụ thể (tên tổ chức, năm, con số) mà không có nguồn đầu vào là dấu hiệu điển hình của hallucination, vì vậy cần xác minh bằng nguồn bên ngoài. Hỏi lại Claude (C) không phải là cách kiểm chứng độc lập. Xóa hết số liệu (B) là phản ứng quá mức.
</details>

### Câu 2
Dấu hiệu nào **khó phát hiện nhất** khi đánh giá đầu ra của AI?

- A. Câu trả lời bị cắt giữa chừng
- B. Câu trả lời trôi chảy, đúng định dạng, giọng văn tự tin nhưng có một chi tiết sai
- C. Câu trả lời sai chính tả
- D. Câu trả lời từ chối thực hiện

<details><summary>Xem đáp án</summary>

**B.** Đây là "silent failure": đầu ra trông chuyên nghiệp nên người đọc dễ tin mà không kiểm tra. Văn phong trôi chảy và tự tin không chứng minh nội dung đúng.
</details>

### Câu 3
Công ty dùng Claude soạn câu trả lời cho khách hàng về chính sách hoàn tiền. Mức độ kiểm duyệt nào phù hợp nhất?

- A. Chỉ cho Claude trả lời dựa trên tài liệu chính sách chính thức, và có người duyệt các trường hợp ngoại lệ hoặc nhạy cảm trước khi gửi
- B. Gửi thẳng mọi câu trả lời vì Claude rất chính xác
- C. Không dùng AI cho CSKH
- D. Chỉ kiểm tra chính tả trước khi gửi

<details><summary>Xem đáp án</summary>

**A.** Đáp án này kết hợp grounding (dựa trên nguồn chính thức) với human-in-the-loop ở các điểm rủi ro. Gửi thẳng không kiểm soát (B) rủi ro cao. Không dùng AI (C) bỏ lỡ lợi ích một cách không cần thiết.
</details>

### Câu 4
Trường hợp nào **bắt buộc nhất** phải có chuyên gia con người duyệt đầu ra của Claude?

- A. Gợi ý tiêu đề cho bài đăng blog nội bộ
- B. Tóm tắt biên bản họp nhóm
- C. Tư vấn liều dùng thuốc gửi trực tiếp cho bệnh nhân
- D. Viết lại email cho lịch sự hơn

<details><summary>Xem đáp án</summary>

**C.** Nội dung y tế, pháp lý, tài chính có ảnh hưởng trực tiếp đến con người là rủi ro cao, nên bắt buộc có chuyên gia duyệt. Các lựa chọn còn lại rủi ro thấp.
</details>

### Câu 5
Bạn cần Claude trả lời câu hỏi từ bộ tài liệu nội bộ và muốn dễ kiểm chứng. Kỹ thuật nào hiệu quả nhất?

- A. Yêu cầu câu trả lời ngắn gọn
- B. Yêu cầu Claude trích dẫn nguyên văn đoạn tài liệu hỗ trợ cho mỗi khẳng định
- C. Yêu cầu Claude trả lời bằng tiếng Anh
- D. Yêu cầu Claude tự chấm điểm độ tự tin từ 1 đến 10

<details><summary>Xem đáp án</summary>

**B.** Trích dẫn nguyên văn giúp người đọc đối chiếu nhanh với tài liệu gốc, và cũng làm giảm khả năng Claude bịa ra thông tin. Điểm tự tin do Claude tự chấm (D) không phải là bằng chứng.
</details>

### Câu 6
Claude tóm tắt một báo cáo tài chính 50 trang. Cách kiểm tra **độ đầy đủ** hợp lý nhất là gì?

- A. Đếm số từ của bản tóm tắt
- B. Hỏi Claude "Bản tóm tắt đã đầy đủ chưa?"
- C. Đọc lướt bản tóm tắt, thấy hợp lý là được
- D. Lập trước danh sách các điểm bắt buộc phải có (doanh thu, lợi nhuận, rủi ro chính…) rồi đối chiếu bản tóm tắt với danh sách này

<details><summary>Xem đáp án</summary>

**D.** Một checklist tiêu chí định trước giúp đánh giá khách quan và lặp lại được. Số từ (A) không phản ánh nội dung. Đọc lướt (C) dễ bỏ sót.
</details>

### Câu 7
Claude được yêu cầu "cộng tổng doanh thu 12 tháng" từ một bảng dữ liệu và đưa ra con số cuối. Cách kiểm chứng phù hợp là gì?

- A. Kiểm tra lại bằng công cụ tính toán (Excel, code) hoặc yêu cầu Claude trình bày từng bước để đối chiếu
- B. Tin vì máy tính luôn tính đúng
- C. So sánh với con số của năm trước
- D. Hỏi đồng nghiệp xem con số có hợp lý không

<details><summary>Xem đáp án</summary>

**A.** Mô hình ngôn ngữ có thể sai khi tính toán thủ công trong văn bản, nên số liệu cần được kiểm tra bằng công cụ xác định hoặc phép tính có thể đối chiếu. Claude không phải "máy tính" (B sai).
</details>

### Câu 8
Một nhóm HR dùng Claude sàng lọc CV và nhận thấy ứng viên nữ bị xếp hạng thấp hơn một cách có hệ thống. Đây là vấn đề gì và nên xử lý thế nào?

- A. Lỗi định dạng, nên chuyển CV sang PDF
- B. Không phải vấn đề vì AI khách quan
- C. Thiên lệch (bias); cần dừng dùng kết quả để ra quyết định, rà soát tiêu chí và prompt, kiểm tra trên mẫu cân bằng, và giữ con người ra quyết định cuối
- D. Do model quá nhỏ, nên đổi sang model lớn hơn là xong

<details><summary>Xem đáp án</summary>

**C.** Đây là dấu hiệu bias, cần đánh giá có hệ thống và có người giám sát, đặc biệt với quyết định ảnh hưởng đến con người như tuyển dụng. AI không tự động khách quan (B sai). Đổi model (D) không đảm bảo hết bias.
</details>

### Câu 9
Đâu là chỉ dẫn tốt nhất để Claude **không bịa** khi thông tin không có trong tài liệu?

- A. "Nếu tài liệu không chứa thông tin, hãy trả lời: 'Không tìm thấy trong tài liệu được cung cấp.'"
- B. "Hãy luôn đưa ra câu trả lời đầy đủ nhất có thể."
- C. "Đừng bao giờ nói không biết."
- D. "Hãy suy đoán hợp lý nếu cần."

<details><summary>Xem đáp án</summary>

**A.** Cho phép (và hướng dẫn cụ thể) cách nói "không biết" là kỹ thuật cơ bản để giảm hallucination. Các đáp án B, C, D đều đẩy Claude về phía bịa thông tin.
</details>

### Câu 10
Bạn đang so sánh 2 phiên bản prompt cho tác vụ viết mô tả sản phẩm. Cách đánh giá đáng tin cậy nhất là gì?

- A. Thử mỗi prompt 1 lần, chọn bản mình thích hơn
- B. Chọn prompt dài hơn
- C. Hỏi Claude prompt nào tốt hơn
- D. Chạy cả hai prompt trên cùng một bộ đầu vào đa dạng, chấm theo các tiêu chí định trước (đúng thông tin, giọng văn thương hiệu, độ dài)

<details><summary>Xem đáp án</summary>

**D.** Đánh giá tốt cần một bộ dữ liệu thử đại diện và tiêu chí rõ ràng. Thử 1 lần (A) không đủ để kết luận vì đầu ra có thể khác nhau giữa các lần chạy.
</details>

### Câu 11
Claude đưa ra một đoạn code và khẳng định "đã kiểm thử, chạy đúng". Bạn nên hiểu thế nào?

- A. Code chắc chắn chạy đúng
- B. Cần tự chạy kiểm thử thực tế (hoặc xem bằng chứng chạy thật) trước khi đưa vào sản phẩm
- C. Code chắc chắn sai
- D. Chỉ cần đọc lướt code là đủ

<details><summary>Xem đáp án</summary>

**B.** Một lời khẳng định không phải là bằng chứng. Cần xác minh bằng cách chạy test thật. Không nên mặc định code đúng (A) hay sai (C).
</details>

### Câu 12
Bộ phận pháp chế dùng Claude rà soát hợp đồng. Claude nêu ra 5 điều khoản rủi ro. Kết luận nào **đúng**?

- A. Hợp đồng chỉ có đúng 5 rủi ro đó
- B. Có thể ký ngay sau khi sửa 5 điều khoản đó
- C. Danh sách là điểm khởi đầu hữu ích, nhưng luật sư vẫn phải rà soát toàn bộ vì Claude có thể bỏ sót hoặc đánh giá chưa đúng
- D. Claude sai vì hợp đồng nào cũng có rủi ro

<details><summary>Xem đáp án</summary>

**C.** Đầu ra của AI hỗ trợ con người chứ không thay thế trách nhiệm chuyên môn. Việc Claude không nêu một rủi ro không có nghĩa là rủi ro đó không tồn tại (A sai).
</details>

### Câu 13
Bạn muốn giảm thời gian kiểm tra thủ công khi Claude xử lý 1.000 tài liệu mỗi ngày mà vẫn đảm bảo chất lượng. Cách tiếp cận hợp lý nhất là gì?

- A. Kiểm tra thủ công toàn bộ 1.000 tài liệu
- B. Bỏ hẳn bước kiểm tra
- C. Chỉ kiểm tra các tài liệu ngắn
- D. Kết hợp kiểm tra tự động (định dạng, trường bắt buộc), lấy mẫu ngẫu nhiên để người kiểm tra, và chuyển các trường hợp bất thường sang người duyệt

<details><summary>Xem đáp án</summary>

**D.** Kiểm tra theo tầng (tự động, lấy mẫu, xử lý ngoại lệ) cân bằng giữa chi phí và chất lượng. Kiểm tra 100% (A) không mở rộng được. Bỏ kiểm tra (B) rủi ro cao.
</details>

### Câu 14
Claude dịch một tài liệu kỹ thuật sang tiếng Việt. Cách kiểm tra chất lượng **tốt nhất** là gì?

- A. Nhờ người thông thạo cả hai ngôn ngữ và lĩnh vực kỹ thuật đọc soát, kiểm tra đặc biệt thuật ngữ chuyên ngành và số liệu
- B. Đếm số đoạn có khớp với bản gốc không
- C. Dùng một công cụ khác dịch ngược lại và xem có "giống giống" không
- D. Đọc bản tiếng Việt, thấy trôi chảy là đạt

<details><summary>Xem đáp án</summary>

**A.** Bản dịch trôi chảy (D) vẫn có thể sai thuật ngữ hoặc nghĩa. Người có chuyên môn ở cả hai ngôn ngữ và lĩnh vực là cách kiểm chứng đáng tin nhất. Dịch ngược (C) chỉ là phép thử bổ sung, không đủ để kết luận.
</details>

### Câu 15
Sau khi triển khai, người dùng phản ánh Claude thỉnh thoảng trả lời sai giờ mở cửa của các chi nhánh. Nguyên nhân khả dĩ nhất và cách xử lý là gì?

- A. Claude bị lỗi phần cứng; khởi động lại
- B. Thông tin không được cung cấp, hoặc tài liệu nguồn đã cũ; cần cập nhật nguồn dữ liệu chính thức, yêu cầu Claude chỉ trả lời từ nguồn đó và theo dõi phản hồi định kỳ
- C. Người dùng hỏi sai cách; không cần xử lý
- D. Tăng độ dài câu trả lời

<details><summary>Xem đáp án</summary>

**B.** Thông tin thực tế, hay thay đổi cần được lấy từ nguồn được cập nhật (grounding) và giám sát sau triển khai. Câu này kết hợp Domain 1 với Domain 6 (Knowledge) và Domain 7 (Troubleshooting).
</details>

---

## Chấm điểm
- 13–15: Vững
- 10–12: Ôn lại các câu sai, đọc lại [ghi chú Domain 1](../01-domains/01-output-evaluation.md)
- < 10: Làm BT2 (bắt hallucination) trong [danh sách bài tập](../02-bai-tap/danh-sach-bai-tap.md), rồi làm lại đề sau 2 ngày

Ghi các câu sai vào [ket-qua.md](ket-qua.md).
