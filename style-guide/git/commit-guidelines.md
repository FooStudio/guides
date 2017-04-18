Angular Commit Guidelines
=

[Github][1]

Cada commit consiste de un **encabezado**, un **cuerpo** y un **pie de página**. El **encabezado** tiene un formato especial que consiste de **tipo**, **contexto** y **descripción**.

```
<tipo>(<contexto>): <descripción>
<SALTO DE LÍNEA>
<cuerpo>
<SALTO DE LÍNEA>
<pie de página>
```

El **encabezado** es obligatorio, el **contexto** es opcional.

Ninguna línea en el mensaje debe de sobrepasar 100 caracteres. Esto permite que el mensaje sea más fácil de leer en Github y en varias herramientas de Git.

Revertir
-
Si el commit revierte un cambio anterior, debe de empezar con `revert:` seguido por el **encabezado**. En el **cuerpo** se debe de agregar: `Revierte al commit <hash>`, donde el hash es el SHA del commit que esta siendo revertido.

Tipo
-
Debe de ser uno de los siguientes:
- **feat**: Un cambio que agrega un nuevo feature
- **fix**: Un cambio que arregla un bug
- **docs**: Cambios de documentación solamente
- **style**: Cambios que no modifican el significado del código (agregar o quitar white-spaces, dar formato, agregar semicolons, etc)
- **refactor**: Un cambio que no arregla un bug y tampoco es un feature
- **perf**: Un cambio que mejora el rendimiento
- **test**: Un cambio que agrega o corrige tests existentes
- **chore**: Un cambio en el proceso de compilación (gulp, webpack, jsdocs, etc)

Contexto
-
Cualquier cosa que identifique el lugar del cambio. Por ejemplo `src/views`, `src/styles`, `backend/controllers`, `backend/db`, etc.

Se puede usar `*` cuando se afecta a más de un contexto.

Descripción
-
Contiene un mensaje sucinto sobre el cambio:
- usar el imperativo, tiempo presente: "modifica" no "modifico" no "modificando"
- no capitalizar la primera letra
- no usar punto al final

Cuerpo
-
Así como en la descripción, usar el imperativo, tiempo presente. El **cuerpo** debe de incluir la motivación que produjo el cambio así como el contraste con la funcionalidad anterior.

Footer
-
Debe de contener información sobre cambios que puedan afectar a otros componentes o hacerlos fallar (breaking changes).

Debe de comenzar con la línea `BREAKING CHANGE:` con un espacio o entre dos líneas nuevas.

Herramientas
-
Para dar este tipo de formato a los commits se puede utilizar [Commitizen][2].

Ejemplos
-
Solo encabezado
```
docs(readme): documenta los scripts de npm
```
Encabezado y cuerpo
```
feat(src/scripts): reemplazar navegacion con hash por history

El back-end esta actualizado y sirve las paginas necesarias, esto propicia el cambio para usar
history en vez de hash para navegar el sitio.
```

Revertir
```
revert:feat(src/styles): cambia los easings del carousel

Revierte al commit c6bd58e
```

Footer
```
refactor(src/scripts): elimina al helper core.isFirefox()

Este helper fue un fix temporal, su uso se reemplazo con polyfills y fallbacks.

BREAKING CHANGE:

El metodo estaba expuesto de manera publica, sin embargo nunca se alento su uso y tampoco esta
documentado. En el caso de que se haya usado fuera de contexto la manera de solucionarlo es
reemplazarlo por un polyfill o un fallback dependiendo el caso.
```

[1]: http://bit.ly/291c3GU
[2]: http://bit.ly/2oJTFed
