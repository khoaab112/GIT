# SSH_KEY GIT
1. cài đặt git : 
```javascript   
sudo dnf install git-all
```
2. setup ssh key cho vps:
- check đã tồn tại ssh key nào chưa :
```javascript   
 ls -al ~/.ssh
```
3. Tạo ssh key cho git:
```javascript   
ssh-keygen -t rsa -b 4096 -C "[gmail đăng ký git]"
```
4. Thêm key vào ssh-agent :
-  Đảm bảo rằng `ssh-agent` đã được kích hoạt bằng lệnh :

```javascript 
eval "$(ssh-agent -s)"
```
 - Add ssh key của bạn vào `ssh-agent` :
 ```javascript
 ssh-add ~/.ssh/id_rsa
 ```
 5. lấy ssh ke từ server :
 ```javascript
 get ssh key :cat ~/.ssh/id_rsa.pub
 ```
 6. Vào githup truy cập vào địa chỉ :
 ```javascript
 https://github.com/settings/profile
 ```
 -  Click chọn SSH and GPG keys > New SSH Key
