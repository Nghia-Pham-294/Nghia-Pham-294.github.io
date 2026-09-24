# Website của Nghia Pham

Website tĩnh theo bố cục tham khảo của Caleb Langdon: ảnh tròn và thông tin bên trái; nội dung bên phải; tên dẫn về trang chủ; hai tab CV và Research. Không cần cài đặt hay chạy lệnh.

## Xem trước trên Mac

1. Giải nén `nghia-website-code.zip`. Safari có thể đã tự giải nén.
2. Mở thư mục chứa `index.html`, `cv.html`, `research.html`, `style.css` và `assets`.
3. Bấm đúp `index.html` để xem bằng Safari. Bấm CV, Research hoặc Nghia Pham để chuyển trang.

## Sửa ở đâu?

| Nội dung | File |
| --- | --- |
| Giới thiệu, Research Interests, Education trên trang chủ | `index.html` |
| Nội dung tab CV và link PDF | `cv.html` |
| Nội dung tab Research | `research.html` |
| Font, màu sắc, khoảng cách, khung ảnh | `style.css` |
| Ảnh chân dung | `assets/portrait.jpeg` |
| Tên, chức danh, email, LinkedIn, GitHub trong cột trái | Cùng đoạn `profile-details` ở cả ba file HTML |

Mở HTML/CSS bằng trình soạn thảo code. Trên GitHub cũng có thể bấm vào tên file rồi dùng nút bút chì để sửa. Các chỗ cần thay đều có chú thích trong code.

Research Interests có đúng hai mục: Machine Learning và Empirical Asset Pricing.
Education có đúng hai dòng: Caltech (PhD đang học) và MSc Bocconi. Không ghi năm tốt nghiệp.

## Thêm CV

Chưa có file CV PDF trong bộ code này. Tab CV hiện thông tin liên hệ và Education.
1. Đặt CV vào `assets/cv.pdf`.
2. Mở `cv.html`, tìm chú thích `CV PDF`.
3. Thay đoạn liên hệ ngay dưới chú thích bằng:

```html
<p><a href="assets/cv.pdf">Download CV (PDF)</a></p>
```

## Thêm nghiên cứu sau

Hiện tab Research chỉ có hai research interests; chưa đăng paper nào.
Trong `research.html` có đoạn mẫu được comment, trình duyệt không hiển thị. Khi sẵn sàng, bỏ dấu `<!--` và `-->` quanh mẫu, thay tiêu đề, mô tả, đường dẫn PDF. Chỉ bỏ comment khi file được liên kết đã có trong `assets`.

## Bật GitHub sau này

Trong cả ba file HTML, tìm `class="github-link" hidden`.
1. Thay `YOUR_USERNAME` bằng tài khoản muốn công khai.
2. Xóa chữ `hidden` trong dòng đó.

Hiện link GitHub được ẩn. Việc có repo để host web không bắt buộc phải công khai link GitHub trên giao diện.

## Upload vào repo hiện tại

Repo: https://github.com/Nghia-Pham-294/Nghia-Pham-294.github.io

1. Vào tab **Code** của repo → **Add file → Upload files**.
2. Từ thư mục đã giải nén, kéo **index.html, cv.html, research.html, style.css và nguyên thư mục assets** vào vùng upload. Kéo các mục bên trong, không kéo nguyên thư mục bọc ngoài hay ZIP.
3. GitHub sẽ thay hai file trùng tên `index.html`, `style.css` và thêm các file mới. Bấm **Commit changes**, chọn nhánh `main` nếu được hỏi.
4. Nếu mày vẫn đang để Pages ở `None`, upload chưa bật lại website. Khi muốn công khai: Settings → Pages → Source: Deploy from a branch → Branch: main → /(root) → Save.
5. Chờ deployment hoàn tất rồi xem https://nghia-pham-294.github.io/.

Bộ code này chỉ là các file để tải về, chưa tự upload hay thay đổi trạng thái GitHub Pages.
