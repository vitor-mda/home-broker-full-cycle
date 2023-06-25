FROM node:20.3-alpine3.18

RUN npm install -g @nestjs/cli

USER node

WORKDIR /home/node/app

COPY package*.json .

CMD npm ci && npm run build && npx prisma generate && npm start
