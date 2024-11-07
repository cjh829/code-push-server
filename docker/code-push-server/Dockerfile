FROM node:12.18.3-alpine

RUN npm i -g code-push-server@5.7.1 pm2@4.4.1 --no-optional

COPY ./process.json /process.json

EXPOSE 3000

CMD ["pm2-docker", "start", "/process.json"]
