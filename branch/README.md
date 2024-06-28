# LÀM  VIỆC VỚI NHÁNH
#
# Checkout = Switch + Restore
# 
----------------------------------------------------------------

- `git checkout ` :được dùng để chuyển nhánh hoặc để phục hồi file trong thư mục làm việc từ một commit trước đây \
    -  `git checkout master` : chuyển sang nhánh master \
    -  `git checkout [hash_code] index.html` : phục hồi file index.html theo commit có mã hasd \
    -  `git checkout  index.html` : phục hồi file index.html theo commit cuối cùng đc cập nhật ở nhánh hiện tại \
    -  `git checkout -- *.html` : phục hồi file .html theo commit cuối \
    -  `git checkout -- .` : phục hồi tất cả theo commit cuối \
    -  `git checkout [hash_code]` : trờ về commit có mã hasd mà mình chuyển tới [ lúc này con trỏ HEAD sẽ chuyển đến commit này, và Git ở chế độ head detached, bạn làm việc trên một nhánh tạm thời ] \

----------------------------------------------------------------

- `git switch` :  dùng để chuyển nhánh và có thể tạo nhánh mới \
    - `git switch master` :     chuyển sang nhánh master \
    - `git switch -c [new_branch] [hash_code]` : tạo nhánh mới có tên new_branch theo commit có hash_code \
    - `git switch -c [new_branch]` : tạo nhánh mới theo commit cuối  \

----------------------------------------------------------------

- `git restore .`: phục hồi tất cả các file từ commit cuối
- `git restore <file>` : phục hồi file từ commit cuối

----------------------------------------------------------------

- `git branch [branch_name]` : tạo nhánh branch_name từ nhánh hiện tại
- `git branch -l` : xem nhánh hiện tại
- `git branch -a` : xem tất cả các nhánh ở local
- `git branch -d [branch_name]` : xóa nhánh branch_name khỏi git
- `git push origin -d [branch_name]` : Cập nhật lại trạng thái nhánh đã xóa ở local  || xóa nhánh đó ở local

----------------------------------------------------------------

