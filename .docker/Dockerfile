FROM node:16.20.2-alpine AS build-stage

WORKDIR /app

COPY Angular6/package.json Angular6/package-lock.json ./

RUN npm install

COPY ../Angular6 .

RUN npm run build-prod

FROM nginx:alpine AS production-stage

COPY ../.docker/nginx.conf /etc/nginx/nginx.conf

COPY --from=build-stage /app/dist/ /usr/share/nginx/html

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]