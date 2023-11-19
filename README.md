# dhmt-tetris-gk
Code organization
-----------------
Logic của trò chơi được triển khai trong tetris.cpp. Các quy tắc và cơ chế chính xác của trò chơi được tìm hiểu từ một số wiki về Tetris.

Lớp Piece đại diện cho một mảnh trò chơi ("tetrimino"), nó xác định cách một mảnh quay và loại bỏ các chướng ngại vật.

Lớp Board đại diện cho trạng thái hình học của bảng. Nó lưu trữ các ô đã được chiếm, vị trí của mảnh hiện tại và xử lý các chuyển động cần thiết tuân theo ràng buộc hình học. Lớp Tetris hoạt động trên Board và xác định thời gian trò chơi, xử lý đầu vào người dùng và điểm số.

Các hàm vẽ được triển khai trong render.cpp. Nó xác định một số lớp tiện ích để vẽ bảng, mảnh và văn bản bằng cách sử dụng các shader OpenGL đơn giản.

File utility.cpp chứa các lớp đại diện cho shader, texture và glyph của font. Cũng như các hàm để tải texture và font từ tệp.

Việc khởi tạo trò chơi và vòng lặp chính được triển khai trong game.cpp theo cách đơn giản nhất mà không có trừu tượng hóa nào hơn.

Building
--------
Chạy solution trong folder vs với visual studio 2017/2022.
