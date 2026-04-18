# 🏢 Sistema de Gestión de Condominios

<p align="center">
  <img src="https://img.shields.io/badge/Estado-Activo-success?style=for-the-badge">
  <img src="https://img.shields.io/badge/Laravel-5-FF2D20?style=for-the-badge&logo=laravel&logoColor=white">
  <img src="https://img.shields.io/badge/PHP-7.0-777BB4?style=for-the-badge&logo=php&logoColor=white">
  <img src="https://img.shields.io/badge/Licencia-MIT-yellow?style=for-the-badge">
</p>

<p align="center">
  <img src="https://img.shields.io/badge/MySQL-Database-4479A1?style=for-the-badge&logo=mysql&logoColor=white">
  <img src="https://img.shields.io/badge/Node.js-Frontend-339933?style=for-the-badge&logo=node.js&logoColor=white">
  <img src="https://img.shields.io/badge/Composer-Dependency-885630?style=for-the-badge&logo=composer&logoColor=white">
</p>

---

## 🏥 Descripción

Sistema web desarrollado para la **gestión de condominios**, permitiendo administrar torres, departamentos, administradores y configuraciones iniciales de manera eficiente.

Construido con **Laravel 5**, este sistema ofrece una base sólida para la administración de conjuntos residenciales.

---

## 🚀 Características

- Gestión de torres  
- Administración de departamentos  
- Registro de administradores  
- Configuración inicial del sistema  
- Arquitectura basada en Laravel (MVC)  
- Base de datos relacional  

---

## 🛠️ Requisitos del Sistema

- Sistema operativo: Linux / Windows  
- PHP 7.0  
- Composer 1.7.*  
- Node.js v8.*  
- MySQL / MariaDB v10.3.*  
- phpMyAdmin  
- Laravel 5  

---

## ⚙️ Instalación

### 1. Clonar el proyecto
```bash
git clone https://github.com/isairey/Sistema-Gestion-Condominios.git
```
cd gestion-condominios
2. Instalar dependencias
```
composer install
```
3. Configurar base de datos

Crear una base de datos en MySQL/MariaDB con el nombre:
```
gestion_condominios
```
Editar el archivo .env:
```
DB_DATABASE=gestion_condominios
DB_USERNAME=tu_usuario
DB_PASSWORD=tu_password
```
4. Ejecutar migraciones y seeders
```
php artisan migrate --seed
```
6. Iniciar el servidor
```
php artisan serve
```
Abrir en el navegador:
```
http://localhost:8000
```
## 🧭 Rutas Principales

Las rutas del sistema se encuentran en:
```
/routes/web.php
```
## 🔧 Configuración inicial
```
Route::get('admin/config/towers', ['as' => 'configTowersInitial', 'uses' => 'AdminConfigInitialController@index']);
Route::post('registerTowers', ['as' => 'registerTowers', 'uses' => 'AdminConfigInitialController@storeTowers']);

Route::get('admin/config/apartment-admin', ['as' => 'apartAdmin', 'uses' => 'AdminConfigInitialController@apartAdmin']);
Route::post('registerApartAdmin', ['as' => 'registerApartAdmin', 'uses' => 'AdminConfigInitialController@registerApartAdmin']);
```
## 📂 Estructura del Proyecto
```
/project-root
│── /app
│── /resources
│── /routes
│── /database
│── /public
│── artisan
```
## 🚀 Estado del Proyecto
✅ Funcional
✅ Configuración básica completa
⚠️ En desarrollo continuo
```
localhost:8000/register
```
Para obtener la primera vista del proceso de configuración del sistema.
