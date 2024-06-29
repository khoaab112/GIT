# GITIGNORE :file chỉ định tệp tin || thư mục không theo dõi chúng nữa

- `*.log` : bỏ hết các file có đuôi là log
- `folder_1/` : bỏ theo dõi  thư mục  folder_1
- `file_1.txt` : bỏ file có tên file_1.txt
- `# comment` : tạo 1 comment   
- `!abc/example.exe` : phụ  định không theo dõi file example.exe ở folder abc
- `config/*.xml ` : chỉ định các file cụ thể ở trong config
- `folder/**` : chỉ định thư mục folder ở toàn dự án


# NODE
`khi mới thêm file .gitignore hoặc chỉnh sửa file .gitignore thì git cache có thể chưa nạp lại file .gitignore  nó vẫn dữ cache cũ`
 - `git rm -r --cached /path/to/file_or_folder` : xóa cache  cho thư mục hoạc file cụ thể nào đó
 - `git rm -r --cached .`: xóa cache git cho toàn bộ dự án
 tiếp theo `git add` rồi commit lại file .gitinore
 nếu chỉ xóa cache không thôi thì `gid add` là ok
