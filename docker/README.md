# docker

```sh
# nest 설치
npm i -g @nestjs/cli

# nest project 생성
nest new handson -p npm --skip-git

# project 경로로 이동
cd ./handson

# Dockerfile 복사
cp ../Dockerfile .

# 코드 빌드
npm run build

# docker 빌드
docker build -t handson:v0.0.1 -t handson:latest .

# 확인
docker image ls
```
