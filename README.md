# Notas de troubleshooting en Azure

[![Publicación](https://github.com/ygallardops/devops-notes/actions/workflows/deploy.yml/badge.svg)](https://github.com/ygallardops/devops-notes/actions/workflows/deploy.yml)
[![Licencia MIT](https://img.shields.io/github/license/ygallardops/devops-notes)](LICENSE)
[![Material for MkDocs](https://img.shields.io/badge/Material_for_MkDocs-526CFE?logo=MaterialForMkDocs&logoColor=white)](https://squidfunk.github.io/mkdocs-material/)

> **Notas de estudio, no un entregable profesional.** Apuntes que recopilé mientras trabajaba en soporte y operación de infraestructura. Los mantengo en público como consulta personal.

**Leer en línea:** [ygallardops.github.io/devops-notes](https://ygallardops.github.io/devops-notes/), con buscador y modo oscuro.

## Qué hay aquí

| Tema | Nota |
| --- | --- |
| Azure · AKS | [Diagnóstico de pods](docs/azure/aks/troubleshooting-pods.md) |

Por ahora es solo eso. Prefiero listar lo que existe antes que anunciar secciones vacías.

## Verlo en local

```bash
git clone https://github.com/ygallardops/devops-notes.git
cd devops-notes
pip install -r requirements.txt
mkdocs serve
```

El sitio queda en `http://127.0.0.1:8000` y se recarga al editar cualquier archivo de `docs/`.

## Publicación

Cada push a `main` ejecuta [`deploy.yml`](.github/workflows/deploy.yml): instala las dependencias, construye el sitio con MkDocs y lo publica en GitHub Pages.

## Licencia

[MIT](LICENSE)
