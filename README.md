# Prueba Técnica

## Backend (Laravel)

### Requisitos

-   PHP
-   Composer
-   Alguna base de datos

Para SQL Server, tener instalado el driver para conectar Laravel con SQL Server y modificar el archivo `php.ini` para ahbilitarlo.

1. Para instalar el backend, deberá ejecutar el siguiente comando:

```
composer install
```

2. Hacer una copia del archivo `.env.example` y reemplazar las siguientes variables:

-   `DB_CONNECTION`: Para SQL Server agregarle `sqlsrv` después de haber instalado el driver de SQL Server para PHP.
-   `DB_HOST`: Es el host donde está alojada la base de datos.
-   `DB_PORT`: El puerto en que se expone la base de datos.
-   `DB_DATABASE`: El nombre de la base de datos.
-   `DB_USERNAME`: El nombre de usuario de la base de datos.
-   `DB_PASSWORD`: La contraseña de la base de datos.

3. Crear las migraciones ejecutando:

```
php artisan migrate
```

4. Ingresar datos iniciales a la base de datos ejecutando:

```
php artisan db:seed
```

5. Para ejecutar la aplicación:

```
php artisan serve
```

## Frontend (Angular)

### Requisitos

-   Node.js

1. Para instaar el frontend, deberá ejecutar el siguiente comando:

```
npm install
```

2. Modificar el archivo ubicado en la ruta `src/environments/environment.ts`, las propiedades `BASE_URL` y `PORT` con la IP y puerto proporcionados por la aplicación de Laravel.

3. Para ejecutar la aplicación:

```
npm start
```
