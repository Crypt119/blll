# Blue Lock Manager — Versión Beta: 0.0.1

Proyecto Android (WebView, sin internet) que empaqueta el juego como APK. El juego está en `app/src/main/assets/index.html` y se juega con el celular acostado.

## Opción A: APK sin instalar nada (GitHub Actions)
1. Crea un repositorio en github.com y sube TODO el contenido de esta carpeta (incluida `.github`).
2. Entra a la pestaña **Actions** → **Build APK** → **Run workflow**.
3. Cuando termine (3-6 min), abre la ejecución y descarga **BlueLockManager-beta-0.0.1-apk** (sección Artifacts).
4. Descomprime, pasa `app-debug.apk` al celular e instálalo (permite "instalar apps desconocidas").

## Opción B: Android Studio
1. File → Open → elige esta carpeta y espera el sync de Gradle.
2. Build → Build Bundle(s) / APK(s) → Build APK(s).
3. El archivo queda en `app/build/outputs/apk/debug/app-debug.apk`.

## Actualizar el juego
Reemplaza `app/src/main/assets/index.html` por la versión nueva y vuelve a compilar.

Fan game no oficial inspirado en Blue Lock. Plantillas y estadísticas inventadas.

## Actualizar sobre una versión ya instalada
Si Android no deja instalar el APK nuevo encima del anterior, desinstala primero la versión vieja (los APK de GitHub Actions se firman con una clave distinta en cada ejecución). La partida guardada vive dentro de la app, así que se pierde al desinstalar.
