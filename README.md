# Khóa học Static Demo

Dự án khóa học tĩnh (HTML thuần) chạy trên **GitHub Pages**.

## Cấu trúc

```
course-static/
├── index.html                 # Trang chủ - danh sách chương
├── css/style.css
├── modules/
│   ├── 01-gioi-thieu/
│   │   ├── index.html         # Trang tổng quan chương
│   │   ├── slides/
│   │   │   └── 01-demo.html   # Slide web (điều khiển bằng phím ← →)
│   │   ├── lab/
│   │   │   └── index.html
│   │   └── code/
│   │       └── example/
│   └── 02-chuong-hai/
└── README.md
```

## Cách chạy local

1. Mở thư mục bằng VS Code
2. Cài extension **Live Server**
3. Click chuột phải `index.html` → Open with Live Server

Hoặc dùng Python:

```bash
python -m http.server 8000
```

## Deploy lên GitHub Pages

1. Push toàn bộ nội dung lên GitHub và bảo đảm workflow nằm tại
   `.github/workflows/static.yml`.
2. Vào **Settings → Pages → Build and deployment**.
3. Ở **Source**, chọn **GitHub Actions** (không chọn **Deploy from a branch**).
4. Vào tab **Actions**, chạy workflow **Deploy static content to Pages** hoặc push
   một commit mới lên nhánh `master`.
5. Đợi workflow hoàn tất rồi truy cập `https://<username>.github.io/<repo-name>/`.

Nếu workflow báo `Get Pages site failed` hoặc `404 Not Found`, Pages chưa được
bật cho repository. Hãy thực hiện bước 2–3 trước khi chạy lại workflow. Nếu
repository thuộc tổ chức, administrator có thể cần cho phép GitHub Pages và
GitHub Actions trong phần policy của tổ chức.

## Thêm chương mới

1. Copy thư mục `01-gioi-thieu` → đổi tên thành `03-ten-chuong`
2. Sửa nội dung bên trong
3. Thêm thẻ `<a>` mới vào `index.html` gốc
