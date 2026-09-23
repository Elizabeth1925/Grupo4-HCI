# Proyecto HCI - Grupo 4

## Requisitos
- PHP 8.0.x (XAMPP)
- Composer
- MySQL

## Configuración del Entorno (T02)
1. Clonar el repositorio.
2. Ejecutar `composer install`.
3. Copiar `.env.example` a `.env`.
4. Ejecutar `php artisan key:generate`.

## Base de Datos (T03)
1. Abre tu panel de control de XAMPP e inicia los módulos **Apache** y **MySQL**.
2. Ve a phpMyAdmin (http://localhost/phpmyadmin) y crea una base de datos vacía llamada `grupo4_hci`.
3. Asegúrate de que las variables en el archivo `.env` estén configuradas de la siguiente manera:
   ```env
   DB_CONNECTION=mysql
   DB_HOST=127.0.0.1
   DB_PORT=3306
   DB_DATABASE=grupo4_hci
   DB_USERNAME=root
   DB_PASSWORD=
   ```
4. Ejecutar las migraciones con `php artisan migrate`.

## Ejecución del proyecto
Para levantar el servidor de desarrollo, ejecuta:
```bash
php artisan serve
```
El proyecto estará disponible en `http://localhost:8000`.
