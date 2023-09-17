# 개발환경 설정법

## 레포 클론

```bash
git clone https://github.com/withSang/zilzu-ghost-website
cd zilzu-ghost-website
code .
```

## node 가상환경 설정

```bash
# 16.16.0 버전의 node 설치
fnm install 16.16.0
# 16.16.0 버전의 node 사용
fnm use
# yarn 설치
npm install -g yarn
```

## 테마 개발 환경 시작

```bash
# 필요한 패키지 설치
yarn
# 테마 개발 환경 시작
yarn dev
```

## docker container 시작

```bash
# docker volume 생성 (웹사이트용 DB)
docker volume create ghost-db-data
# docker container 시작
yarn ghost:up
```

[localhost:8080](http://localhost:8080)으로 접속하여 블로그 설정 가능
