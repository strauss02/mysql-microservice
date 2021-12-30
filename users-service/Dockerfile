FROM node:16

ADD . /app

COPY ./wait-for-it.sh /wait-for-it.sh

RUN cd /app; \
  npm install --production

RUN chmod +x wait-for-it.sh

EXPOSE 8123 

CMD [ "node", "/app/index.js" ]