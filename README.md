# Hệ thống Quản lý Phòng Cấy Mô

Hệ thống quản lý phòng cấy mô được xây dựng bằng Python Flask, giúp theo dõi và quản lý các môi trường nuôi cấy mô thực vật.

## Tính năng

- Quản lý người dùng (đăng ký, đăng nhập)
- Quản lý môi trường nuôi cấy (thêm, sửa, xóa)
- Theo dõi lịch sử thay đổi môi trường
- Giao diện người dùng thân thiện với Bootstrap

## Yêu cầu hệ thống

- Python 3.8 trở lên
- pip (Python package installer)
- SQLite3

## Cài đặt

1. Clone repository:
```bash
git clone <repository-url>
cd tissue-culture-app
```

2. Tạo môi trường ảo:
```bash
python -m venv venv
```

3. Kích hoạt môi trường ảo:
- Windows:
```bash
venv\Scripts\activate
```
- Linux/Mac:
```bash
source venv/bin/activate
```

4. Cài đặt các gói phụ thuộc:
```bash
pip install -r requirements.txt
```

5. Tạo file .env:
```bash
SECRET_KEY=your-secret-key
DATABASE_URL=sqlite:///tissue_culture.db
```

6. Khởi tạo cơ sở dữ liệu:
```bash
python run.py
```

## Sử dụng

1. Chạy ứng dụng:
```bash
python run.py
```

2. Truy cập ứng dụng tại: http://localhost:5000

## Cấu trúc thư mục

```
tissue-culture-app/
├── app/
│   ├── __init__.py
│   ├── models/
│   │   ├── nguoi_dung.py
│   │   └── moi_truong.py
│   ├── routes/
│   │   ├── auth.py
│   │   ├── main.py
│   │   └── moi_truong.py
│   └── templates/
│       ├── auth/
│       ├── moi_truong/
│       └── base.html
├── venv/
├── .env
├── .gitignore
├── requirements.txt
└── run.py
```

## Đóng góp

Mọi đóng góp đều được hoan nghênh. Vui lòng tạo issue hoặc pull request để đóng góp.

## Giấy phép

[MIT License](LICENSE) 