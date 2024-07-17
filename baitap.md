1. Bạn hiểu backend\server hoạt động như thế nào?  
   -Back-end là hậu trường phía sau, xử lý dữ liệu, tương tác với database, xử lý yêu cầu HTTP.  
   -Khi client gửi yêu cầu tới sever, sever xử lý yêu cầu và trả về kết quả tương ứng.  
   -Trong Backend có 3 thành phần quan trong việc liên quan đến lưu trữ thông tin người dùng trong phiên làm việc nhất định.  
     +cookie: là thông tin từ sever gửi đến client và thông tin đó lưu trữ ở máy client. ví dụ, khi ta đăng nhập shopee, sever gửi client thông tin và lưu trữ dạng cookie, những trạng thái giỏ hàng, ta xem sản phẩm nào đều được lưu vào cookie. Khi đó, nếu client có tương tác với sever thì sever dựa vào cookie có thể biết nhận dạng client đó là ai.  
     +Session: như vùng lưu trữ tạm thông tin của client. Ví dụ trong nhà hàng, đối với những khác hàng quen thuộc thường hay ghé qua, thì tiếp tân, người phục vụ có thể biết họ là ai mà ko cần nhìn vào sổ ghi chép thông tin. Điều này có thể tiết kiệm thời gian để tra cứu, nhận dạng người gửi yêu cầu đến sever qua database.  
     +database: Là nơi lưu trữ thông tin người dùng, như 1 cuốn sổ ghi chép.  
  
2. Bạn hiểu http protocol là gì?  
   +là 1 giao thức truyền tải dữ liệu giữa client/sever.  
   +1 trong loại giao thức đó là stateless, đó là những yêu cầu là độc lập với yêu cầu trước đó và sau khi thực hiện yêu cầu thì ko lưu trữ nó ở bất kỳ đâu.  
   +có 3 thành phần chính trong sự tương tác giữa client/sever:  
     1. General: nó lưu trữ địa chỉ web, địa chỉ máy chủ, status code(trạng thái yêu cầu được gửi đi)  
     2. Response header: Kết quả trả về(chỉ có khi được phản hồi từ sever).  
     3. Request header: Nội dung gửi đi.   
3. Giải thích mô hình client - server?  
   +Đây là 1 mô hình mà đa số website đều sài.  
   +Dựa trên hoạt động và vai trò (yêu cầu và phản hồi) thì ta sẽ phân các máy ra thành 2 loại:  
     -client: máy gửi yêu cầu(yêu cầu giao diện,hình ảnh,đăng nhập).  
     -sever: máy nhận yêu cầu từ client và phản hồi tương ứng.  
   -đối với sever:  
     +để có thể xử lý những phản hồi, sever cần cài web sever, ngôn ngữ backend, database(vài trường hợp thì database sẽ được lưu trữ ở 1 máy khác).  
   
4. Giải thích server side rendering?  
   -sever side rendering là việc client gửi yêu cầu đến sever và sever phàn hội lại thành 1 HTML hoàn chỉnh, nghĩa là ko có các thẻ đính kèm các file javascript.  
  
5. Bạn hiểu API là gì?  
   -Là người trung gian giữa database và giao diện người dùng(như app ứng dụng hoặc trình duyệt).  
   -API có ích khi 1 bên sử dụng tính năng của đối tác. Ví dụ, Momo sử dụng API để có thể các hoạt động nạp thẻ điện thoại, bằng cách dùng API để có thể thêm tiền vào giá trị tiền vào tài khoản điện thoại như Mobifone.  

