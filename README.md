# BÀI TẬP TỔNG HỢP: HÀNH TRÌNH XỬ LÝ 1 LỖI CÀI ĐẶT THẬT

## PHẦN 1 – GOOGLING ĐÚNG CÁCH

### 1. Vì sao câu hỏi ban đầu tìm kiếm kém hiệu quả?

Câu hỏi ban đầu sử dụng ngôn ngữ nói, quá dài và không có từ khóa kỹ thuật cụ thể. Google khó xác định chính xác lỗi cần tìm nên có thể trả về nhiều kết quả không liên quan.

### 2. Bóc tách lỗi theo 3 thành phần cốt lõi

| Thành phần                  | Nội dung bóc tách                                                                             |
| --------------------------- | --------------------------------------------------------------------------------------------- |
| Tên phần mềm / Hệ điều hành | Node.js trên Windows 11                                                                       |
| Mã lỗi nguyên văn           | `'npm' is not recognized as an internal or external command, operable program or batch file.` |
| Thao tác đang làm           | Gõ lệnh `npm -v` trong Terminal của VS Code để kiểm tra phiên bản npm.                        |

### 3. Ba câu truy vấn Google tối ưu

- Dùng `site:`: `site:stackoverflow.com npm is not recognized Windows 11`
- Dùng dấu ngoặc kép: `"npm is not recognized as an internal or external command"`
- Dùng dấu `-`: `npm is not recognized Windows 11 PATH -Windows XP`

Mỗi câu sử dụng một toán tử khác nhau để tìm kiếm chính xác hơn.

## PHẦN 2 – THẨM ĐỊNH STACKOVERFLOW

### 1. So sánh câu trả lời A và B

| Tiêu chí                        | Câu trả lời A                   | Câu trả lời B                                  |
| ------------------------------- | ------------------------------- | ---------------------------------------------- |
| Vote & Tích xanh                | +186 vote, có tích xanh.        | +2 vote, không có tích xanh.                   |
| Thời gian đăng bài              | 2 năm trước, tương đối mới.     | 9 năm trước, khá cũ.                           |
| Tags khớp hệ điều hành/phần mềm | node.js, windows, npm. Phù hợp. | node.js, windows-xp. Không phù hợp Windows 11. |

### 2. Kết luận

Em chọn Câu trả lời A vì có nhiều lượt bình chọn, được chấp nhận và nội dung phù hợp với Windows.

Câu trả lời B là cái bẫy nguy hiểm vì hướng dẫn cài lại driver mạng cho Windows XP không liên quan đến lỗi npm trên Windows 11. Làm theo có thể gây mất thời gian và ảnh hưởng đến hệ thống.

### 3. Quy trình 30 giây đọc lướt

1. Kiểm tra tiêu đề câu hỏi có đúng lỗi mình gặp không.
2. Kiểm tra Tags có đúng phần mềm và hệ điều hành không.
3. Xem câu trả lời có tích xanh không.
4. Kiểm tra số lượt Vote.
5. Xem thời gian đăng bài.
6. Đọc nội dung hướng dẫn và đánh giá xem có phù hợp với trường hợp của mình không.

## PHẦN 3 – HỎI AI ĐÚNG CÁCH VÀ NHẬN DIỆN RỦI RO

### 1. Viết Prompt theo công thức 3 thành phần

**Ngữ cảnh:**

Em là sinh viên đang sử dụng laptop Windows 11 và vừa cài đặt Node.js để học lập trình web. Em sử dụng Terminal trong VS Code để kiểm tra phiên bản npm.

**Lỗi nguyên văn:**

`'npm' is not recognized as an internal or external command, operable program or batch file.`

Em đã thử thêm đường dẫn cài đặt Node.js vào biến môi trường PATH và mở lại Terminal nhưng lỗi vẫn xuất hiện.

**Yêu cầu:**

Hãy giải thích nguyên nhân có thể gây ra lỗi và hướng dẫn em cách kiểm tra, khắc phục từng bước. Ưu tiên các lệnh kiểm tra an toàn, giải thích rõ tác dụng của từng lệnh và cảnh báo nếu có thao tác nguy hiểm. Không đề xuất xóa dữ liệu hoặc file hệ thống.

### 2. Đánh giá câu trả lời của AI theo 3 nguyên tắc an toàn vàng

Câu trả lời của AI không an toàn và tuyệt đối không được làm theo.

3 Nguyên tắc An toàn Vàng khi sử dụng lệnh do AI đề xuất có thể trình bày như sau:
1. Kiểm tra độ tin cậy: Hỏi ít nhất 2 AI khác nhau xem lệnh có an toàn không, có thể gây hại gì cho máy tính không.
2. Hiểu trước khi chạy: Phải hiểu lệnh dùng để làm gì, tác động đến file hoặc hệ thống nào. Không chạy lệnh khi chưa hiểu rõ.
3. Kiểm tra rủi ro: Ưu tiên lệnh chỉ đọc thông tin, tránh các lệnh có thể xóa dữ liệu, thay đổi hệ thống hoặc yêu cầu quyền Admin khi không cần thiết.

### 3. Phản hồi và hỏi lại AI

Em sẽ hỏi lại:

"Bạn có thể giải thích vì sao lệnh xóa toàn bộ file trong System32 lại sửa được lỗi npm không? Lệnh này có nguy cơ làm hỏng Windows không? Hãy đề xuất cách kiểm tra biến PATH và vị trí cài đặt Node.js bằng các lệnh an toàn, không làm thay đổi hoặc xóa dữ liệu hệ thống."

## PHẦN 4 – VIẾT BUG REPORT CHUẨN ĐỂ NHỜ HỖ TRỢ

### 1. Tin nhắn kém

Thầy ơi, máy em bị lỗi npm rồi, thầy giúp em với ạ!

### 2. Tin nhắn chuẩn theo Bug Reporting Framework 4 bước

| Mảnh ghép        | Nội dung trong tin nhắn                                                                                                                                       |
| ---------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Context          | Em vừa cài Node.js trên laptop Windows 11 và sử dụng Terminal trong VS Code.                                                                                  |
| Expected         | Khi gõ `npm -v`, máy sẽ hiển thị phiên bản npm đã cài đặt.                                                                                                    |
| Actual           | Máy báo lỗi: `'npm' is not recognized as an internal or external command, operable program or batch file.`                                                    |
| Log & Screenshot | Em đã thử thêm đường dẫn cài đặt Node.js vào PATH và mở Terminal mới nhưng lỗi vẫn xuất hiện. Em gửi kèm ảnh chụp màn hình thông báo lỗi và kết quả kiểm tra. |

Tin nhắn hoàn chỉnh:

Em chào thầy ạ!

Em vừa cài đặt Node.js trên laptop Windows 11 để học lập trình web. Khi mở Terminal trong VS Code và nhập lệnh `npm -v`, em mong muốn máy hiển thị phiên bản npm nhưng lại nhận được thông báo:

`'npm' is not recognized as an internal or external command, operable program or batch file.`

Em đã thử thêm đường dẫn cài đặt Node.js vào biến môi trường PATH và mở lại Terminal nhưng lỗi vẫn chưa được khắc phục.

Em gửi kèm ảnh chụp màn hình lỗi để thầy tiện kiểm tra. Mong thầy hướng dẫn em cách khắc phục ạ.

Em cảm ơn thầy!

### 3. Phím tắt chụp màn hình và lưu ý bảo mật

- Phím tắt: `Windows + Shift + S` để mở công cụ chụp màn hình.
- Lưu ý bảo mật: Trước khi gửi ảnh, cần che các thông tin nhạy cảm như mật khẩu, API Key, token hoặc thông tin cá nhân.
