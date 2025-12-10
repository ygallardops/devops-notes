# Documentación de DevOps con MkDocs

![CI/CD](https://github.com/ygallardops/devops-notes/actions/workflows/deploy.yml/badge.svg)
![License](https://img.shields.io/github/license/ygallardops/devops-notes)
![MkDocs](https://img.shields.io/badge/Material_for_MkDocs-526CFE?style=flat&logo=MaterialForMkDocs&logoColor=white)

Este repositorio contiene una colección de notas, guías y documentación técnica sobre herramientas y prácticas de DevOps. El sitio se genera utilizando **MkDocs** junto con el tema **Material for MkDocs**, permitiendo una documentación limpia, modular y fácilmente navegable.

## Ver Documentación Online

El sitio web completo, con buscador y modo oscuro, está disponible aquí:

 **[https://ygallardops.github.io/devops-notes/](https://ygallardops.github.io/devops-notes/)**

---

## Características

- **Documentación Modular:** Todo el contenido se organiza dentro de la carpeta `docs/` utilizando Markdown.
- **Tema Profesional:** Uso del tema Material for MkDocs, con navegación lateral, búsqueda integrada y estilos modernos.
- **Despliegue Automatizado:** GitHub Actions genera y publica el sitio automáticamente en GitHub Pages.
- **Configuración Extensible:** Soporte para extensiones como `pymdown-extensions`, resaltado de sintaxis y navegación avanzada.
- **Desarrollo Local Sencillo:** MkDocs incluye un servidor local de auto-recarga para edición en tiempo real.

## Estructura del Repositorio

    .
    ├── mkdocs.yml               # Configuración principal del sitio
    ├── requirements.txt         # Dependencias necesarias para MkDocs
    ├── docs/
    │   ├── index.md             # Página principal
    │   └── ...                  # 
    └── .github/
        └── workflows/
            └── deploy.yml       # Pipeline para GitHub Pages

## Uso

### 1. Clonar el repositorio

``` bash
git clone https://github.com/ygallardops/devops-notes.git
cd devops-notes
```

### 2. Instalar dependencias

``` bash
pip install -r requirements.txt
```

### 3. Levantar el servidor de desarrollo

``` bash
mkdocs serve
```

El sitio estará disponible en:

    http://127.0.0.1:8000

## Despliegue Automático (CI/CD)

Este repositorio utiliza GitHub Actions para compilar y desplegar el
sitio.  
Cada push a la rama `main` ejecuta el workflow `deploy.yml`, el cual:

1.  Instala las dependencias definidas en `requirements.txt`.
2.  Construye el sitio usando `mkdocs build`.
3.  Publica automáticamente los artefactos en GitHub Pages.

## Archivos Principales

| Archivo                        | Descripción                                                     |
|--------------------------------|-----------------------------------------------------------------|
| `mkdocs.yml`                   | Configuración global del sitio (tema, navegación, extensiones). |
| `requirements.txt`             | Dependencias necesarias para MkDocs y el tema Material.         |
| `.github/workflows/deploy.yml` | Pipeline para CI/CD utilizando GitHub Actions.                  |
| `docs/index.md`                | Página de inicio del sitio.                                     |
| `README.md`                    | Información general del repositorio.                            |

## Licencia

MIT

