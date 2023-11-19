# dhmt-tetris-gk
Tổ chức code
-----------------

Lớp Piece đại diện cho một khối trò chơi ("tetrimino"), nó xác định cách một khối có thể quay và loại bỏ các chướng ngại vật.

Lớp Board đại diện cho trạng thái hình học của bảng. Nó lưu trữ các ô đã được fill, vị trí của khối hình hiện tại và xử lý các chuyển động cần thiết tuân theo ràng buộc hình học. Lớp Tetris hoạt động trên Board và xác định thời gian trò chơi, xử lý input đầu vào và điểm số.

Các hàm vẽ được triển khai trong render.cpp. Nó xác định một số lớp tiện ích để vẽ bảng, khối và text bằng cách sử dụng các shader OpenGL đơn giản.

File utility.cpp chứa các lớp đại diện cho shader, texture và glyph của font. Cũng như các hàm để tải texture và font từ tệp.

Việc khởi tạo trò chơi và vòng lặp chính được triển khai trong file game.cpp.

Building
--------
Chạy solution trong folder vs với visual studio 2017/2022.
