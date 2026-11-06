# Preflight3D — bản cài đặt

**Kiểm tra & tối ưu file in 3D trước khi in — theo đúng máy, nhựa và tấm bàn của bạn.**

Repo này chỉ chứa **bản cài đặt** của Preflight3D. Tải ở mục **[Releases](https://github.com/tuanmd3001/Preflight3D-releases/releases/latest)**.

## Tải bản mới nhất

| Hệ điều hành | Link |
|---|---|
| macOS Apple Silicon (M1–M4) | [Preflight3D_macOS_Apple_Silicon.dmg](https://github.com/tuanmd3001/Preflight3D-releases/releases/latest/download/Preflight3D_macOS_Apple_Silicon.dmg) |
| Windows 10/11 64-bit | [Bộ cài .exe](https://github.com/tuanmd3001/Preflight3D-releases/releases/latest/download/Preflight3D_Windows_x64-setup.exe) · [.msi](https://github.com/tuanmd3001/Preflight3D-releases/releases/latest/download/Preflight3D_Windows_x64.msi) |
| Linux x86_64 | [AppImage](https://github.com/tuanmd3001/Preflight3D-releases/releases/latest/download/Preflight3D_Linux_x64.AppImage) · [.deb](https://github.com/tuanmd3001/Preflight3D-releases/releases/latest/download/Preflight3D_Linux_amd64.deb) |

Các link trên luôn trỏ tới **bản mới nhất**. Số phiên bản ghi ở tiêu đề mỗi bản phát hành.

## Lần mở đầu

- **macOS**: bản chưa ký Developer ID. Chuột phải vào app → **Open** → **Open**. Nếu macOS báo app "bị hỏng":
  ```bash
  xattr -dr com.apple.quarantine /Applications/Preflight3D.app
  ```
- **Windows**: nếu SmartScreen chặn → **More info** → **Run anyway**.
- **Linux (AppImage)**: `chmod +x Preflight3D_Linux_x64.AppImage` rồi chạy.

## Nên cài thêm

- **Bambu Studio** — để Preflight3D đọc máy in, nhựa, tấm bàn và preset của bạn.
- **Claude Code CLI** (tuỳ chọn) — cho chế độ phân tích AI. Không có vẫn dùng được bộ quy tắc offline.

## Kiểm tra file tải về

Mỗi bản phát hành có `SHA256SUMS.txt`:
```bash
shasum -a 256 -c SHA256SUMS.txt --ignore-missing
```

## Giấy phép

MIT — xem [LICENSE](LICENSE). Preflight3D là bản phái sinh của [LayerZero Studio](https://github.com/nnmduc/layerzero).
