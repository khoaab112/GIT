# Hợp nhất nhánh || code
# ----------------------------------------------------------------
`Git merge` : sẽ chuyển toàn bộ commit ở branchB vào master, tạo ra 1 commit thông báo merged thành công, thứ tự commit theo thời gian.

`Git rebase` :  không tạo ra commit merged, thứ tự commit tùy thuộc cách áp dụng rebase

`Git cherry-pick` : chỉ chọn một số commit ở branchB áp dụng vào master, không tạo ra commit merged, các commit được nối tiếp vào nhánh master

`merge và rebase` : cơ bản là kéo các commit tới branch cần hợp nhất
    - merge : thì tạo ra các commit mới vào nhánh cần hợp nhất  , nó copy các commit từ nhánh cũ vào nhánh hợp nhất
    - rebase : thì là di chuyển commit từ nhánh cũ vào nhánh cần hợp nhất , lịch sử commit của nhánh cũ sẽ không còn vì nó đã chuyển tới nhánh mới
# ----------------------------------------------------------------

- `git merge [branch_name]` : nhánh muốn merge vào nhánh hiện tại

- `git cherry-pick [hash_code_commit]` : Thêm một commit vào nhánh hiện tại
- `git cherry-pick [hash_code_commit_1 hash_code_commit_2]` : Thêm 2  hay nhiều commit vào nhánh hiện tại
- `git cherry-pick [hash_code_commit_1...hash_code_commit_6]` : Thêm các commit lần lượt từ 2 ->6
- `git cherry-pick [hash_code_commit_1^...hash_code_commit_6]` : Thêm các commit lần lượt từ 1 ->6

