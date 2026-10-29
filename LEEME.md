# Laboratorio de seguridad — proyecto Android

Este proyecto envuelve el archivo HTML educativo en una aplicación Android usando WebView.
El contenido HTML original se conserva en `app/src/main/assets/index.html`.

## Compilar APK desde GitHub usando el teléfono

1. Descomprime este ZIP.
2. Sube todos los archivos y carpetas del proyecto a un repositorio de GitHub. Debe quedar `.github/workflows/CONSTRUIR.yml` en esa ruta exacta.
3. En GitHub, abre la pestaña **Actions**.
4. Selecciona **CONSTRUIR APK** y pulsa **Run workflow** (o espera a que termine la compilación automática tras subir los archivos).
5. Cuando termine en verde, abre esa ejecución, baja a **Artifacts** y descarga `Laboratorio-de-seguridad-APK`.
6. Descomprime el archivo descargado y abre `app-debug.apk` en Android para instalarlo. Es posible que Android pida autorizar instalaciones desde esa fuente.

## Detalles

- Nombre visible: Laboratorio de seguridad
- Identificador: `mx.laboratorio.seguridad`
- Versión inicial: 1.0
- Android mínimo: Android 6.0 (API 23)
- No solicita permisos de Internet, cámara, micrófono, contactos ni ubicación.
- La aplicación carga el HTML localmente; no necesita conexión a Internet para ejecutar las lecciones.

## Importante

La compilación no se ejecuta dentro de este ZIP. GitHub Actions generará el APK cuando subas el proyecto a GitHub y ejecutes el flujo.
