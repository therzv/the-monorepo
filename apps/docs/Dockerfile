FROM node:18
 
WORKDIR /docs
 
 # Copy app source
COPY . .
RUN yarn install
EXPOSE 3001
CMD ["yarn", "run", "dev"]
