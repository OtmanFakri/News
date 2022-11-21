FROM node:alpine

WORKDIR /app/frontend
COPY package.json /app/frontend
COPY . .


RUN npm install

EXPOSE 3000

CMD ["cache","clean","--force"]

RUN chown -R root /app/frontend/node_modules

USER root


CMD ["npm", "start"]