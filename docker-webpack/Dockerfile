FROM node:6.11.2-slim
MAINTAINER Ayhan Kuru <ayhankuru@yandex.com.tr>


RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app


COPY package.json /usr/src/app/
RUN yarn install


COPY . /usr/src/app

ENV NODE_ENV=production
ENV PORT=4000

EXPOSE 4000

CMD ["yarn", "start"]