FROM node:14

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

EXPOSE 3000

CMD ["npm", "start"] 

# docker run --rm -it -p 3000:3000 goals-fe:latest
#  Running with the goals-net:
#  Even having the react app running on the same network as node backend app, the react app is not able to access node backend app with it's container name
#  b/c the react app's js code runs on the browser and it can only recognize the localhost or ip address and port that is 
#  docker run -d -p 3000:3000 -it --rm --name goals-fe --rm goals-fe:latest