# SrpingJWTh2

https://www.bezkoder.com/spring-boot-jwt-authentication/

spring.h2.console.enabled=true
# default path: h2-console
spring.h2.console.path=/h2-ui
 
spring.datasource.url=jdbc:h2:file:./subdirectory/demodb
spring.datasource.driverClassName=org.h2.Driver
spring.datasource.username=sa
spring.datasource.password=admin
 
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.H2Dialect
spring.jpa.hibernate.ddl-auto= update

# App Properties
bezkoder.app.jwtCookieName= bezkoder
bezkoder.app.jwtSecret= bezKoderSecretKey
bezkoder.app.jwtExpirationMs= 86400000

H2 db UI url
http://localhost:8080/h2-ui/login.do?jsessionid=c7bb12b5de0250e8f0ef283f2611e738


http://localhost:8080/api/auth/signup   -- post 

req body :

{"username":"subbu",
"email":"subbu@cg.com",
"password":"subbu@123",
"role":["subbu","user"]
}



select * from roles;
select * from users;
select * from user_roles;



INSERT INTO roles(name) VALUES('ROLE_USER');
INSERT INTO roles(name) VALUES('ROLE_MODERATOR');
INSERT INTO roles(name) VALUES('ROLE_ADMIN');

