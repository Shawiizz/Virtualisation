FROM debian:12

RUN apt-get update && apt-get install -y \
    nodejs \
    npm

COPY sources/12 /app

WORKDIR /app

RUN npm install

RUN npm run build

EXPOSE 3000

CMD ["npm", "start"]