# Terminal Cheatsheet cho Mac (Căn bản)
Original translation by [toankid1412](https://github.com/toankid1412)
------------

## PHÍM TẮT

| Phím/Lệnh | Mô tả |
| ----------- | ----------- |
| Ctrl + A   | Di chuyển con trỏ đến đầu dòng. Ngoài ra tổ hợp phím này còn tác dụng với hầu hết các phương thức nhập, ngoại trừ Netbean... |
| Ctrl + E   | Di chuyển con trỏ đến cuối dòng. Ngoài ra tổ hợp phím này còn tác dụng với hầu hết các phương thức nhập, ngoại trừ Netbean... |
| Ctrl + L   | Xóa sạch màn hình. Giống với lệnh: clear |
| ⌘Cmd + K   | Xóa sạch màn hình. Giống với lệnh clear |
| Ctrl + U   | Cắt từ vị trí con trỏ chuột đến đầu dòng |
| Ctrl + K   | Cắt từ vị trí con trỏ chuột đến cuối dòng |
| Ctrl + W   | Cắt một từ ở phía trước con trỏ chuột |
| Ctrl + Y   | Dán những từ được cắt cuối cùng |
| Ctrl + H   | Xóa một kí tự trước con trỏ(Giống nút backspace) |
| Ctrl + C   | Kill tất cả mọi thứ đang chạy |
| Ctrl + D   | Thoát khỏi shell hiện tại khi không có tiến trình nào được chạy, hoặc gửi một lệnh kết thúc tới tiến trình đang chạy |
| Ctrl + Z   | Đặt bất cứ điều gì bạn đang chạy vào một tiến trình nền bị đình chỉ. |
| Ctrl + _   | Hoàn tác lệnh cuối cùng. (Dấu gạch dưới.  Là  Ctrl + Shift + -) |
| Ctrl + T   | Di chuyển kí tự trước con trỏ sang bên phải |
| Ctrl + F   | Di chuyển con trỏ về sau một ký tự |
| Ctrl + B   | Di chuyển con trỏ về trước một ký tự |
| Option + →  | Di chuyển con trỏ về sau một từ  |
| Option + ←  | Di chuyển con trỏ về trước một từ |
| Esc + T  | Di chuyển từ đằng trước con trỏ về sau một từ |
| Tab  | Tự động hiển thị tệp hoặc thư mục |

## LỆNH HỆ THỐNG

| Phím/Lệnh | Mô tả |
| ----------- | ----------- |
| cd |  Về thư mục Home |
| cd [thư mục] | Chuyển đến thư mục. Ví dụ: `cd tailieu` |
| cd /  | Đến thư mục gốc |
| cd -  | Đến thư mục trước đó |
| ls | Xem nhanh danh sách file, thư mục trong thư mục hiện tại |
| ls -l | Xem chi tiết danh sách file, thư mục trong thư mục hiện tại  |
| ls -a | Xem tất cả file, thư mục trong thư mục hiện tại kể cả file ẩn |
| ls -lh| Xem chi tiết danh sách file, thư mục trong thư mục hiện tại với kích thước file |
| ls -R | Hiển thị toàn bộ file, thư mục kể cả trong thư mục con  |
| sudo [command] | Chạy lệnh với quyền Super User  (Super User DO) |
| open [file] | Mở một file ( Giống như ta click đúp vào file đó ) |
| top | Hiển thị tiến trình đang hoạt động. Ấn phím q để thoát |
| nano [file] | Mở file để sử dụng với trình soạn thảo nano |
| vim [file] | Mở file để sử dụng với trình soạn thảo vim |
| clear |  Xóa sạch màn hình |
| reset |  Khởi chạy lại terminal |

## NỐI LỆNH

| Phím/Lệnh | Mô tả |
| ----------- | ----------- |
| [Lệnh-a]; [Lệnh-b] | Chạy lệnh A sau đó chạy lệnh B, bất chấp A có thành công hay không |
| [Lệnh-a] && [Lệnh-b] | Chạy lệnh B nếu Lệnh A thành công |
| [Lệnh-a] || [Lệnh-b] | Chạy lệnh B nếu lệnh A thất bại |
| [Lệnh-a] & | Chạy lệnh A dưới chế độ nền |


## PIPING LỆNH

| Phím/Lệnh | Mô tả |
| ----------- | ----------- |
| [Lệnh-a] \| [Lệnh-b] | Chạy lệnh A sau đó lấy kết quả để chạy lệnh B. Ví dụ: ps auxwww \| grep google
|


## LỊCH SỬ LỆNH
| Phím/Lệnh | Mô tả |
| ----------- | ----------- |
| history n |  Hiển thị lịch sử lệnh gần nhất với n là số lượng lệnh muốn xem |
| Ctrl + r  | Tương tác tìm kiếm thông qua các lệnh đã gõ trước đó |
| ![value] |  Thực hiện lệnh cuối cùng gõ bắt đầu với ‘value’ |
| !! |  Thực hiện lệnh cuối cùng |

## QUẢN LÝ FILE

| Phím/Lệnh | Mô tả |
| ----------- | ----------- |
| touch [file] |   Tạo mới file |
| pwd | Đường dẫn đầy đủ đến thư mục hiện tại |
| . |  Thư mục hiện tại, Ví dụ: `ls .` |
| .. | Thư mục cha, vd: `ls ..` |
| `ls -l ..` | Xem chi tiết danh sách file, thư mục của thư mục cha |
| `cd ../../` | Di chuyển ra ngoài 2 cấp |
| cat | Concatenate to screen |
| rm [file] |  Xóa một file, vd: `rm data.tmp` |
| rm -i [file] | Xóa với sự xác nhận |
| rm -r [dir] | Xóa một thư mục và tất cả mọi thứ bên trong nó |
| rm -f [file] | Xóa mà không cần xác nhận lại |
| cp [file] [filemoi] | Sao chép file với tên filemoi |
| cp [file] [dir] | Sao chép file tới thư mục |
| mv [file] [tenfilemoi] |  di chuyển hoặc đổi tên file, vd: `mv file1.ad /tmp` |
| pbcopy < [file] | Sao chép nội dung file tới clipboard |
| pbpaste | dán nội dung từ clipboard  |
| pbpaste > [file] | dán nội dung từ clipboard vào file, `pbpaste > paste-test.txt` |

## QUẢN LÝ THƯ MỤC

| Phím/Lệnh | Mô tả |
| ----------- | ----------- |
| mkdir [dir] | Tạo mới thư mục |
| mkdir -p [dir]/[dir] |  tạo mới nhiều thư mục |
| rmdir [dir] | Xóa thư mục (Chỉ hoạt động trên các thư mục rỗng) |
| rm -R [dir] | Xóa sạch thư mục |
| [lệnh] \| [lệnh] | Cho phép kết hợp nhiều lệnh mà tạo đầu ra, e.g. `cat data.txt | pbcopy` |
| less |  In nội dung trong khối kích thước màn hình |
| [lệnh] > [file] |  Push output to file, keep in mind it will get overwritten |
| [lệnh] >> [file] | Append output to existing file |
| [lệnh] < [file] |  Tell command to read content from a file |

## TÌM KIẾM

| Phím/Lệnh | Mô tả |
| ----------- | ----------- |
| find [dir] -name [mau_tim_kiem] | Tìm kiếm file theo mẫu, vd: `find /Users -name "file.txt"` |
| grep [mau_tim_kiem] [file] | Tìm kiếm trong tất cả các dòng của file để tim kiếm quả, e.g. `grep "Tom" file.txt` |
| grep -r [mau_tim_kiem] [file] | Recursively search for all lines that do not contain the pattern |
| grep -v [mau_tim_kiem] [file] | Search for all lines that do NOT contain the pattern |

## HELP

| Phím/Lệnh | Mô tả |
| ----------- | ----------- |
| [lệnh] -h |  Hiển thị trợ giúp |
| [lệnh] —help | Hiển thị trợ giúp |
| info [lệnh] | Hiển thị trợ giúp |
| man [lệnh] |  Hiển thị trợ giúp cho [lệnh] |
| whatis [lệnh] | Một dòng mô tả về [lệnh] |
| apropos [search-pattern] | Tìm kiếm các lệnh với từ khóa trong search-pattern |
