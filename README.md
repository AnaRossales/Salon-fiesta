# Sistema de Gestión de Salón de Fiestas 

Este proyecto consiste en una aplicación web robusta desarrollada con el framework **Django**, diseñada para digitalizar la administración de un salón de eventos, permitiendo el control de reservaciones, usuarios y catálogos.

## Instalación y Configuración Local
Sigue estos pasos para replicar el entorno en tu computadora:

### 1. Clonar el proyecto
```bash
git clone [[https://github.com/FrancoLoera/DW-PIA.git](https://github.com/FrancoLoera/DW-PIA.git](https://github.com/AnaRossales/Salon-fiesta.git))
cd DW-PIA
```

### 2. Configurar el Entorno Virtual
Dentro del entorno
```bash
python -m venv env

# Activar en Windows (CMD)
env\Scripts\activate

# Activar en Windows (PowerShell)
.\env\Scripts\activate
```

### 3. Instalar Dependencias
```bash
pip install django django-extensions Pillow
```

### 4. Preparar la Base de Datos

Aplica las migraciones para crear las tablas necesarias:

```bash
python manage.py makemigrations
python manage.py migrate
```
### 5. Crear acceso de Administrador
Para gestionar el contenido desde el panel /admin:
```bash
python manage.py createsuperuser
```


Para iniciar el servidor de desarrollo, ejecuta:

```bash
python manage.py runserver
```

Luego, abre tu navegador en: http://127.0.0.1:8000/

 Estructura del Proyecto
-salon_fiestas/: Carpeta de configuración global (settings, urls, wsgi).

-apps/: Contiene la lógica dividida por módulos (Usuarios, Reservaciones, Salones).

-templates/: Archivos HTML con sintaxis de Django.

-static/: Archivos CSS, JavaScript e imágenes de diseño.
