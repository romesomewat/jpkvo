SALE BRAVAT WEB - BẢN CÓ LOGO + CONTENT JSON

Cấu trúc đặt trong thư mục D:\JPK VO\SALE BRAVAT:

index.html
styles.css
script.js
data.json
content.json
README.txt
jpkvo.png
bravat.png
TOILET/
LAVABO/
PAN/
FAUCET/
SHOWER/

1. LOGO
- Đặt logo JPK VO ở file: jpkvo.png
- Đặt logo BRAVAT ở file: bravat.png
- Hai file logo nằm cùng cấp với index.html.
- Nếu muốn đổi tên file logo, sửa trong content.json tại:
  logos.jpkvo.src
  logos.bravat.src

2. CHỈNH TEXT TOÀN WEB
- Sửa file content.json.
- Các text như tiêu đề, subtitle, nhãn thống kê, tab, ô tìm kiếm, nút BACK TO TOP / TOP TO BOTTOM, footer, dòng VAT đều nằm trong content.json.
- Tên sản phẩm, mã sản phẩm, giá, kích thước nằm trong data.json.

3. CHỈNH SẢN PHẨM
- Sửa data.json.
- Mỗi sản phẩm cần có category, code, name, dimensions, originalPrice, salePrice, discountPercent, saveAmount, image.
- Đường dẫn ảnh nên để dạng: LAVABO/C22149W-1-ENG.png

4. LƯU Ý KHI MỞ TRÊN MÁY
- Nếu double click mở index.html trực tiếp, một số trình duyệt có thể không cho đọc content.json / data.json.
- Khi upload lên hosting hoặc chạy bằng VS Code Live Server, web sẽ đọc content.json và data.json bình thường.
- script.js vẫn có dữ liệu dự phòng để web không bị trắng khi mở file trực tiếp.

5. VAT
- Dòng cuối trang hiện tại: GIÁ TRÊN CHƯA BAO GỒM VAT 8%
- Muốn đổi dòng này, sửa trong content.json tại footer.vat.


CẬP NHẬT NỘI DUNG CHỮ:
- content.json: dùng khi web chạy bằng Live Server/local server hoặc khi upload lên hosting.
- content.js: dùng khi mở index.html trực tiếp bằng double click từ ổ D. Trình duyệt thường chặn đọc file JSON local, nên nếu sửa content.json mà không thấy đổi, hãy sửa cùng nội dung trong content.js hoặc chạy web bằng Live Server.
- Dòng cuối trang hiện nằm ở footer.note. Muốn căn trái/phải/giữa, chỉnh footer.noteAlign thành left, right hoặc center.


CẬP NHẬT MỚI:
- Header đặt logo JPK VO và BRAVAT ở giữa.
- Dòng trên logo: JPK VO - BRAVAT PREMIUM SALE.
- Dòng dưới logo tự lấy số lượng sản phẩm và mức sale cao nhất: {count} MÃ SẢN PHẨM · SALE UP TO {maxDiscount}%.
- Tab ALL hiển thị toàn bộ sản phẩm của tất cả nhóm.
- Khi mở file trực tiếp bằng double click, chỉnh text trong content.js để thấy thay đổi ngay.
