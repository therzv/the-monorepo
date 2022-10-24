FROM node:18
 
WORKDIR /web
 
 # Copy app source
COPY . .
RUN yarn install
EXPOSE 3000
CMD ["yarn", "run", "dev"]
