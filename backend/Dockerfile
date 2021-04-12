FROM node:14

WORKDIR /app

COPY . .

RUN npm install

VOLUME [ "/app/logs" ]

ENV PORT=80

EXPOSE ${PORT}

CMD ["node", "app.js"]