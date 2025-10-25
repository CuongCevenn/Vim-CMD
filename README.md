
# 🧠 Vim — Các phím tắt hữu ích khi chỉnh sửa file

## 🧭 1. Các chế độ cơ bản trong Vim

| Chế độ | Cách vào | Chức năng |
|---------|-----------|------------|
| **Normal mode** | `Esc` | Dùng để di chuyển & ra lệnh |
| **Insert mode** | `i`, `a`, `o` | Gõ chữ, thêm ký tự hoặc mở dòng mới |
| **Visual mode** | `v`, `V`, `Ctrl+v` | Chọn vùng văn bản |
| **Command-line mode** | `:` | Gõ lệnh (vd `:w`, `:q`) |

---

## 🏃 2. Di chuyển nhanh

| Phím | Chức năng |
|------|------------|
| `h`, `j`, `k`, `l` | Trái / Xuống / Lên / Phải |
| `0` hoặc `^` | Đầu dòng |
| `$` | Cuối dòng |
| `gg` | Đầu file |
| `G` | Cuối file |
| `Ctrl + f` | Lướt xuống 1 trang |
| `Ctrl + b` | Lướt lên 1 trang |
| `w` | Nhảy tới đầu từ tiếp theo |
| `b` | Nhảy về đầu từ trước |
| `}` | Nhảy tới đoạn kế tiếp |
| `{` | Nhảy về đoạn trước |

---

## ✂️ 3. Chỉnh sửa văn bản

| Phím | Tác dụng |
|------|-----------|
| `x` | Xóa ký tự tại con trỏ |
| `dd` | Xóa dòng hiện tại |
| `yy` | Sao chép dòng hiện tại |
| `p` | Dán sau con trỏ |
| `P` | Dán trước con trỏ |
| `u` | Hoàn tác (undo) |
| `Ctrl + r` | Làm lại (redo) |
| `cw` | Thay thế 1 từ |
| `cc` | Thay thế cả dòng |
| `r<char>` | Thay thế ký tự tại con trỏ |
| `J` | Nối dòng với dòng kế tiếp |
| `>>` | Thụt dòng sang phải |
| `<<` | Thụt dòng sang trái |

---

## 🧾 4. Làm việc với toàn bộ file

| Lệnh | Chức năng |
|------|------------|
| `:%d` | Xóa toàn bộ nội dung |
| `:%y` | Copy toàn bộ nội dung |
| `:%s/old/new/g` | Tìm và thay tất cả |
| `:w` | Lưu file |
| `:q` | Thoát |
| `:wq` hoặc `ZZ` | Lưu và thoát |
| `:q!` | Thoát không lưu |
| `:e filename` | Mở file khác |
| `:w filename` | Lưu thành file mới |

---

## 🔍 5. Tìm kiếm và thay thế

| Lệnh | Chức năng |
|------|------------|
| `/từ_cần_tìm` | Tìm xuống dưới |
| `?từ_cần_tìm` | Tìm lên trên |
| `n` | Lặp lại tìm kiếm (cùng hướng) |
| `N` | Lặp lại ngược hướng |
| `:%s/foo/bar/g` | Thay toàn bộ “foo” thành “bar” |
| `:s/foo/bar/` | Thay trong dòng hiện tại |

---

## 📚 6. Chọn và thao tác khối (Visual mode)

| Phím | Chức năng |
|------|------------|
| `v` | Chọn ký tự |
| `V` | Chọn dòng |
| `Ctrl + v` | Chọn khối (block) |
| `d` | Xóa vùng chọn |
| `y` | Copy vùng chọn |
| `p` | Dán đè vùng chọn |

---

## 🪄 7. Các thao tác tiện dụng khác

| Phím | Tác dụng |
|------|-----------|
| `.` | Lặp lại lệnh vừa làm |
| `Ctrl + g` | Hiện vị trí con trỏ & tên file |
| `:set number` | Hiển thị số dòng |
| `:set relativenumber` | Hiển thị số dòng tương đối |
| `:syntax on` | Bật tô màu cú pháp |
| `:noh` | Xóa highlight tìm kiếm |
| `ZZ` | Lưu và thoát nhanh |

---

## 💡 8. Mẹo cực nhanh

| Hành động | Lệnh |
|------------|------|
| Chọn tất cả và xóa | `ggdG` hoặc `:%d` |
| Sao chép tất cả | `:%y` |
| Xóa từ con trỏ → cuối file | `dG` |
| Xóa 5 dòng | `5dd` |
| Lặp lại lệnh vừa làm 10 lần | `10.` |
| Tìm & thay chữ toàn file | `:%s/old/new/gc` |
