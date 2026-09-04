# app-ads.txt — Black Hole Factory

Este repo sirve para hostear el archivo `app-ads.txt` en un dominio propio,
gratis, con **GitHub Pages**. Sirve para que AdMob pueda verificar que tenés
derecho de vender el inventario de tu app y no pierdas ingresos.

## 1) Poner tu ID de publicador real

Abrí `app-ads.txt` y reemplazá `pub-XXXXXXXXXXXXXXXX` por TU ID de publicador
de AdMob. Lo encontrás en:

**AdMob → Configuración → Configuración de la cuenta → ID de publicador**
(es algo como `pub-1234567890123456`, SIEMPRE empieza con `pub-`).

> NOTA: el ID del `AdManager.kt` (`3924779479996677`) es el ID de la *app*,
> NO el de publicador. Buscá el que empieza con `pub-`.

Debería quedar así (con tu número real):

```
google.com, pub-1234567890123456, DIRECT, f08c47fec0942fa0
```

## 2) Subirlo a GitHub Pages

1. Creá un repo nuevo en GitHub (ej: `app-ads-txt`), público.
2. Subí este `app-ads.txt` a la **raíz** del repo.
3. Andá a **Settings → Pages** → en "Branch" elegí `main` / root y guardá.
4. Esperá 1-2 min a que se publique. La URL queda:
   `https://TUUSUARIO.github.io/app-ads-txt/app-ads.txt`
   Probala en el navegador: debe mostrar el contenido del archivo.

## 3) Avisarle a AdMob

En AdMob: **Configuración → visto de aplicaciones → app-ads.txt**.
Agregá tu dominio/host como dueño autorizado y verificá que Google lo lea
(hay una opción de "verificación" que muestra si el archivo es válido).

Normalmente propagación tarda hasta 24 h.

## Alternativa sin dominio

Si no querés GitHub Pages, cualquier hosteo que sirva el archivo por HTTPS
en la raíz de un dominio funciona igual. Lo único necesario es que la URL
del app-ads.txt sea accesible públicamente.
