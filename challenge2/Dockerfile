# Fedora 베이스 이미지 사용
FROM fedora:latest

# 웹 서버 설치
RUN dnf -y install httpd

# tar 파일을 /var/www/html에 복사하고 압축 해제
ADD website.tar.gz /var/www/html/

CMD [ "-D", "FOREGROUND" ]

ENTRYPOINT ["/usr/sbin/httpd"]

# 포트 80 노출
EXPOSE 80
