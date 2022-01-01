FROM node
#init a dir to copy project to
WORKDIR /app
COPY package.json package-lock.json ./
#installing requirements
RUN npm install
COPY . .
#specifying port num inide container
EXPOSE 4200
#launch client side, binding it to the host ip, in order to open it in the host OS browser
CMD [ "npm","start", "--", "--host", "0.0.0.0"]