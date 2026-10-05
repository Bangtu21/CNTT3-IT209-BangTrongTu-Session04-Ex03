Session04-Ex03
## 1. Tạo khóa SSH Ed25519
Sử dụng Git Bash để tạo cặp khóa SSH Ed25519 bằng lệnh `ssh-keygen -t ed25519`.

Khóa được lưu tại thư mục `~/.ssh/`, gồm:

* `id_ed25519`: khóa private, chỉ lưu trên máy cá nhân và không nộp lên GitHub.
* `id_ed25519.pub`: khóa public, được thêm vào GitHub để xác thực.

Sau đó kiểm tra kết nối bằng lệnh `ssh -T git@github.com` và xác thực SSH thành công.

## 2. Liên kết Remote Repository
Khởi tạo Git repository trong thư mục bài tập bằng `git init`, sau đó tạo commit cho file README.

Liên kết repository local với GitHub bằng remote SSH:

`git remote add origin git@github.com:Bangtu21/CNTT3-IT209-BangTrongTu-Session04-Ex03.git`

Kiểm tra bằng `git remote -v` cho thấy remote `origin` sử dụng giao thức SSH.

## 3. Đẩy dự án lên GitHub
Sử dụng lệnh `git push -u origin master` để đẩy branch `master` lên GitHub.

Kết quả cho thấy branch `master` đã được tạo trên GitHub và liên kết với `origin/master` thành công.

## 4. URL Repository
Repository GitHub:

https://github.com/Bangtu21/CNTT3-IT209-BangTrongTu-Session04-Ex03

Khóa private `id_ed25519` không được nộp hoặc tải lên GitHub.
