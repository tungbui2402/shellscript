# SHELL SCRIPT
## A. Khái niệm
### I. Shell script là gì
- Shell script là một tập hợp các lệnh được viết bằng ngôn ngữ shell (thông thường là Bourne shell hoặc các biến thể của nó như Bash) trong hệ điều hành Unix hoặc Unix-like. Một shell script có thể chứa các lệnh điều khiển hệ thống, gọi các chương trình và thực hiện các tác vụ tự động.
- Shell script thường được sử dụng để thực hiện các công việc lặp đi lặp lại, tự động hóa các tác vụ hệ thống, xử lý dữ liệu hoặc thực hiện các tác vụ phức tạp. Ví dụ, một shell script có thể được sử dụng để sao lưu dữ liệu định kỳ, xử lý tệp tin, kiểm tra sự tồn tại của các tệp tin hoặc thư mục, và thực hiện các tác vụ quản lý hệ thống khác.
- Cú pháp của shell script tương tự như viết các lệnh trong terminal. Một shell script có thể được chạy bằng cách gọi tên tập tin script từ dòng lệnh, hoặc được cấu hình để chạy tự động theo lịch trình hoặc trong các tác vụ hệ thống khác.
- Shell script có thể là một công cụ mạnh mẽ để tự động hóa các tác vụ hệ thống và giúp tiết kiệm thời gian và công sức cho người dùng.
### II. Shell script trong linux
- Shell script trong Linux là một tập tin văn bản chứa một chuỗi các lệnh và tác vụ được viết bằng ngôn ngữ shell (như Bash) và được thi hành trên môi trường dòng lệnh của hệ điều hành Linux. Shell script được sử dụng để thực hiện các tác vụ tự động, tự động hóa các công việc hằng ngày và tự động hóa quá trình quản lý hệ thống.
- Shell script trong Linux có thể chứa các lệnh điều khiển, biến, hàm, vòng lặp, câu lệnh điều kiện và xử lý dữ liệu. Một số công việc phổ biến mà shell script có thể thực hiện bao gồm:
1. Tự động hóa quá trình sao lưu dữ liệu.
2. Thực hiện các tác vụ xử lý dữ liệu, như tìm kiếm, sắp xếp, lọc và biến đổi dữ liệu.
3. Thực hiện các tác vụ hệ thống như tạo và xóa tệp tin, thư mục, kiểm tra sự tồn tại của tệp tin hoặc thư mục, đổi tên tệp tin, và nhiều hơn nữa.
4. Xử lý đầu vào từ người dùng và thực hiện các tác vụ tương ứng.
5. Gọi các chương trình khác và truyền tham số cho chúng.
6. Xử lý lỗi và ghi log các thông báo quan trọng.
- Để chạy một shell script trong Linux, bạn cần có quyền thực thi trên tập tin script đó. Bạn có thể thực thi một shell script bằng cách gọi tên tập tin script từ dòng lệnh hoặc sử dụng lệnh `./ten_tap_tin.sh` (với `ten_tap_tin.sh` là tên của tập tin script).
### III. Một số khái niệm và khả năng của shell script trong Linux:
- Shell: Shell là môi trường dòng lệnh của hệ điều hành Linux. Bash (Bourne Again SHell) là một trong những shell phổ biến nhất trong Linux.
- Shebang: Shebang là dòng đầu tiên trong một shell script và thông báo cho hệ thống biết shell nào sẽ thực thi script. Ví dụ: #!/bin/bash cho biết script sẽ được thực thi bởi Bash.
- Biến: Biến trong shell script được sử dụng để lưu trữ dữ liệu và giá trị. Các biến có thể được gán giá trị và sử dụng trong các lệnh và tác vụ. Ví dụ: name="John" và sau đó sử dụng $name để truy cập giá trị của biến.
- Lệnh điều khiển: Shell script hỗ trợ các lệnh điều khiển như if, for, while để điều khiển luồng thực thi của script dựa trên điều kiện hoặc vòng lặp.
- Tham số dòng lệnh: Shell script có thể nhận các tham số từ dòng lệnh khi được gọi và sử dụng chúng trong quá trình thực thi. Ví dụ: $1, $2,... để truy cập các tham số.
- Câu lệnh điều kiện: Các câu lệnh điều kiện như if, case được sử dụng để kiểm tra điều kiện và thực thi các lệnh tương ứng.
- Hàm: Shell script hỗ trợ định nghĩa và sử dụng các hàm. Điều này giúp tái sử dụng mã lệnh và tạo các phần tử có cấu trúc trong script.
- Xử lý tệp tin: Shell script có thể đọc, viết và xử lý tệp tin. Ví dụ: đọc nội dung tệp tin, tạo mới tệp tin, di chuyển, đổi tên hoặc xóa tệp tin.
- Lưu trữ và quản lý dữ liệu: Shell script cho phép lưu trữ và quản lý dữ liệu bằng cách sử dụng biến, tệp tin và các công cụ xử lý dữ liệu.
- Shell script cung cấp sự linh hoạt và tiện ích cho việc tự động hóa các tác vụ, quản lý hệ thống và xử lý dữ liệu trong Linux. Nó là một phần quan trọng của quản lý hệ thống và quá trình phát triển ứng dụng trong môi trường Linux.
### IV. Các loại shell 
- Trên Linux, có nhiều loại shell script khác nhau có sẵn, nhưng Bash (Bourne Again SHell) là shell phổ biến nhất và được sử dụng rộng rãi. Dưới đây là một số loại shell script phổ biến trên Linux:
1. Bash (Bourne Again SHell): Là shell mặc định trên hầu hết các phiên bản Linux. Bash kế thừa từ Bourne shell (sh) và bổ sung nhiều tính năng và cải tiến. Nó hỗ trợ nhiều cú pháp mạnh mẽ và đa dạng, và là một lựa chọn phổ biến cho việc viết shell script trên Linux.
2. Shell Bourne (sh): Là shell gốc trong hệ thống Unix và Linux. Nó cung cấp một tập hợp hạn chế các tính năng so với Bash, nhưng vẫn được sử dụng trong một số trường hợp đơn giản hoặc khi tương thích ngược với các phiên bản cũ hơn của Unix.
3. Korn shell (ksh): Là một shell mạnh mẽ và tương thích ngược với Bourne shell. Nó cung cấp nhiều tính năng mở rộng như vòng lặp, câu lệnh switch, và xử lý chuỗi phong phú hơn so với Bourne shell.
4. C shell (csh): Là một shell mà cú pháp gần với ngôn ngữ lập trình C. Nó cung cấp cú pháp dễ hiểu và các tính năng như lịch sử lệnh, tự hoàn thành và alias. Tuy nhiên, csh không phổ biến và ít được sử dụng trong các tác vụ tự động hóa.
- Ngoài các loại shell script trên, còn có nhiều shell khác như Zsh, Dash, Fish và PowerShell, nhưng chúng ít phổ biến hơn trên Linux. Mỗi loại shell có những tính năng và cú pháp riêng, tùy thuộc vào mục đích và sở thích cá nhân, người dùng có thể lựa chọn shell phù hợp để viết shell script trên Linux.
