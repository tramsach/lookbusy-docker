xoá version (dòng 1) để chạy

hướng dẫn từ web

Cài đặt Lookbusy

Yêu cầu VPS của bạn đã được cài đặt sẵn Docker và Git.

Clone repo sau về máy


https://github.com/10h30/lookbusy-docker.git


Truy cập vào thư mục và kích hoạt

cd lookbusy-docker
docker compose up -d --build

Chờ vài phút để hệ thống kích hoạt.

Kiểm tra lại lookbusy đã hoạt động ổn định chưa bằng cách kiểm tra log

docker compose logs


Thông báo hiện ra như bên dưới: lookbusy sẽ duy trì tải cpu luôn trong khoảng 15-20%

lookbusy  | cpu_spin (7): starting 4 spinner(s) for 15%-20% usage


Kiểm tra tải hệ thống bằng btop : lookbusy chạy 4 instance khác nhau để giữ CPU luôn hoạt động trong ngưỡng yêu cầu.