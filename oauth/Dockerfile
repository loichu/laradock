ARG VERSION
ARG PORT

FROM node:$VERSION
MAINTAINER loic.humbert@epfl.ch

RUN mkdir /opt/fake-oauth2-server
WORKDIR /opt/fake-oauth2-server
ADD server.js server.js
ADD input.html input.html
ADD app.js app.js
ADD node_modules node_modules
EXPOSE $PORT
ENTRYPOINT ["node" , "/opt/fake-oauth2-server/server.js" ]
