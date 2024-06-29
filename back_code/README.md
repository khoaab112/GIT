# Đưa code về một commit nào đó ?

#### GIT RESET || GIT REVERT
----------------------------------------------------------------
# GIT RESET 
- `git reset [hard_commit]` : được sử dụng để di chuyển HEAD (con trỏ chỉ đến commit hiện tại) trỏ đến một commit cụ thể.
`git reset có 2 tùy chọn đó là: git reset --hard và git reset --soft.` :
    - `--hard`: Di chuyển HEAD trỏ đến commit đã chỉ định và đặt lại trạng thái làm việc (working directory) để trạng thái của bạn trở về trạng thái của commit đã chỉ định. Các thay đổi chưa được commit sẽ mất.
    - `--soft`: Di chuyển HEAD trỏ đến commit đã chỉ định, nhưng không thay đổi trạng thái làm việc (working directory).
- `git reset --hard`: nó sẽ xóa các commit cũ sau con trỏ chỉ định và không thể khôi phục lại được
# syntax : hard || soft 
- `git reset --hard [hard_commit]` :back code đến commit chỉ định
- `git reset --hard [hard_commit]^` :back code  trước 1 commit tính từ commit chỉ định
- `git reset --hard [hard_commit]~1` :back code  trước 1 commit tính từ commit chỉ định
- `git reset --hard [hard_commit]~2` :back code  trước 2 commit tính từ commit chỉ định
- `git reset --hard [hard_commit]~n` :back code  trước n commit tính từ commit chỉ định

# sau khi xóa xong cần :
- `git clean -f  -d` : được sử dụng để xóa các tệp không được theo dõi trong thư mục làm việc của bạn
- `git push --force origin <branch-name>` :Để xóa các commit này khỏi remote repository

 # GIT REVERT 
 `Git revert được sử dụng để tạo một commit mới, loại bỏ các thay đổi đã được thực hiện trong một hoặc nhiều commit trước đó, và áp dụng các thay đổi đó vào nhánh hiện tại.`

`git revert [hard_commit]` : tạo commit mới nhằm quay lại commit chỉ định || bản chất là copy code ở commit chỉ định rồi tạo commit mới ở HEAD cuối

Lưu ý : 
- revert  : sẽ tạo ra một commit mới , copy code ở commit chỉ định vào commit cuối 
- nó không xóa lịch sử commit cũ
- có thể sảy ra config
- nếu merge lại các commit cũ từ nhánh cũ thì không thể được vì các mã commit vẫn còn đó


