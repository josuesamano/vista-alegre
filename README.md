# Reglamento de Vista Alegre

Sitio estático en Astro con el reglamento del Fraccionamiento Vista Alegre y el PDF original. El texto está en `src/content/reglamento.json` y los archivos públicos están en `public/`.

## Vista previa local

Con Node.js 24 o posterior, ejecuta estos comandos en la carpeta que contiene `package.json`.

```sh
npm ci
npm run dev
```

Abre la dirección local que muestra Astro. Para comprobar la versión de producción, usa `npm run build` y luego `npm run preview`.

## Publicar en GitHub Pages

1. Extrae el ZIP y sube el contenido de la carpeta `vista-alegre` a la raíz de un repositorio de GitHub, incluida la carpeta `.github`.
2. En el repositorio, abre **Settings → Pages** y selecciona **GitHub Actions** como **Source**.
3. Sube los cambios a la rama `main` o ejecuta **Publicar en GitHub Pages** desde **Actions**. Si la rama principal tiene otro nombre, actualízala en `.github/workflows/deploy.yml`.
4. Al terminar el flujo, abre la dirección que aparece en el resultado del despliegue.

El flujo lee la URL y la ruta base desde GitHub Pages, tanto para sitios en la raíz del dominio como para sitios bajo el nombre del repositorio.

[Guía oficial de Astro para GitHub Pages](https://docs.astro.build/en/guides/deploy/github/)
