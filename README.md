<p align="center">
  <a href="" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" /></a>
</p>

# Ejecutar en desarrollo

1. Clonar el repositorio
2. Ejecutar
```
yarn install
```
3. Nest CLI instalado
```
npm i -g @nestjs/cli
```
4. Levantar base de datos
```
docker-compose up -d
```

5. Clonar el archivo __.env.template__ y renombrar la copia a __.env__


6. Llenar las variables de entorno definidas en el __.env__


7. Ejecutar la app en dev con yarn start:dev


8. Reconstruir la base de datos con la semilla
```
http://localhost:3000/api/seed
```


## Stack usado
* MongoDB
* Nest

# Production Build

1. Crear el archivo ```.env.prod```
2. Llenar las variables de entorno de prod
3. Construir la imagen 
```
docker-compose -f docker-compose.prod.yaml --env-file .env.prod up --build
```