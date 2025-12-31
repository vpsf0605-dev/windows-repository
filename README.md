# 🌐 ZUNRDP - Remote Desktop Automation

Workflow này tự động tạo máy Windows hoặc Ubuntu trên GitHub Actions, cài đặt Remote Desktop, kết nối Tailscale và hiển thị thông tin truy cập. Tất cả các bước chạy **ẩn log**, chỉ hiện thông tin IP, User, Password và Port.

---

## ⚡ Tính năng

- Tạo máy Windows hoặc Ubuntu.
- Tạo user mới với quyền Admin/Sudo.
- Cài và kết nối **Tailscale** tự động.
- Cài **XRDP** trên Ubuntu.
- Hiển thị thông tin kết nối: IP, User, Pass, Port.
- Treo máy để nhận lệnh hoặc remote.
- Chạy hoàn toàn ẩn log, chỉ hiển thị thông tin truy cập.

---

## 📋 Cách sử dụng

1. Fork repository này hoặc tạo repository mới.
2. Vào **Settings → Secrets → Actions** và thêm:
   - `TAILSCALE_AUTH_KEY`: Token Tailscale.
3. Vào **Actions → Run workflow**:
   - Chọn hệ điều hành: **Windows** hoặc **Ubuntu**.
   - Nhấn **Run workflow**.

4. Chờ workflow chạy, xem **HIỂN THỊ THÔNG TIN WINDOWS/UBUNTU**:
5. ---

## 🖥️ Chi tiết hệ thống

- **Windows**
- User: `ADMINZUN`
- Pass: `ZunRDP@123456`
- Remote Desktop Port: 3389
- Kết nối thông qua IP Tailscale.
- **Ubuntu**
- User: `adminzun`
- Pass: `ZunRDP@123456`
- XRDP Port: 3389
- Kết nối thông qua IP Tailscale.

---

## ⚙️ Lưu ý

- Workflow treo máy sau khi chạy để nhận lệnh hoặc remote.
- Log cài đặt và cấu hình **được ẩn hoàn toàn**, chỉ hiển thị thông tin truy cập.
- Đảm bảo token Tailscale hợp lệ, nếu không workflow sẽ dừng.
- Windows hoặc Ubuntu đều có IP riêng do Tailscale cấp.

---

## 🔗 Tham khảo

- [Tailscale](https://tailscale.com/)
- [GitHub Actions](https://docs.github.com/en/actions)
- [XRDP trên Ubuntu](https://wiki.ubuntu.com/XRDP)
