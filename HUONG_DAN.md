# Giao diện kết quả tìm kiếm Cocoon

Bản thực hành bổ sung ảnh và giá trong kết quả tìm kiếm. Mỗi kết quả giữ tên, dung tích và liên kết đến đúng sản phẩm chính thức. Trang có bốn kết quả mẫu cố định cho từ khóa “bí đao”.

## Cách xem

1. Giải nén nếu đang dùng gói ZIP.
2. Nhấp đúp `index.html` trong thư mục này để mở bằng trình duyệt.
3. Xem danh sách và thay đổi chiều rộng cửa sổ.
4. Bấm “Xem chi tiết” để mở sản phẩm trên Cocoon trong thẻ mới; cần Internet cho liên kết này.

Ảnh và CSS đã nằm trong dự án. Không cần cài thư viện. Ô từ khóa chỉ đọc vì đây là bản minh họa cách trình bày kết quả bằng HTML/CSS.

## Cấu trúc

- `index.html`: tiêu đề, ô từ khóa mẫu và bốn kết quả.
- `css/style.css`: màu, chữ, bố cục và cách đổi bố cục theo màn hình.
- `images/`: bốn ảnh chính thức được lưu cục bộ.
- `NGUON_ANH.md`: nguồn ảnh, trang sản phẩm và dữ liệu giá.

## Điểm thay đổi được chọn

Trong khung tìm kiếm Cocoon đã quan sát, danh sách hiển thị tên sản phẩm có liên kết nhưng chưa kèm ảnh và giá. Bản thực hành thêm hai thông tin này ngay trong kết quả. Đây là đề xuất bổ sung thông tin; chưa có phép đo với khách hàng chứng minh giao diện mới thuận tiện hơn.

Máy tính từ 900 px xếp ảnh, thông tin, giá và nút trên cùng hàng. Từ 560 đến 899 px đưa giá xuống dưới tên. Dưới 560 px đưa nút xuống dưới nội dung, rộng theo hàng; ảnh giữ bên trái.

## Kiểm tra do trợ lý AI thực hiện

Đã xem ở 1280 × 900, 768 × 1024, 375 × 812 và 320 × 740: bốn ảnh tải được, không tràn ngang, mỗi nút cao 44 px. Đã kiểm tra Tab đến liên kết đầu tiên, viền bàn phím và Enter mở đúng trang sản phẩm. Các giá trị tên, dung tích, giá và địa chỉ được đối chiếu với bốn trang Cocoon ngày 21/10/2026.

## Tự kiểm tra và ghi nhận điều chỉnh

Đề bài có bước tự phát hiện và chỉnh ít nhất một điểm. Các phép thử của trợ lý không thay thế phần này.

1. Mở trang trên máy tính và điện thoại hoặc chế độ màn hình hẹp.
2. Kiểm tra ảnh, độ rõ của tên/giá/dung tích, nút thao tác và trang đích.
3. Chọn một điểm cần sửa dựa trên điều thực sự quan sát được.
4. Ghi lại: điểm phát hiện, thay đổi đã làm, phần HTML/CSS liên quan và kết quả sau sửa.
5. Lưu ảnh trước/sau. Chỉ ghi nhận thao tác sau khi đã thực hiện.

Một số vị trí để hiểu và điều chỉnh khi có lý do: `.product-image` điều khiển khung ảnh; `h3` điều khiển tên; `.product-volume` điều khiển dung tích; `.product-price` điều khiển giá; `.product-action` điều khiển liên kết; `@media` đổi cách xếp các vùng.
