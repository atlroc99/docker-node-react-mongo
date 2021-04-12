FROM node:14

WORKDIR /app

COPY . .

RUN npm install

VOLUME [ "/app/logs" ]

ENV PORT=80

ENV MONGODB_USERNAME=mzaman
ENV MONGODB_PASSWORD=secret

EXPOSE ${PORT}

CMD ["node", "app.js"]

# runnign mongodb container with username and password
#-e MONGO_INITDB_ROOT_USERNAME=mzaman
#-e MONGO_INITDB_ROOT_PASSWORD=secret

# docker run -d --rm -v mongo-data-dir:/data/dir -e MONGO_INITDB_ROOT_USERNAME=mzaman -e MONGO_INITDB_ROOT_PASSWORD=secret --network goals-net --name mz-mongo mongo:latest