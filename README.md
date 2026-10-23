# Clínica Vital Service

Aplicación web académica para la gestión de información clínica mediante Django, operaciones CRUD, API REST y documentación interactiva.

Proyecto desarrollado en **2025** para la **Evaluación 2 de Backend**.

## Autor

- Matías Gajardo

Proyecto desarrollado individualmente como parte del proceso formativo en desarrollo backend con Django.

## Descripción del proyecto

Clínica Vital permite administrar información básica de un flujo médico mediante modelos relacionales, formularios, vistas web y endpoints REST.

El sistema gestiona las siguientes entidades:

- Especialidades médicas.
- Médicos.
- Pacientes.
- Consultas médicas.
- Tratamientos.
- Medicamentos.
- Recetas médicas.

También incorpora documentación automática de la API mediante Swagger y ReDoc.

## Características principales

- Operaciones CRUD desde la interfaz web.
- Formularios basados en `ModelForm`.
- Vistas basadas en funciones para listado, creación, edición y eliminación.
- API REST por entidad mediante `ModelViewSet` y `DefaultRouter`.
- Documentación de API disponible en Swagger y ReDoc.
- Organización de una aplicación Django orientada a la gestión de datos clínicos.

## Tecnologías

- Python 3.13
- Django 6.0.3
- Django REST Framework
- drf-yasg
- HTML, CSS y plantillas Django
- SQLite para ejecución local
- PostgreSQL utilizado en una etapa previa del proyecto

## Estructura del proyecto

- `clinica_vital`: configuración principal del proyecto Django.
- `gestion`: aplicación principal con modelos, formularios, vistas, serializadores y rutas.
- `gestion/templates/gestion`: plantillas para el menú y las vistas CRUD.

## Puesta en marcha local

### 1. Clonar el repositorio

```powershell
git clone <url-del-repositorio>
cd Clinica-Vital
```

### 2. Crear y activar el entorno virtual

```powershell
python -m venv env
.\env\Scripts\Activate.ps1
```

### 3. Instalar dependencias

```powershell
pip install -r requirements.txt
```

### 4. Aplicar migraciones

```powershell
python manage.py migrate
```

### 5. Iniciar el servidor

```powershell
python manage.py runserver
```

## Rutas principales

| Ruta | Descripción |
|------|-------------|
| `http://127.0.0.1:8000/` | Menú principal |
| `http://127.0.0.1:8000/admin/` | Panel de administración Django |
| `http://127.0.0.1:8000/gestion/api/` | Endpoints REST |
| `http://127.0.0.1:8000/swagger/` | Documentación Swagger |
| `http://127.0.0.1:8000/redoc/` | Documentación ReDoc |

## Base de datos y alcance

Durante el desarrollo se trabajó con PostgreSQL en una etapa previa. La versión disponible en este repositorio utiliza **SQLite por defecto** para facilitar la ejecución local y la revisión académica.

## Contexto académico

Este repositorio conserva una entrega formativa orientada al aprendizaje de fundamentos de desarrollo web con Django, modelado relacional, operaciones CRUD, organización de aplicaciones y consumo básico de API REST.
