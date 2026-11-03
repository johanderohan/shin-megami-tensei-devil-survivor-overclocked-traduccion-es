# Shin Megami Tensei: Devil Survivor Overclocked — Traducción al castellano

[![Invítame a un café en Ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/johanderohan)

Ficha del proyecto, capturas y más traducciones al castellano en **[Parches en Castellano](https://parchesencastellano.com/traducciones/nintendo-3ds/shin-megami-tensei-devil-survivor-overclocked)**.

Traducción al **español de España** de *Shin Megami Tensei: Devil Survivor Overclocked* (Nintendo 3DS, Atlus, 2011), que nunca salió en español. Se ha hecho sobre la **edición americana en inglés** (Rev 1); no es una traducción directa del japonés. Es la precuela de *Devil Survivor 2 Record Breaker*, que también hemos traducido, y comparte su terminología.

Se distribuye como parche **XDELTA** para crear una ROM `.3ds` ya traducida. Necesitas tu propia copia del juego: la descarga no incluye ninguna ROM.

## Estado

Versión **1.0**: guion completo, interfaz, tablas de datos y rótulos gráficos.

| Parte | Alcance |
|---|---|
| Guion | **24.684 textos únicos** de diálogo: los 8 días de la historia, sus rutas y finales, combates, encuentros del mapa y perfiles |
| Datos | **918 textos**: compendio de demonios, frases de fusión y subasta de demonios |
| Interfaz | **2.246 textos** del ejecutable: menús, ayudas, habilidades, hablantes, frases de la subasta y correos (Laplace Mail incluido) |
| Texto dentro de imágenes | **523 texturas**: título, menús del COMP, teclado de nombres, barra del día, combate, estado, resultados, fusión, subasta, rótulos de lugar y capítulo, y las frases del prólogo y los finales |
| Caracteres españoles | **á é í ó ú ü ñ Á É Í Ó Ú Ü Ñ ¡ ¿ « »** en las dos fuentes del juego; el teclado de nombres permite escribir **Á É Í Ó Ú Ñ Ü** y sus minúsculas |

Se conservan los nombres de demonio y de hechizo de la saga (Jack Frost, Agi, Bufu…), los logotipos, los rótulos de marca, los créditos y las voces originales. La terminología sigue la de nuestra traducción de *Devil Survivor 2 Record Breaker* (PS/PM, Nv, Macca, Subasta de demonios, Descifrado de habilidades…).

### Comprobaciones y límites

- Todo el texto se ha reinsertado con validación automática de etiquetas, codificación, ancho en píxeles con la fuente real del juego (medido en el emulador para el diálogo, las opciones, las placas de nombre, los correos y las listas de habilidades), líneas por cuadro y espacio disponible en el ejecutable. Los textos que no cabían en su sitio se han trasladado a un espacio nuevo del ejecutable.
- Una auditoría automática lee la ROM construida y comprueba los límites del motor (compresión, tablas, punteros, tamaño de los guiones, correos y memoria). Se ha comprobado que el juego carga los guiones con memoria reservada a su tamaño, sin búferes fijos, y que el pico de memoria queda muy por debajo del disponible.
- Traducción por lotes con biblia y glosario comunes, revisión independiente de cada lote y pasada final de unificación entre diálogo y menús.
- **Prueba jugable en Azahar** (unas 2,5 horas en tres rondas, desde partida nueva y desde partidas guardadas): avisos, título, dificultad, teclado de nombres, prólogo, la víspera completa (Shibuya, Omotesando, Harajuku, Shinjuku, Aoyama, Ebisu), tutoriales del COMP y del correo, primer combate entero (misión, estado, habilidades, resultados, subida de nivel, Descifrado de habilidades), opciones y **guardado y carga** desde el menú. Sin cuelgues.
- Los dos parches se han reaplicado sobre la ROM original con resultado idéntico a la ROM comprobada, y la ROM traducida arranca en Azahar sin mods. La CIA hecha a partir de ella se instala y arranca en Azahar.
- **Pendiente:** no se han jugado la fusión, el compendio, la subasta ni los días 1 a 8 (su texto está traducido, validado y revisado, pero no visto en pantalla); falta una partida completa hasta los finales. **No se ha probado en una consola real.**
- Siguen en inglés algunos rótulos gráficos menores, de letras grandes giradas o decorativas: «SELECTED» y «Unknown» en la fusión, «Placed/Free» al colocar equipos, «ST+1» al subir estadísticas, «MENU», el fondo «DEVIL AUCTION» y los créditos.
- Por falta de espacio en sus ventanas, algunos nombres de habilidad van abreviados (por ejemplo «Pot. Fuego», «Danza Fuego», «Abs. Hielo»), igual en los menús que en el diálogo.
- En la ranura de guardado de la víspera se lee «día VÍSPERA»: el «día» lo pinta el juego para todos los días.

La traducción y la revisión se han hecho con asistencia de modelos de IA; no se atribuye una revisión humana independiente.

## Descarga

En **[Releases](../../releases)** (versión 1.0):

| Fichero | Para qué | SHA-256 |
|---|---|---|
| `dso-es-v1.0.xdelta` | **Opción A (recomendada):** parche de la ROM completa | `c6bf3dda187d802d2e70b3678eaa0b2305c2a15e39ffe1b509a844c4f42599e8` |
| `dso-es-v1.0-romfs.xdelta` | Opción B: parche solo de los datos del juego | `0076f39923ddf963e58fdcddc7718c8e3c3b6d4e337f9b7ccb4f7dc2f1d8bf8d` |
| `dso-es-v1.0-ejecutable.zip` | Opción B: parche del ejecutable para Luma (consola) y Azahar | `482602c9260cd722a2edb42097dd9d588bfbc4429b729c3786d950510dcce5be` |

La opción A lo hace todo en un paso. La opción B separa los datos del juego y el ejecutable, y solo lleva nuestros cambios; necesita **las dos piezas**: sin la carpeta del ejecutable, el diálogo sale en castellano pero los menús, habilidades y correos salen en inglés y las letras con tilde quedan mal espaciadas.

## Versión necesaria

| Dato | Valor |
|---|---|
| Edición | América (USA), **Rev 1**, ROM `.3ds` descifrada |
| Código de producto / Title ID | `CTR-P-AMTE` / `0004000000038800` |
| Tamaño | 2.147.483.648 bytes |
| MD5 | `e3dc207dfbbeb8476baec8a4e85225d5` |
| SHA-256 | `d75fb82af20cbd76af6e3e678796cc8310c20d29c09eb01fb057d54bc1201af3` |

No vale para la edición europea (que tiene su propia actualización 1.1) ni para la japonesa. Esta edición americana no tiene actualizaciones ni contenido descargable.

## Instalación

Comprueba primero el MD5 de tu ROM (`md5sum`, `md5` o `CertUtil -hashfile … MD5` en Windows).

### A. Parche completo (recomendado)

1. Aplica `dso-es-v1.0.xdelta` con [Delta Patcher](https://github.com/marco-calautti/DeltaPatcher/releases) o con
   `xdelta3 -d -s "ROM original.3ds" dso-es-v1.0.xdelta "ROM traducida.3ds"`.
2. La ROM traducida debe tener MD5 `ab4cfd07b08a9de541408e1f1cc66af3`.
3. **Emulador (Azahar):** ábrela tal cual. **Consola:** cárgala como cualquier `.3ds` o conviértela en CIA (por ejemplo, con GodMode9: *Build CIA from file*) e instálala con FBI.

### B. Datos + ejecutable por separado

1. Aplica `dso-es-v1.0-romfs.xdelta` a la ROM original igual que en A. El resultado debe tener MD5 `d04fee7f4c93f0e334e60e2eedf93dcb`.
2. Extrae `dso-es-v1.0-ejecutable.zip`:
   - **Consola (Luma3DS):** copia la carpeta `luma` a la raíz de la SD (debe quedar `luma/titles/0004000000038800/code.ips` y `exheader.bin`), enciende con **SELECT** pulsado, activa **Enable game patching** y guarda.
   - **Azahar:** clic derecho en el juego → **Open Mods Location** y copia ahí el contenido de `azahar/load/mods/0004000000038800/` (la carpeta `exefs` y `exheader.bin`).
3. Arranca el juego con la ROM del paso 1.

## Cambios

### v1.0 — 2026-11-03

- Primera versión pública: guion, interfaz, tablas de datos y rótulos gráficos en castellano.

## Créditos y aviso

Proyecto de **johanderohan / Parches en Castellano**. Juego y materiales originales de **ATLUS** e **Index Corporation**. Traducción de aficionados sin relación oficial con ellos.

Herramientas: utilidades propias de extracción y reinserción, [Azahar](https://github.com/azahar-emu/azahar), [3dstool](https://github.com/dnasdw/3dstool) y xdelta3. Las letras castellanas reutilizan las fuentes del juego; algunos rótulos gráficos usan además letras de las fuentes libres Fira Sans y Noto Serif (licencia SIL OFL).

El repositorio contiene solo este README; el parche está en Releases. No se publican ROMs, partidas ni el guion extraído. Si encuentras un problema, abre una incidencia indicando versión del parche, emulador o consola y una captura.
