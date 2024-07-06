# Blog Project

Este es un proyecto de blog simple desarrollado con Django, siguiendo una arquitectura monolítica. El proyecto demuestra las funcionalidades básicas de un blog con sistema de autenticación.

## Características

- Listado de posts
- Visualización de posts individuales
- Creación de nuevos posts (requiere autenticación)
- Sistema de autenticación (login/logout)

## Requisitos

- Python 3.8+
- Django 3.2+

## Instalación

1. Clona este repositorio:

```
git clone https://github.com/tu-usuario/blog_project.git
cd blog_project
```
2. Crea un entorno virtual y actívalo:
```
python -m venv venv
source venv/bin/activate  # En Windows usa venv\Scripts\activate
```
3. Instala las dependencias:
```
pip install -r requirements.txt
```
4. Realiza las migraciones:
```
python manage.py migrate
```
5. Crea un superusuario:
```
python manage.py createsuperuser
```
6. Inicia el servidor de desarrollo:
```
python manage.py runserver
```
## Uso

- Accede a `http://localhost:8000` para ver la lista de posts
- Inicia sesión en `http://localhost:8000/login/`
- Crea nuevos posts desde la página principal cuando estés autenticado
- Cierra sesión usando el enlace "Logout" en la página principal

## Estructura del Proyecto
```
blog_project/
│
├── blog/
│   ├── templates/
│   │   └── blog/
│   │       ├── post_list.html
│   │       ├── post_detail.html
│   │       ├── post_form.html
│   │       └── login.html
│   ├── models.py
│   ├── views.py
│   └── urls.py
│
├── blog_project/
│   ├── settings.py
│   └── urls.py
│
├── manage.py
└── README.md
```
## Arquitectura

Este proyecto sigue una arquitectura monolítica, lo que significa que todas las funcionalidades están integradas en una sola aplicación. Esta arquitectura fue elegida por su simplicidad y facilidad de desarrollo para proyectos pequeños a medianos.

### Ventajas de la arquitectura monolítica en este proyecto:

- Desarrollo rápido y sencillo
- Fácil de desplegar y mantener para proyectos pequeños
- Adecuado para equipos pequeños o desarrolladores individuales

## Próximos pasos

Algunas mejoras que se podrían implementar en el futuro:

1. Añadir sistema de comentarios en los posts
2. Implementar categorías o etiquetas para los posts
3. Mejorar el diseño con CSS (posiblemente usando Bootstrap)
4. Añadir funcionalidad de búsqueda de posts
5. Implementar un sistema de usuarios más robusto (registro, perfiles, etc.)

## Contribuir

Si quieres contribuir a este proyecto, por favor:

1. Haz un Fork del repositorio
2. Crea una nueva rama (`git checkout -b feature/AmazingFeature`)
3. Haz commit de tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Haz Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## Licencia

Distribuido bajo la licencia MIT. Ver `LICENSE` para más información.

## Contacto

Tu Nombre - [@tu_twitter](https://twitter.com/tu_twitter) - email@example.com

Link del Proyecto: [https://github.com/tu-usuario/blog_project](https://github.com/tu-usuario/blog_project)