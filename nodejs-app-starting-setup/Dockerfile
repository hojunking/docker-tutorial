FROM node
#  node라는 image

WORKDIR /app
##  //복사 전 여기서 RUN 실행하라

COPY . /app
# //첫 번째 경로는 컨테니너의 외부(이미지 외부).은 Dockerfile과 동일 선상
# // 두번째 경로는 컨테이너 내부 (컨테이너에 넣을 경로)

RUN npm install

CMD node server.js
#RUN node server.js
##docker build 시에 한 번 실행 (image, container 시작 (container 시작하려고))
