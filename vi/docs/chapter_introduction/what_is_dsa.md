# Giải thuật là gì

## Định nghĩa Giải thuật

Một <u>giải thuật</u> (thuật toán) là một tập hợp các chỉ dẫn hoặc các bước vận hành để giải quyết một bài toán cụ thể trong một khoảng thời gian hữu hạn. Nó có các đặc điểm sau.

- Bài toán được xác định rõ ràng, với định nghĩa đầu vào (input) và đầu ra (output) rõ ràng.
- Có tính khả thi và có thể hoàn thành trong số bước, thời gian và bộ nhớ hữu hạn.
- Mỗi bước có một ý nghĩa xác định, và dưới cùng một đầu vào cũng như điều kiện vận hành, đầu ra thu được luôn luôn giống nhau.

## Định nghĩa Cấu trúc Dữ liệu

Một <u>cấu trúc dữ liệu</u> là một cách tổ chức và lưu trữ dữ liệu, bao gồm chính các dữ liệu đó, mối quan hệ giữa các phần tử dữ liệu và các phương pháp được sử dụng để thao tác trên chúng. Nó có các mục tiêu thiết kế sau.

- Chiếm càng ít dung lượng càng tốt để tiết kiệm bộ nhớ máy tính.
- Các thao tác dữ liệu phải nhanh nhất có thể, bao gồm truy cập dữ liệu, thêm, xóa, cập nhật, v.v.
- Cung cấp một biểu diễn dữ liệu ngắn gọn và thông tin logic rõ ràng để các thuật toán có thể chạy hiệu quả.

**Thiết kế cấu trúc dữ liệu là một quá trình đầy rẫy sự đánh đổi (trade-off)**. Nếu chúng ta muốn đạt được sự cải thiện ở một khía cạnh này, chúng ta thường phải chấp nhận sự thỏa hiệp ở một khía cạnh khác. Dưới đây là hai ví dụ.

- So với mảng, danh sách liên kết thuận tiện hơn cho các thao tác thêm và xóa dữ liệu nhưng phải hy sinh tốc độ truy cập ngẫu nhiên dữ liệu.
- So với danh sách liên kết, đồ thị cung cấp thông tin logic phong phú hơn nhưng yêu cầu không gian bộ nhớ lớn hơn.

## Mối quan hệ giữa Cấu trúc Dữ liệu và Giải thuật

Như được thể hiện trong hình dưới đây, cấu trúc dữ liệu và giải thuật có liên quan chặt chẽ và gắn kết chặt chẽ với nhau, thể hiện cụ thể ở ba khía cạnh sau.

- Cấu trúc dữ liệu là nền tảng của giải thuật. Cấu trúc dữ liệu cung cấp cho giải thuật cách lưu trữ dữ liệu có cấu trúc và các phương pháp để thao tác trên dữ liệu.
- Giải thuật thổi hồn vào cấu trúc dữ liệu. Bản thân cấu trúc dữ liệu chỉ lưu trữ thông tin dữ liệu; khi kết hợp với giải thuật, chúng mới có thể giải quyết các bài toán cụ thể.
- Một giải thuật thường có thể được triển khai dựa trên các cấu trúc dữ liệu khác nhau, nhưng hiệu suất thực thi có thể khác biệt rất lớn. Việc lựa chọn cấu trúc dữ liệu phù hợp là yếu tố then chốt.

![Mối quan hệ giữa cấu trúc dữ liệu và giải thuật](what_is_dsa.assets/relationship_between_data_structure_and_algorithm.png)

Cấu trúc dữ liệu và giải thuật giống như việc lắp ráp các khối hình Lego như hình minh họa bên dưới. Một bộ khối hình lắp ráp, ngoài việc chứa nhiều chi tiết, còn đi kèm hướng dẫn lắp ráp chi tiết. Bằng cách làm theo hướng dẫn từng bước, chúng ta có thể lắp ráp thành một mô hình hoàn chỉnh và tinh tế.

![Lắp ráp khối hình](what_is_dsa.assets/assembling_blocks.png)

Sự tương đồng chi tiết giữa hai bên được thể hiện trong bảng dưới đây.

<p align="center"> Bảng <id> &nbsp; So sánh cấu trúc dữ liệu và giải thuật với việc lắp ráp khối hình Lego </p>

| Cấu trúc dữ liệu và giải thuật | Lắp ráp khối hình Lego |
| ------------------------------ | ------------------------------------------------------------------ |
| Dữ liệu đầu vào | Các chi tiết khối hình chưa lắp ráp |
| Cấu trúc dữ liệu | Hình thức tổ chức các khối hình, bao gồm hình dạng, kích thước, phương thức kết nối, v.v. |
| Giải thuật | Một loạt các bước vận hành để lắp ráp các mảnh ghép thành hình dạng mục tiêu |
| Dữ liệu đầu ra | Mô hình khối hình hoàn chỉnh |

Đáng chú ý là cấu trúc dữ liệu và giải thuật độc lập với các ngôn ngữ lập trình. Đó là lý do tại sao cuốn sách này có thể cung cấp các triển khai bằng nhiều ngôn ngữ lập trình khác nhau.

!!! tip "Chữ viết tắt thông dụng"

    Trong các cuộc thảo luận thực tế, chúng ta thường viết tắt cụm từ "cấu trúc dữ liệu và giải thuật" thành "giải thuật" (hoặc thuật toán). Ví dụ, các bài toán thuật toán nổi tiếng trên LeetCode thực chất là kiểm tra kiến thức về cả cấu trúc dữ liệu lẫn thuật toán.
