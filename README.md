# Docker cheatsheets

## Table of contents

0. cheatsheet

## 0. cheatsheet
### Image
- `docker images` : image  확인
- `docker rmi [IMAGE]` : image 삭제
	- `docker rmi -f [IMAGE]` : image를 사용하는 container가 있어도 삭제

### Container

- `docker ps` : 동작중인 container 확인
	- `docker ps -a` : 모든(+정지된) container 확인
- `docker rm [CONTAINER]` : container 삭제 (동작중인 container 삭제 안됨)
	- `docker rm -f [CONTAINER]` : 동작중인 container 삭제

## 1. Build Docker image

- `docker build` : Build an image from a Dockerfile
	- `docker build -t [NAME:TAG(optional)]` : 주어진 이름:태그 형식으로 image build

- `docker tag` : Create a tag TARGET_IMAGE that refers to SOURCE_IMAGE
	- `docker tag SOURCE_IMAGE[:TAG] TARGET_IMAGE[:TAG]`

- `docker push` : Push an image or a repository to Docker Hub
	- `docker push NAME[:TAG]`

### References
- [초보를 위한 도커 안내서 - 이미지 만들고 배포하기](https://subicura.com/2017/02/10/docker-guide-for-beginners-create-image-and-deploy.html)
