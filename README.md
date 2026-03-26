# 🏠📄 Proyecto Home About

[![Django](https://img.shields.io/badge/Django-6.0.3-green.svg)](https://www.djangoproject.com/)
[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

Un proyecto web simple y elegante construido con Django que presenta páginas de inicio (Home) y acerca de (About). Perfecto para principiantes en Django o como base para proyectos más complejos.

## ✨ Características

- 🏠 **Página de Inicio**: Una página de bienvenida atractiva
- 📖 **Página Acerca De**: Información sobre el proyecto o sitio
- 🎨 **Plantillas HTML**: Diseño limpio y responsivo
- 🔗 **Navegación**: Enlaces entre páginas
- 📱 **Responsive**: Adaptable a diferentes dispositivos
- ⚡ **Rápido**: Optimizado para rendimiento

## 🚀 Instalación

Sigue estos pasos para configurar el proyecto en tu máquina local:

### Prerrequisitos

- Python 3.8 o superior
- Git

### Pasos de Instalación

1. **Clona el repositorio**
   ```bash
   git clone https://github.com/tu-usuario/home-about.git
   cd home-about
   ```

2. **Crea un entorno virtual**
   ```bash
   python -m venv .venv
   ```

3. **Activa el entorno virtual**
   - En Windows:
     ```bash
     .venv\Scripts\activate
     ```
   - En macOS/Linux:
     ```bash
     source .venv/bin/activate
     ```

4. **Instala las dependencias**
   ```bash
   pip install -r requirements.txt
   ```

5. **Realiza las migraciones de la base de datos**
   ```bash
   python manage.py migrate
   ```

6. **Ejecuta el servidor de desarrollo**
   ```bash
   python manage.py runserver
   ```

7. **Abre tu navegador y visita**
   - [http://127.0.0.1:8000/](http://127.0.0.1:8000/) - Página de Inicio
   - [http://127.0.0.1:8000/about/](http://127.0.0.1:8000/about/) - Página Acerca De

## 📁 Estructura del Proyecto

```
home_about/
├── base_project/          # Configuración principal de Django
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py        # Configuraciones del proyecto
│   ├── urls.py            # URLs principales
│   ├── wsgi.py
│   └── __pycache__/
├── pages/                 # Aplicación de páginas
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── models.py          # Modelos de datos
│   ├── tests.py           # Pruebas
│   ├── urls.py            # URLs de la app
│   ├── views.py           # Vistas (TemplateView)
│   ├── __pycache__/
│   └── migrations/        # Migraciones de base de datos
│       ├── __init__.py
│       └── __pycache__/
├── templates/             # Plantillas HTML
│   ├── _base.html         # Plantilla base
│   ├── home.html          # Página de inicio
│   └── about.html         # Página acerca de
├── db.sqlite3             # Base de datos SQLite
├── manage.py              # Script de gestión de Django
└── requirements.txt       # Dependencias del proyecto
```

## 🛠️ Tecnologías Utilizadas

- **Backend**: Django 6.0.3
- **Lenguaje**: Python 3.8+
- **Base de Datos**: SQLite (desarrollo)
- **Frontend**: HTML5, CSS3
- **Servidor**: Django Development Server

## 📋 Dependencias

- `asgiref==3.11.1` - ASGI utilities
- `Django==6.0.3` - Framework web
- `sqlparse==0.5.5` - SQL parser
- `tzdata==2025.3` - Timezone data

## 🔧 Configuración

### Variables de Entorno

Para producción, configura las siguientes variables:

- `DEBUG=False`
- `SECRET_KEY` - Una clave secreta segura
- `ALLOWED_HOSTS` - Lista de hosts permitidos

### Base de Datos

Por defecto usa SQLite. Para cambiar a PostgreSQL u otra base de datos, modifica `settings.py`.

## 🧪 Pruebas

Ejecuta las pruebas con:

```bash
python manage.py test
```

## 📦 Despliegue

Para desplegar en producción:

1. Configura un servidor web (Nginx, Apache)
2. Usa un servidor WSGI/ASGI (Gunicorn, uWSGI)
3. Configura una base de datos robusta
4. Establece variables de entorno seguras
5. Ejecuta migraciones y collectstatic

## 🤝 Contribuir

¡Las contribuciones son bienvenidas! Sigue estos pasos:

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## 📝 Licencia

Este proyecto está bajo la Licencia MIT. Ver el archivo [LICENSE](LICENSE) para más detalles.

## 👥 Autor

- **Tu Nombre** - *Desarrollador Inicial* - [tu-email@ejemplo.com](mailto:tu-email@ejemplo.com)

## 🙏 Agradecimientos

- Django Project por el excelente framework
- Comunidad de Python por el soporte continuo
- Todos los contribuidores que hacen este proyecto mejor

---

⭐ Si te gusta este proyecto, ¡dale una estrella!

📧 ¿Preguntas? [Contáctame](mailto:tu-email@ejemplo.com)