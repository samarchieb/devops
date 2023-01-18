FROM node:latest as node
# set working directory
WORKDIR /app

COPY . .
RUN npm install --save --legacy-peer-deps
RUN npm run build --prod

EXPOSE 4200


CMD ["ng", "serve","--host","0.0.0.0","--port","4200"]
