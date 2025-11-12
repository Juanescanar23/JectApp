# Jectapp

Aplicación Angular (CLI 1.7.3) utilizada en el curso de Udemy para demostrar módulos, rutas, componentes y consumo de servicios en tiempo real con Socket.IO.

## Requisitos previos

- Node.js 8.x (LTS recomendado) y npm 5.x  
- [Angular CLI 1.7.3](https://github.com/angular/angular-cli/releases/tag/v1.7.3) instalada de forma global (`npm install -g @angular/cli@1.7.3`)  
- Google Chrome o un navegador compatible para las pruebas E2E con Protractor

## Instalación

1. Clona el proyecto o descarga el ZIP del curso.  
2. Instala las dependencias desde la raíz del proyecto:

   ```bash
   npm install
   ```

3. Configura variables o servicios externos (por ejemplo, endpoints de sockets) dentro de `src/environments/*.ts` si tu despliegue lo requiere.

## Ejecución en desarrollo

Lanza el servidor con:

```bash
npm start
```

Angular CLI abrirá `http://localhost:4200/` y recargará automáticamente al guardar cambios en `src`.

### Generar nuevos artefactos

Usa los comandos del CLI para crear componentes, servicios u otros artefactos:

```bash
ng generate component my-component
ng generate service core/socket
```

Consulta `ng g --help` para ver todas las opciones disponibles.

## Build de producción

```bash
npm run build
```

Los archivos optimizados quedarán en `dist/`. Para desplegar en producción agrega `--prod` (`npm run build -- --prod`) y sirve el contenido generado con el servidor de tu preferencia.

## Pruebas y lint

- **Unitarias:** `npm test` (Karma + Jasmine). Se ejecutan en modo watch por defecto.  
- **End-to-end:** `npm run e2e` (Protractor). Requiere que `npm start` esté corriendo o que expongas una URL previamente desplegada.  
- **Lint:** `npm run lint` aplica las reglas definidas en `tslint.json`.

## Ayuda adicional

Para más comandos revisa `ng help` o la [documentación oficial de Angular CLI](https://github.com/angular/angular-cli/blob/master/README.md).
