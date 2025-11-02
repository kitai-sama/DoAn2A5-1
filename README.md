I, Tổng quan
Một thuật toán mã hóa dùng ngôn ngữ Java để viết với chức năng chủ yếu để mã hóa & giải mã văn bản người dùng, mã hóa & giải mã file và toàn bộ tệp con bên trong file đó hoặc mã hóa hình ảnh

II, Giải thích thuật toán 
A5/1 là một mật mã được phát triển vào năm 1987 để bảo vệ liên lạc thoại trong mạng di động theo tiêu chuẩn GSM. Hiện nay, nó được coi là đã bị phá vỡ 
Quá trình này bao gồm các bước sau:
1. Tạo khóa từ khóa 64 bit và giá trị khung 22 bit
2. Mã hóa tin nhắn từ 1 người dùng
3. Giải mã tin nhắn từ người dùng khác.
Luồng khóa được liên kết với văn bản rõ (XOR) tại người gửi và do đó văn bản bí mật được hình thành,
sau đó có thể được truyền đi. Cùng một luồng khóa được hình thành tại người nhận,
sau đó được liên kết với văn bản bí mật, để nhận lại văn bản rõ.

A5/1 dựa trên sự kết hợp của ba thanh ghi dịch chuyển phản hồi tuyến tính (LFSR) với xung nhịp không đều. Ba thanh ghi dịch chuyển được chỉ định như sau:

Số LFSR         	Chiều dài tính bằng bit       	Đa thức phản hồi	          Bit xung nhịp         	Bit đã khai thác
   1	                     19                      x19 + x18 + x17 + x14 + 1      	8		                13, 16, 17, 18
   2	                     22	                     x22 + 21 + 1	                    10	                20, 21
   3	                     23	                     x23 + x22 + x21 + x8 + 1	      	10                  10, 7, 20, 21, 22

   
III, Hướng Dẫn Sử Dụng 

<img width="1170" height="667" alt="image" src="https://github.com/user-attachments/assets/68044166-c57c-4a38-a057-f12a04df7580" />
SP A5/1 text 
user 1 sẽ nhập văn bản cần mã hóa vào ô text <img width="308" height="429" alt="image" src="https://github.com/user-attachments/assets/4ab1a4b8-7c90-4c55-ad52-df8126d93306" />
sau khi nhập xong thì sẽ nhập key tùy chọn là 1 dãy số tùy ý, hoặc 1 văn bản tùy ý người dùng.
tiếp đến là nhập Frame với frame là 1 số hex bất kì. Có thể dùng nút GenerateKey để tạo Frame bất kì <img width="144" height="55" alt="image" src="https://github.com/user-attachments/assets/1d7f8ef0-d883-4a0a-ae6a-24b1f0b0bd51" />
Rồi mã hóa Văn bản cho User 2 giải mã 
// Lưu ý Frame và Key Ko đc thay đổi khi mã hoặc giải mã!!!
Sp A5/1 File-Pic
Trước hết người dùng nhập Key và Frame như ở SP A5/1 text <img width="314" height="339" alt="image" src="https://github.com/user-attachments/assets/133b8654-37c0-4e33-980d-dd09de6910f4" />
Sau đó nhấn Encrypt hoặc Decrypt để mã hóa hoặc giải mã 1 file hoặc văn bản tùy chọn <img width="761" height="427" alt="image" src="https://github.com/user-attachments/assets/faa1bd8b-8f22-4e60-80d8-25926cdcf902" />
sau khi chọn được file, văn bản tùy chọn thì sẽ chọn vị trí lưu sau khi chọn file, văn bản mã hóa <img width="592" height="415" alt="image" src="https://github.com/user-attachments/assets/c0f8d2b4-fc69-406f-8b29-4627f128efc3" />
giải mã tương tự!


-END-
















