# Hợp nhất nhánh || code
# ----------------------------------------------------------------
`Git merge` : sẽ chuyển toàn bộ commit ở branchB vào master, tạo ra 1 commit thông báo merged thành công, thứ tự commit theo thời gian.

`Git rebase` :  không tạo ra commit merged, thứ tự commit tùy thuộc cách áp dụng rebase

`Git cherry-pick` : chỉ chọn một số commit ở branchB áp dụng vào master, không tạo ra commit merged, các commit được nối tiếp vào nhánh master
# ----------------------------------------------------------------

- `git merge [branch_name]` : nhánh muốn mượt vào nhánh hiện tại
