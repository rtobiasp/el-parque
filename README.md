# El Parque

Web estática de Bar El Parque, construida con Astro.

## Requisitos

- Node.js `>=22.12.0`
- pnpm

## Comandos

Ejecutar desde esta carpeta:

```sh
pnpm install
pnpm dev
pnpm check
pnpm build
pnpm preview
```

`pnpm build` genera la carpeta `dist/`, lista para publicar en cualquier hosting de sitios estáticos.

## Configuración de producción

Define `PUBLIC_SITE_URL` con la URL pública, sin una barra final, para activar la URL canónica de la página:

```sh
PUBLIC_SITE_URL=https://www.ejemplo.com
```

El archivo `.env.example` sirve como referencia. No subas secretos ni archivos `.env` al repositorio.

## Despliegue

1. Instala dependencias con `pnpm install --frozen-lockfile`.
2. Configura `PUBLIC_SITE_URL` en el proveedor de hosting.
3. Ejecuta `pnpm check` y `pnpm build`.
4. Publica el contenido de `dist/`.

La página principal está en `src/pages/index.astro`; los recursos públicos están en `public/`.
