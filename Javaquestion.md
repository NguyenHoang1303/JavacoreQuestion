                                 Những câu hỏi Java core 

##### 1. JVM là gì?
- Java Virtual Machine (JVM) là quy trình máy ảo java biên dịch chương trình chạy sang ngôn ngữ máy.
##### 2.  Sự khác nhau JDK và JRE?
- Java Runtime Environment (JRE) là trình triển khai của Java Virtual Machine (JVM) nơi mà chương trình Java của bạn được thực thi. Nó cũng bao gồm các plugins trình duyệt để thực thi các applet.
- Java Development Kit (JDK) là công nghệ cốt lõi của Software Development Kit của Java. Nó bao gồm JRE, trình biên dịch và các công cụ như JavaDoc, Java Debugger. JDK dùng để phát triển, biên dịch và thực thi các ứng dụng Java.
##### 3. Stack và Heap?
- Bộ nhớ stack là một phần của bộ nhớ chứa method, local variable và variable tham chiếu.Bộ nhớ stack luôn được tham chiếu theo last in first out. Local variable thi được tạo trong stack.
Bộ nhớ Heap là phần bộ nhớ chưa các Object cũng có thể chưa biến tham chiếu, instance variable được tạo ở đây.
##### 4. Autoboxing và Unboxing là gì?
- Boxing là việc đưa dữ liệu nguyên thuỷ về đối tượng tương ứng của kiểu dữ liệu đó.
- Unboxing là quá trình ngược lại.
##### 5. Tại sao Java là một ngôn ngữ độc lập với nền tảng?
- Java được phát triển độc lập với phần cứng và phần mềm máy do trình biên dịch dịch mã sau đó chuyển đổi sang ngôn ngữ máy nên có thể chạy trên nhiều nền tảng khác nhau ( cần cài đặt JRE ).
##### 6. Tại sao Java không được coi là ngôn ngữ hướng đối tượng thuần tuý?
- Do Java hỗ trợ các kiểu dữ liệu nguyên thuỷ: byte, int, char, boolean, short, float, long, double.
##### 7. Instance Variable and Local Variable?
- Instance variable: là biến bên ngoài các method và bên trong class. các biến này mô tả thuộc tính của đối tượng.
- Local variable: là biến nằm trong 1 block, method, constructor và chỉ được truy cập bên trong chúng.
##### 8. Giải thích về encapsulation?
- Là khái niệm của lập trình hướng đối tượng dùng để ẩn các thuộc tính dữ liệu và các hành vi của chúng.
Giúp nhà phát triển theo modul khi phát triển phần mềm bằng cách mỗi đối tượng được độc lập với các đối tượng khác với các thuộc tính, đặc điểm, hành vi riêng của nó.
- mục đích: bảo mật , ẩn dữ liệu
##### 9. Giải thích overloading và overriding?
- Overloading là việc tạo nhiều hàm có cùng tên nhưng tuỳ vào mục đích sử dụng thì kiểu dữ liệu trả về và số lượng tham số, kiểu dữ liệu của tham số truyền vào sẽ khác nhau.
- Overriding là việc 1 phương thức từ lớp cha được định nghĩa lại ở lớp con.
##### 10. Phương thức Final là gì?
- Final không thể bị ghi đè.
##### 11. Tính chất "viết một lần chạy nhiều nơi" của java là gì?
- Java code được biên dịch thành một byte code, là ngôn ngữ trung gian giữa mã nguồn và mã máy. Byte code này không phải là nền tảng cụ thể và do đó có thể được thông dịch cho bất kỳ nền tảng nào.
##### 12. Constructor là gì?
- Constructor giống như một phương thức được sử dụng để khởi tạo trạng thái của một đối tượng. Nó được gọi ra vào thời điểm tạo ra đối tượng.
##### 13. Biến static là gì?
- Biến static có thể được sử dụng để mô tả thuộc tính chung của tất cả đối tượng (mà không là duy nhất cho mỗi đối tượng), ví dụ như tên công ty của nhân viên, tên trường học của các sinh viên, …
- Biến static được tạo ra khi chúng ta bắt đầu chạy trương trình.
##### 14. Lớp nào là lớp cha cho tất cả các lớp?
- Lớp Object
##### 15. Đa hình runtime là gì?
- Đa hình tại runtime là quá trình gọi phương thức đã được ghi đè trong thời gian thực thi chương trình. Trong quá trình này, một phương thức được ghi đè được gọi thông qua biến tham chiếu của một lớp cha.
##### 16. Có thể thực hiện đa hình lúc runtime với các thành viên dữ liệu không?
- Không.
##### 17. Trừu tượng là gì?
- Tính trừu tượng là việc ẩn đi các chi tiết của 1 đối tượng, chủ thể và chỉ hiển thị tính năng cho người dùng nhìn thấy.
- Sự trừu tượng khiến bạn tập trung vào đối tượng đó làm những gì thay vì đối tượng đó làm như thế nào.
##### 18. Sự khác nhau giữa trừu tượng và đóng gói là gì?
- Trừu tượng là ẩn đi cài đặt chi tiết còn đóng gói là gói code và data vào một khối duy nhất.
##### 19. Class abstract là gì?
- Một lớp được khai báo với từ khóa abstract là lớp trừu tượng trong Java. Cần có một lớp khác kế thừa nó và cài đặt phương thức của nó. Nó không thể là thể hiện cụ thể.
##### 20. Có thể sử dụng cả abstract và final cho một phương thức không?
- Không. Vì final không thể ghi đè còn abstract bắt buộc phải ghi đè.
##### 21. Interface là gì?
- Là 1 bản thiết kế của 1 lớp. Nó có các abstract method.
- Với interface chúng ta có thể khái quát lại toàn bộ 1 bài toàn hay 1 dự án nào đó, giúp việc code trở nên dễ dàng hơn, hạn chế việc bị thiếu hay thừa 1 chức năng nào đó.
##### 22. Có thể khai báo một phương thức của interface với từ khóa static không?
- Không. Vì mặc định các phương thức của một interface là trừu tượng, từ khóa static và abstract không thể được sử dụng chung với nhau.
##### 23. Package là gì?
- Một package (gói) trong java là một nhóm các kiểu tương tự của các lớp, giao diện và các package con.
##### 24. Có phải mỗi khối try phải đi kèm với một khối catch?
- Không. Theo sau khối Try là khối Catch và cuối cùng là Finally. Các khối phải được viết đúng tuần tự như trên.
##### 25. Khối finally là gì?
- Là khối được sử dụng để thực thi các lệnh quan trọng. Ví dụ: đóng kết nối, đóng cả stream,..Nó luôn được thực thi cho dù có xả ra ngoại lệ hay ko.Khai báo sau khối catch.
##### 26. Bạn hãy cho biết sự khác nhau giữa các process và các threads?
- Một process là một quá trình thực thi của một chương trình trong khi Thread (Luồng) là một thực thi đơn bên trong một process. Một process có thể có thể có đa luồng (multiple threads). Một Thread có thể được gọi là một Quy Trình Nhẹ (lightweight process).
##### 27. Các cách tạo Thread?
- Có ba cách để tạo Thread:
  + Cách 1: tạo luồng bằng cách kế thừa từ lớp thread
  + Cách 2: Tạo luồng bằng cách implement từ Interface Runnable
  + Cách 3: một ứng dụng có thể dụng Executor framework để tạo thread pool
##### 28. Các trạng thái của 1 luồng?
- New: Thread ở trạng thái new nếu bạn tạo một instance của lớp Thread nhưng trước khi gọi phương thức start()
- Runnable: thread sẵn sàng để thực thi nhưng không nhất thiết phải bắt đầu thực thi ngay
- Running: vi xử lý bắt đầu thực thi thread code
- Non-Runnable (Blocked): bao gồm blocked on I/O và blocked on Synchronization. Đây là trạng thái khi luồng vẫn còn tồn tại, nhưng hiện tại không đủ điều kiện để chạy.
- Terminated: kết thúc thực thi.
##### 29. Deadlock là gì?
- là một trạng thái xảy ra khi có hai processes mà process này chờ cho process kia thực thi xong trước khi tiếp tục. Kết quả là cả hai process đều chờ vô thời hạn.
##### 30. Làm thế nào để tránh deadlock trong Java?
- Tránh Nested Locks: một deadlock có thể xảy ra khi bạn cung cấp các khóa cho nhiều thread. Vì vậy cần tránh cấp khóa cho multiple threads nếu đã cấp cho một thread.
- Tránh các khóa không cần thiết: chỉ cấp khóa cho các đối tượng cần.
- Dùng Thread.join() với thời gian thực thi tối đa
##### 31. Interface cơ bản của Java Collection?
- Collection, Set, List, Queue, Map.
##### 32. Trình bày về hasCode() và equals()?
- hasCode() và equals() là hai phương thức được định nghĩa trong class Object. Mà Object lại là class cha của tất cả các class trong Java nên tất cả các object đều mặc định có hai phương thức này.
- Phương thức hashCode() trả về 1 số nguyên, chính là địa chỉ vùng nhớ mà Object đó đang được lưu
- Phương thức equals() được sử dụng để kiểm tra xem 2 object có bằng nhau hay không. Mặc định thì phương thức equals() sẽ kiểm tra xem 2 Object này có cùng tham chiếu đến một vùng nhớ hay không.Nếu có thì 2 Object này bằng nhau. Nếu không thì 2 Object này không bằng nhau.
Phương thức equals() sử dụng hashCode() để so sánh 2 Object này có cùng tham chiếu đến một vùng nhớ hay không.
