

# Sử dụng image nginx làm base
FROM nginx

# Xóa các tệp mặc định trong thư mục /usr/share/nginx/html của image nginx
RUN rm -rf /usr/share/nginx/html/*

# Sao chép các tệp build từ thư mục dist của ứng dụng Angular vào thư mục /usr/share/nginx/html của image
COPY release /usr/share/nginx/html

# Cấu hình nginx để phục vụ ứng dụng Angular
COPY nginx-custom.conf /etc/nginx/conf.d/default.conf

# Mở cổng 80
EXPOSE 80

# Chạy nginx khi container được khởi chạy
CMD ["nginx", "-g", "daemon off;"]