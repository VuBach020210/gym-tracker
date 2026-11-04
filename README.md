# Gym Tracker PWA

Ứng dụng ghi log tập luyện cá nhân, ưu tiên offline và lưu dữ liệu cục bộ bằng IndexedDB.

## Chạy thử trên Windows
1. Giải nén thư mục.
2. Mở thư mục bằng VS Code hoặc Cursor.
3. Cài extension **Live Server**.
4. Chuột phải `index.html` → **Open with Live Server**.
5. Kiểm tra giao diện trên trình duyệt máy tính.

Lưu ý: `file://` không phù hợp để kiểm tra service worker/PWA. Hãy dùng localhost hoặc hosting HTTPS.

## Đưa lên iPhone bằng GitHub Pages
1. Tạo tài khoản GitHub nếu chưa có.
2. Tạo repository mới, ví dụ `gym-tracker`.
3. Upload toàn bộ nội dung thư mục này lên repository (các file `index.html`, `app.js`, `styles.css`, `manifest.webmanifest`, `sw.js`, thư mục `icons` phải nằm ở thư mục gốc).
4. Vào **Settings → Pages**.
5. Chọn **Deploy from a branch** → branch `main` → folder `/ (root)` → Save.
6. Đợi GitHub Pages cấp URL dạng `https://TEN-GITHUB.github.io/gym-tracker/`.
7. Mở URL đó bằng Safari trên iPhone.
8. Nhấn Share → Add to Home Screen → bật **Open as Web App** nếu có → Add.

## Lưu ý dữ liệu
- IndexedDB lưu dữ liệu trên thiết bị/trình duyệt hiện tại.
- Dùng Settings → Export JSON thường xuyên để backup.
- Không xóa dữ liệu Safari/website nếu chưa có bản backup.
- Dữ liệu không tự đồng bộ giữa iPhone và máy tính.
- Sau khi cập nhật code, mở lại app khi có mạng để nhận bản mới.

## Phạm vi bản khởi đầu
Đã có: dashboard, thư viện bài tập mẫu, tạo buổi tập, nhập kg/reps/RIR, lịch sử, volume, PR cơ bản, biểu đồ volume, phân bổ working sets theo nhóm cơ, export/import JSON, service worker.

Cần phát triển tiếp: thêm/sửa/xóa bài tập tùy chỉnh, sửa/xóa buổi tập, lịch tập dạng calendar/template, effective-set weighting nâng cao, chart e1RM theo bài tập, muscle map trực quan, rest timer, deload/mesocycle, đồng bộ tùy chọn.
