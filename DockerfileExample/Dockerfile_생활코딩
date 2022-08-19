FROM ubuntu:20.04

RUN apt update && apt install -y python3
WORKDIR /var/www/html

# RUN echo "Hello, <strong>Docker</strong>" > index.html
# 첫 번째 인자 host의 파일을 컨테이너의 wkdir에 전체 복사
COPY ["index.html", "."] 
CMD ["python3", "-u", "-m", "http.server"]