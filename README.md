# alpine_nodejs_dockerfile

FROM alpine:3.7
RUN apk add  --no-cache --repository http://dl-cdn.alpinelinux.org/alpine/v3.7/main/ \
--repository http://dl-cdn.alpinelinux.org/alpine/v3.7/community/ \  
nodejs>=8 ca-certificates tzdata ffmpeg
RUN npm i pm2  -g
