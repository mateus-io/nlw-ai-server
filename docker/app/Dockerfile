FROM node:18.16.1-alpine
RUN corepack enable

WORKDIR /home/node/app

COPY . ./

RUN pnpm install

EXPOSE 3333

CMD [ "pnpm", "run", "dev" ]