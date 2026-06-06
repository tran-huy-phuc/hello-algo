---
comments: true
icon: material/rocket-launch-outline
---

# Lời nói đầu

Một vài năm trước, tôi đã chia sẻ các lời giải cho chuỗi bài toán "Sword for Offer" trên LeetCode, và nhận được sự khuyến khích cùng ủng hộ từ rất nhiều độc giả. Trong quá trình giao lưu với độc giả, câu hỏi mà tôi thường xuyên gặp nhất là "làm thế nào để bắt đầu học giải thuật". Dần dần, tôi đã nảy sinh sự quan tâm sâu sắc đối với câu hỏi này.

Lao đầu ngay vào việc giải quyết bài toán (luyện đề/刷题) dường như là phương pháp phổ biến nhất — nó đơn giản, trực tiếp và hiệu quả. Tuy nhiên, việc luyện đề cũng giống như chơi trò Dò mìn (Minesweeper): những ai có khả năng tự học tốt có thể gỡ mìn thành công từng quả một, trong khi những người chưa có đủ nền tảng vững chắc có thể sẽ kết thúc với cơ thể bầm dập và đầy thương tích, từng bước rút lui trong sự nản lòng. Việc đọc hết sách giáo khoa cũng là một cách làm phổ biến, nhưng đối với những người đang tìm việc, các luận văn tốt nghiệp, hồ sơ xin việc, và việc chuẩn bị cho các bài kiểm tra viết lẫn phỏng vấn đã ngốn hầu hết năng lượng của họ, khiến việc cày cuốc qua những cuốn sách dày cộp trở thành một thử thách đầy gian khổ.

Nếu bạn cũng đang đối mặt với những khó khăn tương tự, thì thật may mắn khi cuốn sách này đã "tìm thấy" bạn. Cuốn sách này là câu trả lời của tôi cho câu hỏi đó — cho dù nó có thể không phải là giải pháp tối ưu nhất, nhưng ít nhất nó cũng là một nỗ lực tích cực. Mặc dù chỉ riêng cuốn sách này sẽ không trực tiếp mang lại cho bạn một lời mời làm việc (job offer), nhưng nó sẽ dẫn dắt bạn đi qua "bản đồ phong cảnh" của cấu trúc dữ liệu và giải thuật, giúp bạn hiểu rõ hình dạng, kích thước và sự phân bố của các loại "mìn" khác nhau, đồng thời trang bị cho bạn các "phương pháp gỡ mìn" đa dạng. Với những kỹ năng này, tôi tin rằng bạn có thể tự tin hơn khi đối mặt với các bài toán và khi đọc các tài liệu kỹ thuật, từ đó dần dần xây dựng nên một hệ thống kiến thức hoàn chỉnh cho riêng mình.

Tôi vô cùng đồng tình với lời của Giáo sư Feynman: "Tri thức không miễn phí. Bạn phải trả giá bằng sự chú ý." Theo nghĩa này, cuốn sách này không hoàn toàn "miễn phí". Để xứng đáng với sự "chú ý" quý giá mà bạn dành cho cuốn sách này, tôi sẽ nỗ lực hết mình và dồn hết "sự chú ý" lớn nhất của mình để hoàn thành tác phẩm này.

Tôi ý thức rõ những giới hạn trong kiến thức và kinh nghiệm của mình. Mặc dù nội dung của cuốn sách này đã được tinh chỉnh qua một thời gian dài, nhưng chắc chắn vẫn còn nhiều sai sót. Tôi chân thành đón nhận mọi ý kiến đóng góp và hiệu đính từ các thầy cô giáo cùng toàn thể các bạn độc giả.

![Hello Algorithms](../assets/covers/chapter_hello_algo.jpg){ class="cover-image" }

<div style="text-align: center;">
    <h2 style="margin-top: 0.8em; margin-bottom: 0.8em;">Hello, Algorithms!</h2>
</div>

Sự ra đời của máy tính đã mang lại những thay đổi to lớn cho thế giới. Với khả năng tính toán tốc độ cao và khả năng lập trình tuyệt vời, chúng đã trở thành phương tiện lý tưởng để thực thi các thuật toán và xử lý dữ liệu. Cho dù đó là đồ họa chân thực trong trò chơi điện tử, việc ra quyết định thông minh trong lái xe tự động, các trận đấu cờ vây xuất sắc của AlphaGo hay các tương tác tự nhiên của ChatGPT, những ứng dụng này đều là những minh chứng nổi bật về hoạt động của giải thuật trên máy tính.

Trên thực tế, trước khi máy tính xuất hiện, các thuật toán và cấu trúc dữ liệu đã tồn tại ở mọi ngóc ngách trên thế giới. Các thuật toán sơ khai tương đối đơn giản, chẳng hạn như phương pháp đếm cổ xưa và quy trình chế tạo công cụ. Khi nền văn minh tiến bộ, các thuật toán dần trở nên tinh tế và phức tạp hơn. Từ sự khéo léo tỉ mỉ của các bậc thầy nghệ nhân, đến các sản phẩm công nghiệp giải phóng lực lượng sản xuất, cho đến các quy luật khoa học chi phối hoạt động của vũ trụ, đằng sau hầu hết mọi thứ bình thường hay đáng kinh ngạc đều ẩn chứa tư duy thuật toán tài tình.

Tương tự như vậy, cấu trúc dữ liệu có ở khắp mọi nơi: từ các mạng xã hội quy mô lớn đến các hệ thống tàu điện ngầm nhỏ, nhiều hệ thống có thể được mô hình hóa dưới dạng "đồ thị" (graph); từ một quốc gia đến một gia đình, các hình thức tổ chức chính của xã hội đều thể hiện đặc điểm của "cây" (tree); quần áo mùa đông giống như một "ngăn xếp" (stack), trong đó món đồ mặc vào đầu tiên là món đồ cởi ra cuối cùng; hộp đựng cầu lông giống như một "hàng đợi" (queue), với các quả cầu được đưa vào ở một đầu và lấy ra ở đầu kia; một cuốn từ điển giống như một "bảng băm" (hash table), cho phép tra cứu nhanh chóng các mục từ khóa cần tìm.

Cuốn sách này nhằm giúp độc giả hiểu được các khái niệm cốt lõi của giải thuật và cấu trúc dữ liệu thông qua các hình minh họa động rõ ràng, dễ tiếp cận và các ví dụ mã nguồn có thể chạy được, đồng thời triển khai chúng trong mã lập trình thực tế. Xây dựng trên nền tảng này, cuốn sách nỗ lực tiết lộ những biểu hiện sinh động của thuật toán trong thế giới phức tạp và giới thiệu vẻ đẹp của giải thuật. Hy vọng cuốn sách này có thể giúp ích cho bạn!
