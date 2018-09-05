FROM node
RUN apt-get update -q && apt-get dist-upgrade -y && apt-get clean && apt-get autoclean
EXPOSE 3000
ENV APP_PATH /usr/share/app
WORKDIR $APP_PATH
USER node
COPY . $APP_PATH
CMD ["npm", "start"]