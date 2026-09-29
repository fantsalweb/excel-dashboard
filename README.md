# Excel Dashboard

Excel Dashboard es una aplicación web que permite transformar archivos Excel en datos estructurados, normalizados y reutilizables para su posterior análisis, filtrado, visualización y generación de informes.

El sistema se centra en separar el formato original del archivo Excel de las funcionalidades de análisis, generando un **Dataset interno normalizado** que actúa como contrato estable entre la importación de datos y el resto de la aplicación.

## Objetivo

- Cargar archivos Excel (`.xlsx`)
- Seleccionar hojas y definir la zona de datos de cada tabla
- Detectar y configurar tipos de datos
- Aplicar transformaciones controladas
- Validar los datos
- Generar un Dataset normalizado
- Visualizar, filtrar, ordenar y analizar los datos
- Crear gráficos, dashboards e informes

## Stack tecnológico

- **Backend:** Laravel 13
- **Frontend:** React + Inertia.js
- **Estilos:** Tailwind CSS
- **Base de datos:** MySQL
- **Procesamiento Excel:** PhpSpreadsheet (previsto)

## Estado actual

Proyecto en fase inicial de desarrollo.

Se ha configurado la base del stack (Laravel + Inertia + React) y se está preparando la arquitectura para el flujo de importación y normalización de datos.

## Instalación

```bash
# Clonar el repositorio
git clone https://github.com/fantsalweb/excel-dashboard.git
cd excel-dashboard

# Instalar dependencias de PHP
composer install

# Instalar dependencias de Node
npm install

# Configurar entorno
cp .env.example .env
php artisan key:generate

# Configurar base de datos en el archivo .env
# Luego ejecutar migraciones
php artisan migrate

# Compilar assets
npm run build

# En otra terminal
npm run dev

# Arrancar el servidor
php artisan serve
