FROM node:20.20.2-alpine3.23
WORKDIR /app
COPY *.js .
COPY package.json .
RUN npm install
EXPOSE 8080
ENV MONGO="true" \
    MONGO_URL="mongodb://mongodb:27017/catalogue"
CMD ["server.js"]
ENTRYPOINT ["node"]