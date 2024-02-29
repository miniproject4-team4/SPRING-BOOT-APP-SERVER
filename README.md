# App Server
## WAS 환경에서 mariaDB 설치하기
```
$ sudo apt install mariadb-server -y
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
- application.properties에서 port번호가 8081로 기본설정 되어있음
- cmd관리자 권한에서 다음과 같이 설정
```
$ netsh interface portproxy add v4tov4 listenport=8080 listenaddress=0.0.0.0 connectport=8081 connectaddress=172.17.82.181
$ netsh interface portproxy show v4tov4

ipv4 수신 대기:             ipv4에 연결:

주소            포트        주소            포트
--------------- ----------  --------------- ----------
0.0.0.0         8080        172.17.82.181   8081

```



## 💻⚡
![image](https://github.com/miniproject4-team4/SPRING-BOOT-APP-SERVER/assets/148880521/03f33863-9628-4dec-adf3-353c0dfd24b4)


