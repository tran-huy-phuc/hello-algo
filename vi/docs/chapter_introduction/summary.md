# Tóm tắt

### Điểm lại kiến thức trọng tâm

- Giải thuật có mặt khắp nơi trong cuộc sống hàng ngày và không phải là một lĩnh vực kiến thức xa vời, bí ẩn. Trên thực tế, chúng ta đã vô thức học được nhiều giải thuật và sử dụng chúng để giải quyết các vấn đề lớn nhỏ trong cuộc sống.
- Nguyên lý tra cứu từ điển nhất quán với thuật toán tìm kiếm nhị phân. Tìm kiếm nhị phân thể hiện tư tưởng thuật toán quan trọng: chia để trị.
- Quy trình sắp xếp quân bài rất giống với thuật toán sắp xếp chèn. Sắp xếp chèn thích hợp để sắp xếp các tập dữ liệu nhỏ.
- Các bước thối tiền thừa về bản chất là một giải thuật tham lam, trong đó lựa chọn tốt nhất được đưa ra ở mỗi bước dựa trên tình huống hiện tại.
- Một giải thuật là một tập hợp các chỉ dẫn hoặc các bước vận hành để giải quyết một bài toán cụ thể trong một khoảng thời gian hữu hạn, trong khi cấu trúc dữ liệu là một cách tổ chức và lưu trữ dữ liệu trong máy tính.
- Cấu trúc dữ liệu và giải thuật có mối liên hệ chặt chẽ. Cấu trúc dữ liệu là nền tảng của giải thuật, và giải thuật thổi hồn vào cấu trúc dữ liệu.
- Chúng ta có thể so sánh cấu trúc dữ liệu và giải thuật với việc lắp ráp các khối hình Lego. Các khối đại diện cho dữ liệu, cách chúng được định hình và kết nối đại diện cho cấu trúc dữ liệu, và các bước để lắp ráp chúng tương ứng với giải thuật.

### Hỏi & Đáp

**H**: Là một lập trình viên, tôi chưa bao giờ sử dụng giải thuật để giải quyết các vấn đề trong công việc hàng ngày. Các giải thuật phổ biến đã được đóng gói sẵn bởi các ngôn ngữ lập trình và có thể sử dụng trực tiếp. Điều này có nghĩa là các bài toán trong công việc của chúng tôi chưa đến mức độ cần dùng đến giải thuật?

Nếu chúng ta so sánh các kỹ năng nghề nghiệp cụ thể với "chiêu thức" trong võ thuật, thì các môn học nền tảng nên được coi là "nội công" hơn.

Tôi tin rằng ý nghĩa của việc học giải thuật (và các môn học nền tảng khác) không phải là bạn sẽ cần triển khai chúng từ đầu trong công việc, mà là kiến thức bạn đạt được sẽ giúp bạn đưa ra các phán xét nghề nghiệp đúng đắn khi giải quyết vấn đề, từ đó cải thiện chất lượng tổng thể của công việc. Đây là một ví dụ đơn giản. Mọi ngôn ngữ lập trình đều có hàm sắp xếp được tích hợp sẵn:

- Nếu chúng ta chưa nghiên cứu về cấu trúc dữ liệu và giải thuật, chúng ta có thể chỉ đơn giản truyền bất kỳ dữ liệu nào được cung cấp vào hàm sắp xếp này. Nó chạy suôn sẻ với hiệu suất tốt và có vẻ không có vấn đề gì.
- Nhưng nếu chúng ta đã nghiên cứu về giải thuật, chúng ta sẽ biết rằng độ phức tạp thời gian của hàm sắp xếp tích hợp sẵn là $O(n \log n)$. Tuy nhiên, nếu dữ liệu cho sẵn là các số nguyên có số chữ số cố định (như mã số sinh viên), chúng ta có thể sử dụng "sắp xếp theo cơ số" (radix sort) hiệu quả hơn, giảm độ phức tạp thời gian xuống còn $O(nk)$, trong đó $k$ là số chữ số. Khi khối lượng dữ liệu rất lớn, thời gian chạy tiết kiệm được có thể tạo ra giá trị đáng kể (chi phí giảm, trải nghiệm cải thiện, v.v.).

Trong thực tế kỹ thuật, nhiều bài toán khó giải quyết một cách tối ưu, và nhiều bài toán khác chỉ được giải quyết "đủ tốt". Độ khó của bài toán phụ thuộc, một mặt vào bản chất của chính vấn đề và mặt khác vào kiến thức của người nghiên cứu nó. Kiến thức của một người càng đầy đủ và kinh nghiệm càng phong phú, phân tích của họ sẽ càng sâu sắc và bài toán có thể được giải quyết một cách thanh lịch hơn.
