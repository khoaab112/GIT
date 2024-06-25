# Đẩy thay đổi nên repository
```bash
  Cơ bản
```
- `git add .` : thêm  hết tất cả thay đổi nên repository    
- `git commit -m "content"` :  tạo một commit với nội dung mong muốn
- `git push ` : tiến hành đẩy code lên repository

```bash
    Tùy chọn
```
 - `git status` : để xem các  thay đổi trước khi commit hoặc sau commit
 - `git log` : xem lịch sự commit trước đó
 - `git diff` : so sánh với commit cuối cùng

```bash
    Nâng cao
```
- `git add --all` :  thêm  hết tất cả thay đổi nên repository   
- `git add -A` :  thêm  hết tất cả thay đổi nên repository   
- `git add [danh sách cách file muốn commit]` : commit các file tùy chọn ví dụ git add index.html about.html
- `git commit --amend -m "content"` : Nếu commit đã được tạo ra nhưng chưa thực hiện push lên remote (khi có làm việc với Remote Repo - nói ở các phần sau) thì bạn có thể tạo ra commit mới thay thế cho commit cuối cùng đó. 
