# TAG || VERSION
- `Tag là chức năng đặt tên hay đánh dấu cho 1 commit bất kỳ, nhằm giúp chúng ta dễ dàng tìm kiếm đến commit đó. Nó giúp chúng ta dễ dàng tìm kiếm một commit được đánh dấu trong hàng loạt các commit`
- `dễ dàng đối chiếu, so sánh về sau này mà không cần nhớ checksum của mỗi commit, mà chỉ cần nhớ tag`
- `tạo hay gắn tag cho 1 commit cụ thể thì ta không thể thay đổi lịch sử của commit đó được nữa.`
- `phiên bản zip khi tạo tag chỉ là các nội dung được commit lên chứ không phải toàn bộ src của dụ án`
------------------------------------------
# Create a new tag
- `git tag [tag_name]` : tạo một tag mới gắn liền với commit cuối cùng của nhánh hiện tại đang đứng
- `git tag -a [tag_name] -m "[commit]" [hand_code]` : tạo một tag mới gắn liền với commit chỉ định (nếu không chỉ định thì mặc đính lấy commit cuối cùng) với nội dung mô tả cho tag
- `git tag` : danh sách tag

# Push a tag to the repository
`git push --tags` : đẩy toàn bộ tag chưa đc push lên remote repository
`git push origin [tag_name]` : đẩy 1 tag lên
# remove a tag from the repository
` git tag -d [tag_name]` : xóa tag với tên
