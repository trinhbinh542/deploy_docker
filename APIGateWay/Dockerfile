


#sử dụng một hình ảnh cơ sở
FROM mcr.microsoft.com/dotnet/aspnet:7.0 AS runtime

#đặt thư mục làm việc hiện tại trong container là /app
WORKDIR /app

#sao chép các tệp từ thư mục ../release của host vào thư mục hiện tại của container
COPY ../release ./   

#xác định lệnh mà Docker sẽ thực thi khi container được khởi chạy
ENTRYPOINT ["dotnet", "APIGateway.dll"]


