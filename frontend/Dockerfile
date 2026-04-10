FROM nginx:1.24-alpine3.17-slim
EXPOSE 80
RUN rm -rf /usr/share/nginx/html/* 
RUN rm -rf /etc/nginx/nginx.conf /etc/nginx/conf.d/default.conf
COPY nginx.conf /etc/nginx/
COPY app /usr/share/nginx/html/
CMD ["nginx", "-g", "daemon off;"]