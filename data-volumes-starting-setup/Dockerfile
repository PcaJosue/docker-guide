FROM node:14

ARG DEFAULT_PORT=80

WORKDIR /app

COPY package.json /app

RUN npm install

COPY . .

ENV PORT $DEFAULT_PORT
#ENV PORT 80
## WE COULD USE A FILE

EXPOSE $PORT

VOLUME ["/app/feedback"]

CMD ["npm" , "start"]
