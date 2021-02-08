npm install -g @nestjs/cli
nest new nest-api
OR
npx @nestjs/cli new nest-api

cd nest-api
npm start

chmod +x .docker/entrypoint.sh

docker-compose up --build

http://localhost:9000/

docker-compose exec app bash

> npm install pg typeorm @nestjs/typeorm @nestjs/config --save

npm run typeorm entity:create -- -n product

npm run typeorm migration:create -- -n CreateProductsTable
npm run typeorm migration:run

nest generate controller controllers/product
