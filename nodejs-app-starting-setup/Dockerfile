FROM node
#  node라는 image

WORKDIR /app
##  //복사 전 여기서 RUN 실행하라

COPY package.json /app

RUN npm install

COPY . /app
# //첫 번째 경로는 컨테니너의 외부(이미지 외부).은 Dockerfile과 동일 선상
# // 두번째 경로는 컨테이너 내부 (컨테이너에 넣을 경로)


EXPOSE 80
## container는 내부 네트워크를 가짐

CMD ["node", "server.js"]
# CMD로 하면 
#RUN node server.js
##docker build 시에 한 번 실행 (image, container 시작 (container 시작하려고)) RUN이 많다면 여러 container 실행 가능
