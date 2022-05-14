# LTM0905

Bài 1: Lập trình server chấp nhận kết nối từ các client và vào vòng lặp hỏi tên client cho đến khi client gửi đúng cú pháp “client_id: xxxxxx” trong đó xxxxxx là tên của client.
Khi client gửi đúng cú pháp thì chuyển sang vòng lặp nhận dữ liệu từ client và gửi dữ liệu đó đến các client còn lại, ví dụ: client có id “abc” gửi “xin chào” thì các client khác sẽ nhận được: “abc: xin chao”.

Bài 2: Lập trình server yêu cầu client gửi user và pass, so sánh với file cơ sở dữ liệu là một file text, mỗi dòng chứa một cặp user + pass ví dụ:
“admin admin

guest nopass

…”

+ Nếu không tìm thấy user và pass thì báo lỗi đăng nhập, yêu cầu nhập lại.
+ Nếu tìm thấy thì chuyển sang đợi lệnh từ client, thực hiện lệnh và trả kết quả cho client.
Dùng hàm system(“dir c:\temp > c:\\temp\\out.txt”) để thực hiện lệnh
+ dir c:\temp là ví dụ lệnh dir mà client gửi
+ > c:\\temp\\out.txt để định hướng kết quả lệnh dir vào file văn bản
