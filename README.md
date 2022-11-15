# DockerFile
*P1:
1. FROM
FROM <image> [AS <name>] : Chỉ định image nào sẽ làm base image để trong quá trình build image thực hiện câu lệnh tiếp theo. Các base image này sẽ được tải về từ Public or Private Repo riêng của mỗi người tùy theo setup
2. RUN 
VD: RUN apt-get update -y : Dùng để chạy câu lệnh trong quá trình build image
3. COPY
COPY [--chown=<user>:<group>] <src>... <dest> : Copy file từ thư mục <src> và thêm vào thư mục <dest> của container
4. CMD
CMD command param1 param2 : Định nghĩa các câu lệnh được chạy sau khi container được khởi động từ image đã build. Có thể khai báo được nhiều nhưng chỉ duy nhất CMD cuối cùng được chạy.
5. Build image PHP từ ubuntu 20.04 : https://congdonglinux.com/how-to-create-docker-images/
6. Build context : Thư mục trên host chứa dockerfile gọi là build context. Khi build toán bộ các file/thư mục trong build context được send đến docker sever
7. Dockerignore : Nó sẽ bỏ qua các thành phần không cần thiết được định nghĩa trong file vào image. Chỉ giữ lại các thành phần cần thiết -> giảm size
*P2:
 - touch Dockerfile
 - docker images
 - docker pull image:tag
 - docker image rm imageName
 - docker run -it --name Name -p 0000:0000 image bash
 - 
 - CTRL + P + Q         
 - 
