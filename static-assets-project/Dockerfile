#build stage
FROM node:12-alpine AS build

WORKDIR /code
COPY . .
RUN npm ci
RUN npm run build

#runtime stage
FROM nginx:1.17

COPY --from=build /code/build /usr/share/nginx/html
