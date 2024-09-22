# Product Microservice

## Dev

1. Clonar repositorio.
2. Instalar dependencias:

```bash
$ npm install
```

3. Crear un archivo `.env` basado en el `.env.template`

4. Ejecutar migraciones de prisma:

```
npx prisma migrate dev
```

5. Levantar aplicación:

```bash
# development
$ npm run start

# watch mode
$ npm run start:dev

# production mode
$ npm run start:prod
```

## Test

```bash
# unit tests
$ npm run test

# e2e tests
$ npm run test:e2e

# test coverage
$ npm run test:cov
```

## Generate migration Prisma:

```
npx prisma generate
```

### Generate migration prisma ORM:

```
npx prisma migrate dev --name init
```

## PROD

Ejecutar:

```
 docker build -f Dockerfile.prod -t client-gateway .
```
