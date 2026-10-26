# Laboratorio DevOps

Laboratorio integrado de Desarrollo Web (26 de octubre de 2026): Docker, Kubernetes, GitHub Actions y CI/CD.

## Estructura

- `site/index.html`: página web que publica GitHub Pages.
- `Dockerfile`: imagen de Nginx que sirve la página.
- `.github/workflows/ci-cd.yml`: validación, prueba con Docker y publicación en GitHub Pages.

## Integrante

Daniel Samayoa · 5090-23-9260.

## Ejecución automática

Cada `push` a `main` ejecuta el workflow `Laboratorio CI-CD`. También puede iniciarse manualmente mediante `workflow_dispatch`.

Para activar el despliegue, configurar `Settings → Pages → Build and deployment → Source → GitHub Actions`.

**Nota:** GitHub Pages publica el HTML estático. La imagen Docker se construye y prueba en el runner de GitHub Actions; no se ejecuta como contenedor en GitHub Pages.
