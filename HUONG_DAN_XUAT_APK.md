# Hướng dẫn xuất file .APK gọn nhẹ cho Android (Không cần cài Android Studio)

Bộ mã nguồn này đã được cấu hình sẵn để đóng gói ứng dụng **Sổ Thu Chi Local** thành file cài đặt `.apk` trên điện thoại Android theo 3 cách từ gọn nhẹ nhất đến tự động hoàn toàn:

## Cách 1: Tự động xuất file `.apk` trên đám mây bằng GitHub Actions (0 MB cài đặt trên máy tính)
1. Tạo một tài khoản và một kho chứa (Repository) mới trên [GitHub](https://github.com).
2. Tải toàn bộ các file trong thư mục giải nén này lên Repository đó (bao gồm thư mục `www/`, `.github/workflows/build-apk.yml`, `package.json`, `capacitor.config.json`).
3. Bấm vào tab **Actions** trên GitHub → Chọn workflow **Build Android APK Automatically** → Bấm **Run workflow**.
4. Đợi khoảng 2 phút, máy chủ GitHub sẽ tự động biên dịch và trả về file **`SoThuChiLocal-Android-APK` (`app-debug.apk`)** ngay ở mục **Artifacts** để bạn tải về điện thoại cài đặt.

## Cách 2: Đóng gói thành `.apk` trong 30 giây bằng Website 2 APK Builder (Trên máy tính Windows)
1. Tải công cụ gọn nhẹ miễn phí **Website 2 APK Builder** (chỉ khoảng 60 MB, không cần cài Android Studio).
2. Chọn chế độ **Local HTML Website**.
3. Chọn thư mục **`www`** trong gói này (chứa `index.html`).
4. Đặt tên ứng dụng là `Sổ Thu Chi Local` và bấm **Generate APK** để nhận ngay file `.apk`.

## Cách 3: Mở và cài trực tiếp trên điện thoại Android (Không cần máy tính)
1. Chép file `www/index.html` vào điện thoại và mở bằng trình duyệt **Chrome**.
2. Bấm vào menu `⋮` góc trên bên phải Chrome → Chọn **Thêm vào màn hình chính (Add to Home Screen)**.
3. Biểu tượng **Sổ Thu Chi** sẽ xuất hiện ngay trên màn hình chính và hoạt động độc lập, lưu trữ dữ liệu 100% trên máy.
