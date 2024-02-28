# App Server
## WAS 환경에서 mariaDB 설치하기
```
$ sudo apt install mariadb-server
$ sudo apt install mariadb-client
$ sudo mysql_secure_installation
$ sudo systemctl enable mariadb
$ sudo systemctl start mariadb
```
```
# bg로 ./mvnw 실행
$ ./mvnw spring-boot:run &
# mariadb 실행
$ sudo mysql -u root -p
```



![image](https://github.com/miniproject4-team4/SPRING-BOOT-APP-SERVER/assets/148880521/03f33863-9628-4dec-adf3-353c0dfd24b4)


