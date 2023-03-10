## Proyecto: Taxi24

### Antes de comenzar...
Es necesario que instale docker y docker desktop en su computador para poder ejecutar las migraciones y correr la base de datos. [Docker](https://docs.docker.com/desktop/install/windows-install/)

### Instalacion
1. Clone el proyecto. ```git clone https://github.com/keven-correa/taxi24-api.git ```
   
2. Teniendo clonado el proyecto, abra una terminal e instale todas las dependencias del proyecto ejecutando: ```npm install```.
   
3. Instale el ORM ```npm install prisma --save -dev``` seguido de ``` npm install @prisma/client```; este ultimo para poder visualizar el esquema de entidades dentro del proyecto.
   
4. Dentro del archivo ```docker-compose.yml``` encontrara la configuracion de la base de datos a utilizar.
   
5. Ejecutar docker con el comando ```docker-compose up``` para levantar el contenedor de la base de datos.
   
6. Descargue el archivo ```Taxi24.postman_collection``` o copie su contenido, que esta en la raiz del proyecto y importelo en Postman para poder hacer las pruebas de los diferentes endpoints solicitados.
   
7. Ejecute el comando para crear la base de datos y sus tablas: ```npx prisma migrate dev```
   
### Ejecutar el proyecto
Para ejecutar el proyecto ejecute el comando: ``` npm run start:dev ```


### Notas importantes
   
1. El archivo con las sentencias SQL para la creacion de las tablas esta situado en la raiz del proyecto llamado: ```taxi_database.sql```

## Tecnologias que se utilizaron para este proyecto
- [NestJS](https://nestjs.com)
- Base de datos: [PostgreSQL](https://www.postgresql.org) y [Docker](https://www.docker.com/)
- ORM para manipular y acceder a los datos: [Prisma](https://www.prisma.io)