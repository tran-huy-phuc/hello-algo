# Đánh giá Hiệu suất Giải thuật

Trong thiết kế giải thuật, chúng ta theo đuổi hai cấp độ mục tiêu sau theo thứ tự:

1. **Tìm ra giải pháp cho bài toán**: Giải thuật phải thu được giải pháp đúng đắn một cách đáng tin cậy trong phạm vi đầu vào đã xác định.
2. **Tìm kiếm giải pháp tối ưu**: Có thể tồn tại nhiều giải pháp cho cùng một bài toán, và chúng ta hy vọng tìm ra một giải thuật hiệu quả nhất có thể.

Nói cách khác, với điều kiện tiên quyết là có thể giải quyết được bài toán, hiệu suất của giải thuật đã trở thành tiêu chí đánh giá chính để đo lường chất lượng của giải thuật. Tiêu chí này bao gồm hai chiều kích sau.

- **Hiệu suất thời gian**: Khoảng thời gian mà giải thuật cần để chạy.
- **Hiệu suất không gian**: Dung lượng bộ nhớ mà giải thuật chiếm dụng.

Tóm lại, **mục tiêu của chúng ta là thiết kế các cấu trúc dữ liệu và giải thuật "vừa nhanh vừa tiết kiệm bộ nhớ"**. Đánh giá hiệu quả hiệu suất của giải thuật là rất quan trọng, vì chỉ như vậy chúng ta mới có thể so sánh các giải thuật khác nhau và định hướng quá trình thiết kế và tối ưu hóa giải thuật.

Các phương pháp đánh giá hiệu suất chủ yếu được chia thành hai loại: kiểm thử thực tế và ước tính lý thuyết.

## Kiểm thử Thực tế

Giả sử chúng ta hiện có giải thuật `A` và giải thuật `B`, cả hai đều có thể giải quyết cùng một bài toán, và chúng ta cần so sánh hiệu suất của chúng. Phương pháp trực tiếp nhất là chạy chúng trên máy tính và đo thời gian chạy cùng mức sử dụng bộ nhớ. Cách tiếp cận đánh giá này có thể phản ánh hành vi trong thế giới thực, nhưng nó cũng có những hạn chế đáng kể.

Một mặt, **thật khó để loại bỏ các yếu tố nhiễu từ môi trường kiểm thử**. Cấu hình phần cứng ảnh hưởng đến hiệu suất giải thuật. Ví dụ, nếu một giải thuật có mức độ song song hóa cao, nó phù hợp hơn để chạy trên các CPU đa nhân; nếu một giải thuật thực hiện các thao tác tốn nhiều bộ nhớ, nó sẽ được hưởng lợi nhiều hơn từ bộ nhớ hiệu suất cao. Nói cách khác, kết quả kiểm thử của một giải thuật trên các máy khác nhau có thể không nhất quán. Điều này có nghĩa là chúng ta cần kiểm thử trên nhiều máy khác nhau và tính toán hiệu suất trung bình, điều này không khả thi.

Mặt khác, **tiến hành kiểm thử hoàn chỉnh rất tốn kém tài nguyên**. Khi khối lượng dữ liệu đầu vào thay đổi, giải thuật sẽ thể hiện các hiệu suất khác nhau. Ví dụ, khi khối lượng dữ liệu đầu vào nhỏ, thời gian chạy của giải thuật `A` ngắn hơn giải thuật `B`; nhưng khi khối lượng dữ liệu đầu vào lớn, kết quả kiểm thử có thể ngược lại. Do đó, để có được những kết luận thuyết phục, chúng ta cần kiểm thử dữ liệu đầu vào ở nhiều quy mô khác nhau, điều này đòi hỏi một lượng lớn tài nguyên tính toán.

## Ước tính Lý thuyết

Vì kiểm thử thực tế có những hạn chế đáng kể, chúng ta có thể xem xét đánh giá hiệu suất giải thuật thông qua tính toán lý thuyết. Phương pháp ước tính này được gọi là <u>phân tích độ phức tạp tiệm cận</u>, hay gọi tắt là <u>phân tích độ phức tạp</u>.

Phân tích độ phức tạp có thể phản ánh mối quan hệ giữa các tài nguyên thời gian và không gian cần thiết để thực thi giải thuật với quy mô dữ liệu đầu vào. **Nó mô tả xu hướng tăng trưởng của thời gian và không gian cần thiết để thực thi giải thuật khi quy mô dữ liệu đầu vào tăng lên**. Định nghĩa này có phần dài dòng, vì vậy chúng ta có thể phân tích nó thành ba điểm chính để hiểu.

- "Tài nguyên thời gian và không gian" tương ứng lần lượt với <u>độ phức tạp thời gian</u> và <u>độ phức tạp không gian</u>.
- "Khi quy mô dữ liệu đầu vào tăng lên" có nghĩa là độ phức tạp phản ánh mối quan hệ giữa hiệu suất chạy của giải thuật và quy mô dữ liệu đầu vào.
- "Xu hướng tăng trưởng của thời gian và không gian" chỉ ra rằng phân tích độ phức tạp không tập trung vào các giá trị cụ thể của thời gian chạy hoặc không gian bị chiếm dụng, mà là thời gian hoặc không gian tăng trưởng "nhanh" như thế nào.

**Phân tích độ phức tạp khắc phục những nhược điểm của phương pháp kiểm thử thực tế**, được phản ánh ở các khía cạnh sau.

- Nó không cần thực sự chạy code, giúp tiết kiệm năng lượng và thân thiện với môi trường hơn.
- Nó độc lập với môi trường kiểm thử, và kết quả phân tích áp dụng được cho tất cả các nền tảng chạy.
- Nó có thể phản ánh hiệu suất giải thuật ở các khối lượng dữ liệu khác nhau, đặc biệt là hiệu suất giải thuật ở khối lượng dữ liệu lớn.

!!! tip

    Nếu bạn vẫn còn mơ hồ về khái niệm độ phức tạp, đừng lo lắng — chúng ta sẽ giới thiệu nó chi tiết trong các chương tiếp theo.

Phân tích độ phức tạp cung cấp cho chúng ta một "thước đo" để đánh giá hiệu suất giải thuật, cho phép chúng ta đo lường các tài nguyên thời gian và không gian cần thiết để thực thi một giải thuật nhất định và so sánh hiệu suất giữa các giải thuật khác nhau.

Độ phức tạp là một khái niệm toán học có thể cảm thấy trừu tượng và đầy thử thách đối với người mới bắt đầu. Từ quan điểm này, phân tích độ phức tạp có thể không phải là chủ đề phù hợp nhất để giới thiệu đầu tiên. Tuy nhiên, khi chúng ta thảo luận về các đặc điểm của một cấu trúc dữ liệu hoặc giải thuật nhất định, thật khó để tránh phân tích tốc độ chạy và mức sử dụng không gian của nó.

Tóm lại, trước khi đi sâu vào cấu trúc dữ liệu và giải thuật, bạn được khuyến nghị **hãy đầu tiên thiết lập sự hiểu biết cơ bản về phân tích độ phức tạp để bạn có thể phân tích độ phức tạp của các giải thuật đơn giản**.
