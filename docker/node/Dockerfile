FROM node:12.21.0

RUN rm /bin/sh && ln -s /bin/bash /bin/sh

USER node

WORKDIR /home/node/app

EXPOSE 3000

ENTRYPOINT [ "docker-entrypoint.sh" ]

CMD yarn install && yarn dev --host 0.0.0.0