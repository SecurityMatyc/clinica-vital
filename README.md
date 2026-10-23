# Clínica Vital Service

Aplicación web académica para gestionar información clínica mediante Django, operaciones CRUD, API REST y documentación interactiva.

Proyecto desarrollado en **2025** para la **Evaluación 2 de Backend**.

## Estado del proyecto

Implementación académica introductoria orientada a demostrar fundamentos de desarrollo backend con Django, modelado relacional y exposición de datos mediante una API REST.

La versión disponible utiliza SQLite para facilitar la ejecución local y la revisión del proyecto.

## Objetivo

Clínica Vital representa un flujo básico de gestión de información médica. Su propósito es organizar entidades clínicas relacionadas y permitir su administración desde una interfaz web y endpoints REST.

El proyecto se centra en demostrar:

- Creación de modelos relacionales.
- Uso de formularios Django.
- Operaciones CRUD.
- Organización de vistas y rutas.
- Serialización de datos.
- Documentación de una API.

## Autor

- Matías Gajardo

Proyecto desarrollado individualmente como parte del proceso formativo en desarrollo backend con Django.

## Entidades gestionadas

- Especialidades médicas.
- Médicos.
- Pacientes.
- Consultas médicas.
- Tratamientos.
- Medicamentos.
- Recetas médicas.

## Funcionalidades principales

- Operaciones CRUD desde la interfaz web.
- Formularios basados en `ModelForm`.
- Vistas basadas en funciones para listado, creación, edición y eliminación.
- API REST por entidad mediante `ModelViewSet`.
- Enrutamiento automático con `DefaultRouter`.
- Documentación de API mediante Swagger y ReDoc.
- Organización de una aplicación Django orientada a la gestión de datos clínicos.

## Estructura del proyecto

- `clinica_vital`: configuración principal del proyecto Django.
- `gestion`: aplicación principal con modelos, formularios, vistas, serializadores y rutas.
- `gestion/templates/gestion`: plantillas para el menú y las vistas CRUD.

## Tecnologías

- Python 3.13
- Django 6.0.3
- Django REST Framework
- drf-yasg
- HTML, CSS y plantillas Django
- SQLite para ejecución local
- PostgreSQL utilizado en una etapa previa del proyecto

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

Este proyecto tiene un alcance introductorio. No corresponde a un sistema clínico listo para producción ni gestiona procesos como autenticación avanzada, agenda médica, fichas clínicas completas, auditoría de cambios, permisos por profesional o protección especializada de datos sensibles.

## Consideraciones para una evolución futura

- Incorporar autenticación y autorización por perfiles.
- Añadir validaciones específicas para datos clínicos.
- Implementar agenda y disponibilidad de profesionales.
- Registrar historial y auditoría de cambios.
- Reforzar la protección de información personal.
- Incorporar pruebas automatizadas.
- Configurar una base de datos y despliegue orientados a producción.

## Contexto académico

Este repositorio conserva una entrega formativa orientada al aprendizaje de fundamentos de desarrollo web con Django, modelado relacional, operaciones CRUD, organización de aplicaciones y consumo o exposición de servicios REST.
