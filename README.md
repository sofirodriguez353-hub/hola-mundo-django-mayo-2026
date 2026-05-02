# Hola Mundo Django

Este proyecto es una aplicación Django mínima que sirve una página de bienvenida estática.
Está diseñado como un punto de partida ligero para aprender Django o para ampliar con nuevas vistas, modelos y rutas.

---

## 📁 Estructura del proyecto

- `manage.py` - punto de entrada para comandos de Django.
- `db.sqlite3` - base de datos SQLite local utilizada por defecto.
- `requirements.txt` - dependencias del proyecto.
- `base_project/` - configuración del proyecto Django.
  - `settings.py` - configuración principal.
  - `urls.py` - enrutamiento global.
  - `wsgi.py` / `asgi.py` - puntos de entrada para despliegue.
- `pages/` - app Django principal.
  - `views.py` - vista basada en clase para la página de inicio.
  - `urls.py` - rutas específicas de la app.
- `templates/` - carpeta de plantillas compartidas.
  - `index.html` - plantilla principal renderizada en la ruta raíz.

---

## 🚀 Características principales

- Aplicación Django con una sola app llamada `pages`.
- Ruta raíz (`/`) que muestra una página simple de bienvenida.
- Uso de `TemplateView` para renderizar `templates/index.html`.
- Base de datos SQLite preconfigurada para desarrollo rápido.

---

## 🧰 Requisitos

- Python 3.11 (o una versión compatible con Django 6.0)
- Django 6.0.4
- SQLite (incluido con Python, no requiere instalación adicional)

> El archivo `requirements.txt` contiene las dependencias necesarias para este proyecto.

---

## ⚙️ Instalación y ejecución

1. Clonar o descargar el repositorio.

2. Crear y activar un entorno virtual:

```bash
python -m venv .venv
.\.venv\Scripts\activate
```

3. Instalar las dependencias:

```bash
pip install -r requirements.txt
```

4. Ejecutar migraciones:

```bash
python manage.py migrate
```

5. Iniciar el servidor de desarrollo:

```bash
python manage.py runserver
```

6. Abrir el navegador en:

```text
http://127.0.0.1:8000/
```

---

## 🧪 Pruebas y administración

- Para crear un superusuario de administración:

```bash
python manage.py createsuperuser
```

- La interfaz de administración estará disponible en:

```text
http://127.0.0.1:8000/admin/
```

---

## 📝 Personalización rápida

- Añadir nuevas rutas: editar `base_project/urls.py` o `pages/urls.py`.
- Añadir nuevas vistas: crear nuevas clases o funciones en `pages/views.py`.
- Añadir plantillas: crear archivos HTML dentro de `templates/` y referenciarlos desde las vistas.

---

## 🌟 Notas finales

Este proyecto es ideal para:

- Aprender la estructura básica de un proyecto Django.
- Probar nuevas funcionalidades en una aplicación ligera.
- Usar como plantilla inicial para un sitio web más completo.

¡Disfruta desarrollando con Django! 😊
