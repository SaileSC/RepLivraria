# Estágio de construção da aplicação
FROM node AS build

WORKDIR /appbuild

COPY package.json .
COPY package-lock.json .
COPY tsconfig.json .
COPY ./src ./src

RUN npm install
RUN npm run build

# Estágio de execução da aplicação
FROM node

WORKDIR /app

COPY package.json ./
COPY package-lock.json ./
COPY .env .
COPY ./public ./public
COPY --from=build /appbuild/dist ./dist

RUN npm install --production

EXPOSE 4444

CMD npm start
