<p align="center">
 <img width="100px" src="https://upload.wikimedia.org/wikipedia/commons/9/91/Octicons-mark-github.svg" align="center" alt="GitHub Readme Stats" />
 <h2 align="center">Tìm hiểu về Git và Github</h2>
</p>

<div align="center">
 <table >
  <theader>
  <th>
   Nội Dung 
   </th>
   </theader>
  <tbody>
  <td>
   <p>1: Github là gì? Khác với git ở chỗ nào?</p>
   <p>2: Tại sao chúng ta lại cần dùng đến Git?</p>
   <p>3: Các trạng thái file trong git?</p>
   <p>4: Các câu lệnh đơn giản trong git?</p>
   <p>5: Cài đặt SSH lên máy tính window (local)?</p>
   <p>6: Thiết Lập Username và Email trong git ?</p>
   <p>7: Tạo Github Repository?</p>
   <p>8: thực hiện đẩy các thay đổi lên github?</p>
   </td>
   </tbody>
   </table>
</div>

# 1: Github là gì? Khác với git ở chỗ nào?
 <div>
    <table>
      <thead>
        <th>Git</th>
        <th>GitHub</th>
      </thead>
      <tbody>
        <tr>
          <td>một hệ thống quản lý phiên bản phân tán</td>
          <td>là một dịch vụ lưu trữ trên web dành cho các dự án có sử dụng hệ thống kiểm soát Git revision.</td>
        </tr>
        <tr>
          <td>một mô hình hệ thống, các máy tính có thể clone lại mã nguồn từ một repository</td>
          <td>một công ty cũng cấp dịch vụ máy chủ repository công cộng, mỗi người có thể truy cập vào website trang chủ để tạo tài khoản trên đó và tạo ra kho chứa source của riêng mình khi làm việc.</td>
        </tr>
      </tbody>
    </table>
</div>

# 2 Tại sao chúng ta lại cần dùng đến Git?

- Git đã mang đến rất nhiều lợi thế cho công việc lập trình:
- Git dễ sử dụng, an toàn và nhanh chóng.
- Quản lý source code dễ dàng chuyên nghiệp
- Có thể giúp quy trình làm việc code theo nhóm đơn giản hơn rất nhiều bằng việc kết hợp các phân nhánh(branch)
- Hạn chế được lỗi xảy ra trong quá trình code trong 1 team
- Khi gặp lỗi có thể dễ dàng Backup lại phiên bản trước
- Dễ dàng trong việc deployment sản phẩm.

# 3: Các trạng thái file trong git?

- Committed: có nghĩa là dữ liệu đã được lưu trữ một cách an toàn trong cơ sở dữ liệu, tức là những gì bạn đã commit thành công.
- Staged: là bạn đã đánh dấu sẽ commit phiên bản hiện tại của một tập tin đã chỉnh sửa trong lần commit sắp tới. Trạng thái này xảy ra khi bạn sử dụng lệnh git add - <file_name> nhưng chưa commit.
- Modified: có nghĩa là bạn đã thay đổi tập tin# nhưng chưa commit vào cơ sở dữ liệu, tức là bạn chưa sử dụng lênh git add và git commit.
- Cài đặt – Cấu hình git

# 4: Các câu lệnh đơn giản trong git?

git init:  Khởi tạo 1 git repository 1 project mới hoặc đã có.\
git add: Thêm thay đổi đến stage/index trong thư mục làm việc.\
git commit: commit nghĩa là một action để Git lưu lại một snapshot của các sự thay đổi trong thư mục làm việc và lưu trữ lịch sử commit\
git config: Để set user name và email của bạn trong main configuration file.\
git clone:  Copy 1 git repository từ remote source.\
git status: Để check trạng thái của những file bạn đã thay đổi trong thư mục làm việc.\
git push/git pull: Push hoặc Pull các thay đổi đến remote.\
git branch: liệt kê các brnach\
git checkout chuyển sang các bracnh khác\
git merge: Merge 2 branch lại với nhau.

# 5 Cài đặt SSH lên máy tính window (local)?

- SSH Key là một cặp key được dùng để mã hóa bất đối xứng, gồm có public key và private key. SSH Key được dùng để xác minh quyền truy cập và mã hóa nội dung để tránh bị tấn công.

- Bạn cứ hình dung Private Key là chìa khóa, còn Public Key là ổ khóa. Một khi chìa khóa mà vừa khít với ổ khóa thì cửa sẽ được mở, thế thôi.

** cấu hình ssh-key **

![image](https://user-images.githubusercontent.com/109157942/194510538-4559a7b7-6e9b-4e16-8a1c-1ee6cf877263.png)

 chọn setting > Developer settings > Personal access tokens > New personal access token > nhập tên note > chọn các quyền ssh > Generate token
 
 Kiểm tra cấu hình ssh lên trên máy và github: ssh-T git@github.com
 
 ![image](https://user-images.githubusercontent.com/109157942/194510754-dc656a44-8744-4b1c-84c6-aae95c65df54.png)
 
 # 6: Thiết Lập Username và Email trong git?
 
 Bước 1: Khởi Động Cửa Sổ Dòng Lệnh Hoặc Git Bash
 
 Bước 2: Thiết Lập Tên Người Dùng
 
 ```
 
  git config --global user.name "John Doe"
 
 ```
 
 Bước 3: Thiết Lập Địa Chỉ Email
 
 ```
 
 git config --global user.email "johndoe@example.net"
 
 ```
 
 Bước 4: Kiểm Tra Lại Các Thiết Lậ
 
 ```
 
 git config --global user.name
 git config --global user.email
 
 ```
 
 
 # 7: Tạo Github Repository?
 
 bước 1: tạo repository
 
  - Trên giao diện Github, Chọn New Repository
  
 ![image](https://user-images.githubusercontent.com/109157942/194511303-b943d8cb-fa6f-4013-ae3e-adfa0d25779c.png)

> lưu ý: Phần tên repository phải là duy nhất, không được trùng. Ở đây mình có demo thử một repo

![image](https://user-images.githubusercontent.com/109157942/194511484-d271b630-439d-4edb-9186-190972be53e4.png)

sau khi tạo một repo mới bạn sẽ có một kết quả như sau 

![image](https://user-images.githubusercontent.com/109157942/194512003-d53401a2-33f3-4c6b-be0b-4bccb625da90.png)

bước 2: tạo một new repository trên command line

bạn có thể chọn HTTPS(bạn phải login trên git base ở bước 6) hoặc SSH(dựa vào khóa ssh tạo ở bước 5)

Để bắt đầu làm việc , ta vào đúng mục muốn đẩy lên git và chọn gitbash

thực hiện các dòng lệnh 

vd:
![image](https://user-images.githubusercontent.com/109157942/194513622-ef94337c-d16e-473a-aac0-1b08a841cce7.png)


# 8: thực hiện đẩy các thay đổi lên github?

bạn thực hiện các câu lệnh sau

git add .\
bạn có thể đẩy toàn bộ các file bằng (git add .) hoặc  git add ten-file

git commit -m "nhưng thay doi"

git branch -M master\
master là nhánh chính bạn đnag làm việc 

git push -u origin master


![image](https://user-images.githubusercontent.com/109157942/194514329-300d4b3a-6db7-446b-b583-1873737e9322.png)

![image](https://user-images.githubusercontent.com/109157942/194515274-fcdbc60c-77a6-4ab4-b838-29bdd5c5cea8.png)

Và đây là dữ liệu chúng ta push lên trên nhánh đó.

![image](https://user-images.githubusercontent.com/109157942/194515472-ee2888a3-6abf-4913-a9a1-91b4e337f985.png)

Sau đó sẽ nhấn vào nút Compare & pull request. Nó sẽ hiện ra như hình dưới. Và ở đây chúng ta có thể xem sự thay đổi của file giữa lần đầu commit và lần commit sau đó.

![image](https://user-images.githubusercontent.com/109157942/194515554-4fceb5e4-cb7d-4740-846f-4d5c6263ee96.png)

- Copy đường link dẫn đến cho này gửi cho bạn bè, đồng nghiệp,.. để họ vào xem và kiểm tra code nhé.

- Để thêm ý kiến,…. và merge nó về nhánh master về code vừa được push lên thì nhấn vào Create pull request.

và bạn có thể xem  file thay đổi tại files changed

![image](https://user-images.githubusercontent.com/109157942/194515698-b9a5a411-d454-41ee-b999-6ad501862d96.png)

nếu bạn làm việc nhóm thì bạn có thể add leader vào review code của mình và meger vào nhánh tổng

![image](https://user-images.githubusercontent.com/109157942/194516375-6788c012-5cb2-4ac9-95ae-221a36245091.png)

![image](https://user-images.githubusercontent.com/109157942/194516196-23837bda-58fa-4f66-abf2-11fc7dace0ce.png)

sau khi bấm pull request bạn sẽ có thấy được sự thay đổi các file ở  nhánh master sẽ giống hệt  ở nhánh phụ mình vừa làm.













 
