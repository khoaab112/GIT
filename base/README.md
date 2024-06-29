```bash
 https://duthanhduoc.com/blog/toi-hoc-lai-git-tu-dau#10-day-code-len-git-server-voi-git-push
```demo

## Cơ bản

- `repository` (repo) : Kho lưu trữ
- `commit` : một đơn vị làm việc
- `branch` : nhánh
- `main/master` : tên của repo chính
- `merge / rebase` : kết hợp 2 nhánh

## câu lệnh
- `git --help` : danh sách câu lệnh
- `git --version` : phiên bản git
- `git status` : hiển thị trạng thái kho lưu trữ, trạng thái thay đổi của các file, thư mục
- `git log` : hiển thị lịch sử commit
- `git log --oneline` : Nếu muốn nhìn thấy thông tin rút gọn thì
           - Enter - dòng tiếp theo
           - w - trang tiếp
           - spacebar - trang trước
           - ?pattern - tìm kiếm, với pattern là mẫu tìm kiếm (keyword)
           - /pattern - giống ?pattern
           - n - đến vị trí tìm kiếm phía dưới
           - N - đến kết quả tìm kiếm phía trước
           - q - thoát
- `git init [tên repo mới muốn tạo]`: tạo ra một repo mới và đặt tên theo yêu cầu
- `git clone [repo name]` : clone dự án  , tạo bản sao dự án
- `git config -l` : xem cấu hình hiện tại
- `git config -l [--scope] [option_name] [value]` : cấu hình repo \
    -   scope : __ `system` => tất cả người dùng \
                __ `global` => liên quan đến nhiều repository \
                __ `local`  => liên quan đến 1 repo \
 - `git branch` :  xem đang ở nhánh nào
 - `git checkout [repo name]` :chuyển sang nhánh mới
 - `git switch [repo name]` :chuyển sang nhánh mới
 - `git add ` : lưu thông tin để tiến tới bưỡc commit 
 - `git commit` : tạo commit
 - `git reset` :
 - `git pull` : kéo code từ repository về 
 - `git push` : đẩy các commit mới lên
 - `git fetch` :  lấy các thôgn tin về commit mới
 - `git branch –all` :  hiển thị danh sách các branch hiện có ở remote repository
 
 # Một vài điểm lưu ý :
 `git pull vs git fetch` : cả 2 đều là lấy code từ repo về local nhưng chúng  có sự khác nhau \
- `git pull` : kéo các commit về local và tạo lệnh merge  chúng ngay dê gây xung đột (lấy toàn bộ code) \
- `git fetch` :  chỉ kéo các commit về local mà chưa hề tạo lệnh mượt  nếu có sự thay đổi giữa repo và local (đơn giản là lấy thông tin)

    ----------------------------------------------------------------
# tool git : biết thêm thôi chứ cũng không đẹp lắm
- `gitk` : xem danh sách commit một cách trực quan hơn qua công cụ
- `git gui` : xem danh sách commit một cách trực quan hơn qua công cụ


