FROM nginx:alpine

WORKDIR /usr/share/nginx/html

COPY 2048.zip /tmp/2048.zip

RUN apk add --no-cache unzip && \
    unzip /tmp/2048.zip -d /tmp && \
    mv /tmp/2048-master/* /usr/share/nginx/html/ && \
    rm -rf /tmp/*

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
