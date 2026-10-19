# JSP Servlet Login

Bài thực hành Java Web: tạo form đăng nhập bằng JSP và xử lý POST bằng Servlet.

## Yêu cầu
- JDK 17+
- Maven 3.8+
- Apache Tomcat 10.1+

## Tính năng
- Form tại `index.jsp` gửi POST đến `/login`.
- Tên đăng nhập và mật khẩu mẫu: `admin` / `admin`.
- Đúng: `Welcome admin to website`.
- Sai: `Login Error`.

> Chú ý: tài khoản cố định chỉ phục vụ bài thực hành, không dùng cho ứng dụng thực tế.

## Chạy
1. Trong thư mục gốc, chạy `mvn clean package`.
2. Chép `target/jsp-servlet-login.war` vào thư mục `webapps` của Tomcat 10.1+.
3. Khởi động Tomcat.
4. Mở http://localhost:8080/jsp-servlet-login/

## Cấu trúc
- `pom.xml`: cấu hình Maven.
- `src/main/webapp/index.jsp`: form đăng nhập.
- `src/main/java/com/codegym/LoginServlet.java`: xử lý yêu cầu POST.
- `src/main/webapp/WEB-INF/web.xml`: cấu hình web.
