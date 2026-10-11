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

1. Tạo repo mới trên GitHub
2. Push toàn bộ nội dung thư mục này lên
3. Vào **Settings → Pages**
4. Source: Deploy from a branch → chọn `main` / `root`
5. Đợi vài phút, truy cập `https://<username>.github.io/<repo-name>/`

## Thêm chương mới

1. Copy thư mục `01-gioi-thieu` → đổi tên thành `03-ten-chuong`
2. Sửa nội dung bên trong
3. Thêm thẻ `<a>` mới vào `index.html` gốc
