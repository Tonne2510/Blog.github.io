---
title: "Khai báo phương thức overloading trong Java"
date: 2021-04-03T22:53:58+05:30
draft: false
github_link: "https://github.com/gurusabarish/hugo-profile"
author: "Gurusabarish"
tags:
  - Emoji support
  - Sample
  - example
image: /images/over.jpg
description: ""
toc: 
---

Trong lập trình hướng đối tượng, overloading là một khái niệm quan trọng và được sử dụng rộng rãi trong ngôn ngữ lập trình Java. Nó cho phép chúng ta định nghĩa nhiều phương thức có cùng tên nhưng khác nhau về tham số, giúp tăng tính linh hoạt và tái sử dụng mã trong chương trình.

Quá tải (overloading) trong Java là gì?
Quá tải (overloading) là khả năng định nghĩa nhiều phương thức có cùng tên nhưng khác nhau về tham số trong cùng một lớp hoặc lớp con. Khi gọi đến một phương thức quá tải, trình biên dịch sẽ tự động chọn phương thức phù hợp dựa trên các tham số thực tế được cung cấp. Điều này giúp cho chương trình trở nên linh hoạt hơn, có thể thực hiện một hành động cụ thể theo nhiều cách khác nhau bằng cách thay đổi các tham số.

Overloading là một tính năng quan trọng trong lập trình hướng đối tượng, giúp cho chương trình trở nên dễ đọc và dễ hiểu hơn. Nó cũng giúp tăng tính tái sử dụng mã và tối ưu hóa hiệu suất của chương trình.

Các loại quá tải khác nhau trong Java
Java hỗ trợ hai loại quá tải chính: quá tải theo kiểu dữ liệu của tham số và quá tải theo số lượng tham số.

Quá tải theo kiểu dữ liệu của tham số
Các phương thức có cùng tên nhưng khác nhau về kiểu dữ liệu của tham số được gọi là quá tải theo kiểu dữ liệu của tham số. Ví dụ:

public class Calculator {
    public int add(int num1, int num2) {
        return num1 + num2;
    }
  
    public double add(double num1, double num2) {
        return num1 + num2;
    }
}
Xem tiếp...
Trong ví dụ trên, chúng ta có hai phương thức add có cùng tên nhưng khác nhau về kiểu dữ liệu của tham số. Phương thức đầu tiên sử dụng hai tham số kiểu int và trả về một giá trị kiểu int, trong khi phương thức thứ hai sử dụng hai tham số kiểu double và trả về một giá trị kiểu double.

Khi gọi đến phương thức add, trình biên dịch sẽ tự động chọn phương thức phù hợp dựa trên kiểu dữ liệu của các tham số được cung cấp.

Overloading theo số lượng tham số
Các phương thức có cùng tên nhưng khác nhau về số lượng tham số được gọi là quá tải theo số lượng tham số. Ví dụ:

public class Calculator {
    public int add(int num1, int num2) {
        return num1 + num2;
    }
    
    public int add(int num1, int num2, int num3) {
        return num1 + num2 + num3;
    }
}
Xem tiếp...
Trong ví dụ trên, chúng ta có hai phương thức add có cùng tên nhưng khác nhau về số lượng tham số. Phương thức đầu tiên sử dụng hai tham số và trả về một giá trị kiểu int, trong khi phương thức thứ hai sử dụng ba tham số và trả về một giá trị kiểu int.

Khi gọi đến phương thức add, trình biên dịch sẽ tự động chọn phương thức phù hợp dựa trên số lượng tham số được cung cấp.

Ứng tuyển các vị trí việc làm Java lương cao trên TopDev

Lợi ích của quá tải trong Java
Quá tải là một tính năng rất hữu ích trong lập trình Java, mang lại nhiều lợi ích cho chương trình của bạn.

Tính linh hoạt
Với quá tải, chúng ta có thể thực hiện một hành động cụ thể theo nhiều cách khác nhau bằng cách thay đổi các tham số. Ví dụ, bạn có thể có nhiều phương thức add để thực hiện phép cộng với các kiểu dữ liệu khác nhau như int, double, float,… giúp cho chương trình trở nên linh hoạt và có thể xử lý được nhiều trường hợp khác nhau.

Khả năng đọc code
Sử dụng quá tải giúp cho code trở nên dễ hiểu hơn bằng cách sử dụng các phương thức có tên giống nhau nhưng được định nghĩa cho các ngữ cảnh khác nhau. Điều này giúp cho việc đọc và hiểu code trở nên dễ dàng hơn, đặc biệt là khi chương trình có nhiều phương thức cùng tên.

Tính tái sử dụng
Quá tải cho phép tái sử dụng mã cho các trường hợp khác nhau. Thay vì phải viết nhiều phương thức có chức năng tương tự nhau nhưng khác nhau về tham số, chúng ta có thể sử dụng quá tải để tái sử dụng mã và giảm thiểu việc lặp lại code.

Tối ưu hóa hiệu suất
Với quá tải, chúng ta có thể chọn các phiên bản hiệu quả nhất của phương thức dựa trên các tham số thực tế được cung cấp. Điều này giúp cho chương trình hoạt động hiệu quả hơn và tối ưu hóa được hiệu suất của nó.

Các quy tắc của quá tải trong Java
Để các phương thức được coi là quá tải, chúng phải tuân theo một số quy tắc sau:

Các phương thức phải có cùng tên.
Các phương thức phải được định nghĩa trong cùng một lớp hoặc lớp con.
Các phương thức phải khác nhau về tham số theo một trong hai cách đã đề cập ở trên.
Giá trị trả về của các phương thức có thể khác nhau.
Khai báo phương thức overloading trong Java
Để khai báo một phương thức quá tải trong Java, chúng ta cần tuân theo các quy tắc đã đề cập ở trên. Ví dụ:

public class Calculator {
    public int add(int num1, int num2) {
        return num1 + num2;
    }
    
    public double add(double num1, double num2) {
        return num1 + num2;
    }
    
    public int add(int num1, int num2, int num3) {
        return num1 + num2 + num3;
    }
}
Xem tiếp...
Trong ví dụ trên, chúng ta có ba phương thức add được định nghĩa trong cùng một lớp Calculator, khác nhau về số lượng và kiểu dữ liệu của tham số. Điều này cho phép chúng ta có thể gọi các phương thức này với các tham số khác nhau để thực hiện phép cộng.

Ví dụ về quá tải trong Java
Để hiểu rõ hơn về quá tải trong Java, chúng ta sẽ xem xét một ví dụ đơn giản về việc tính tổng của hai số nguyên và hai số thực.

public class Calculator {
    public int add(int num1, int num2) {
        return num1 + num2;
    }
    
    public double add(double num1, double num2) {
        return num1 + num2;
    }
}
Xem tiếp...
Trong ví dụ trên, chúng ta có hai phương thức add được định nghĩa trong lớp Calculator. Phương thức đầu tiên sử dụng hai tham số kiểu int và trả về một giá trị kiểu int, trong khi phương thức thứ hai sử dụng hai tham số kiểu double và trả về một giá trị kiểu double.

Bây giờ, chúng ta có thể gọi các phương thức này với các tham số khác nhau để tính tổng của hai số nguyên và hai số thực.

public class Main {
    public static void main(String[] args) {
        Calculator calculator = new Calculator();
        
        // Tính tổng của hai số nguyên
        int sumInt = calculator.add(5, 10);
        System.out.println("Tổng của hai số nguyên là: " + sumInt);
        
        // Tính tổng của hai số thực
        double sumDouble = calculator.add(3.14, 2.71);
        System.out.println("Tổng của hai số thực là: " + sumDouble);
    }
}
Xem tiếp...
Kết quả khi chạy chương trình:

Tổng của hai số nguyên là: 15
Tổng của hai số thực là: 5.85

Như vậy, chúng ta đã sử dụng quá tải để tính tổng của hai số nguyên và hai số thực bằng cách sử dụng các phương thức có cùng tên nhưng khác nhau về kiểu dữ liệu của tham số.

Phân biệt overloading và override) trong Java
Một khái niệm khác liên quan đến quá tải là ghi đè (override). Tuy nhiên, hai khái niệm này có một số điểm khác biệt nhau:

Quá tải xảy ra khi chúng ta định nghĩa nhiều phương thức có cùng tên nhưng khác nhau về tham số trong cùng một lớp hoặc lớp con.
Ghi đè xảy ra khi chúng ta định nghĩa lại một phương thức đã được định nghĩa trong lớp cha trong lớp con.
Quá tải giúp cho chúng ta có thể thực hiện một hành động cụ thể theo nhiều cách khác nhau bằng cách thay đổi tham số của phương thức.
Ghi đè giúp cho chúng ta có thể cải thiện hoặc mở rộng chức năng của một phương thức đã được định nghĩa trong lớp cha.
  Sử dụng override trong Java sao cho hiệu quả?
Khi nào nên sử dụng quá tải trong Java?
Chúng ta nên sử dụng quá tải trong các trường hợp sau:

Các phương thức có cùng chức năng nhưng khác nhau về tham số.
Các phương thức có cùng chức năng nhưng khác nhau về kiểu dữ liệu của tham số.
Các phương thức có cùng chức năng nhưng khác nhau về số lượng tham số.
Với việc sử dụng quá tải, chúng ta có thể tái sử dụng mã và giảm thiểu việc lặp lại code, đồng thời cũng có thể tối ưu hóa hiệu suất của chương trình.

Các trường hợp không được coi là quá tải trong Java
Mặc dù có nhiều trường hợp chúng ta có thể sử dụng quá tải, tuy nhiên cũng có một số trường hợp không được coi là quá tải trong Java. Đó là khi hai phương thức có cùng tên nhưng chỉ khác nhau về kiểu trả về. Ví dụ:

public class Calculator {
    public int add(int num1, int num2) {
        return num1 + num2;
    }
    
    public double add(int num1, int num2) {
        return num1 + num2;
    }
}
Xem tiếp...
Trong ví dụ trên, hai phương thức add có cùng tên và cùng kiểu trả về là int, do đó chúng không được coi là quá tải mà sẽ gây ra lỗi biên dịch.

Những mẹo hay khi sử dụng quá tải trong Java
Tránh sử dụng quá tải quá nhiều, điều này có thể làm cho mã của chúng ta trở nên khó hiểu và khó bảo trì.
Nếu có thể, hãy sử dụng các kiểu dữ liệu nguyên thủy như int hoặc double thay vì các kiểu dữ liệu đối tượng để giảm thiểu việc sử dụng quá tải.
Khi sử dụng quá tải, hãy đặt tên cho các phương thức sao cho dễ hiểu và thể hiện được chức năng của chúng.
Hãy chắc chắn rằng các phương thức quá tải của chúng ta có cùng chức năng và chỉ khác nhau về tham số, không nên sử dụng quá tải để thực hiện các chức năng khác nhau.
Kết luận
Quá tải (overloading) là một tính năng quan trọng trong Java cho phép chúng ta định nghĩa nhiều phương thức có cùng tên nhưng khác nhau về tham số. Điều này giúp cho chúng ta có thể tái sử dụng mã và tối ưu hóa hiệu suất của chương trình. Hãy tiếp tục thường xuyên truy cập đến Blog TopDev để tham khảo thêm nhiều thông tin hữu ích về lập trình và tuyển dụng.