# Shin Megami Tensei: Devil Survivor 2 Record Breaker — Traducción al castellano

[![Invítame a un café en Ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/johanderohan)

Ficha del proyecto, capturas y más traducciones al castellano en **[Parches en Castellano](https://parchesencastellano.com/traducciones/nintendo-3ds/shin-megami-tensei-devil-survivor-2-record-breaker)**.

Traducción al **español de España** de *Shin Megami Tensei: Devil Survivor 2 Record Breaker* (Nintendo 3DS, Atlus, 2015), que nunca salió en español. Se ha hecho sobre la **edición americana en inglés**; no es una traducción directa del japonés.

Se distribuye como parche **XDELTA** para crear una ROM `.3ds` ya traducida, más una pequeña carpeta para quien tenga instalada la **actualización 1.1** del juego. Necesitas tu propia copia del juego: la descarga no incluye ninguna ROM.

## Estado

Versión **1.0.1**: guion completo, interfaz, tablas de datos y rótulos gráficos, compatible con el juego **con o sin la actualización oficial 1.1**.

| Parte | Alcance |
|---|---|
| Guion | **43.155 textos únicos** de diálogo: historia de los dos arcos (Septentriones y Triangulum), conversaciones de Destino, combates y finales |
| Datos | **2.649 textos**: compendio de demonios, frases de fusión, subasta y títulos de capítulo |
| Interfaz | **3.313 textos** del ejecutable: menús, ayudas, habilidades, nombres, correos y perfiles de Destino |
| Texto dentro de imágenes | **299 texturas**: título, nombre del héroe, combate, estado, cabecera de días, correo, fusión, subasta, rótulos de lugar, títulos de día y frases de los finales |
| Caracteres españoles | **á é í ó ú ü ñ Á É Í Ó Ú Ü Ñ ¡ ¿ « »** en las tres fuentes del juego |

Se conservan los nombres de demonio y de hechizo de la saga (Jack Frost, Agi, Bufu…), los logotipos, los rótulos de marca y las voces originales. La terminología sigue la de nuestras traducciones de *Shin Megami Tensei IV: Apocalypse* y *Strange Journey Redux* (PS/PM, Nv, Macca…).

### Comprobaciones y límites

- Todo el texto se ha reinsertado con validación automática de etiquetas, codificación, ancho en píxeles con la fuente real del juego, líneas por cuadro y espacio disponible en el ejecutable. Los textos que no cabían en su sitio se han trasladado a un espacio nuevo del ejecutable, comprobado en el emulador.
- Traducción por lotes con biblia y glosario comunes, revisión independiente de cada lote, atribución de hablantes en los combates para el tú/usted y pasadas de unificación.
- **Prueba jugable en Azahar:** varias rondas desde partida nueva: avisos de inicio, título, nombre del héroe (teclado completo), prólogo, día 1 hasta el combate contra Bai Suzhen, combates con estado, habilidades, comandos, resultados y subida de nivel, configuración, correo, preparación de combate y **guardado real** desde el menú. Sin cuelgues ni glifos vacíos.
- El XDELTA se ha reaplicado sobre la ROM original con resultado idéntico a la ROM reconstruida, y esa ROM arranca en Azahar sin mods.
- **Actualización 1.1:** comprobado en Azahar con la actualización oficial instalada (menús, correos de Nicaea, tildes y cabecera en castellano) y sin ella. La carpeta para consola se ha verificado de forma automática sobre los dos ejecutables, pero no se ha probado en una consola real.
- **Pendiente:** no se han jugado la fusión, el compendio, la subasta, el sistema de Destino ni los días posteriores al primero; falta una partida completa hasta los finales y la prueba en consola física. No se certifican todas las ventanas ni rutas.
- Siguen en inglés algunos rótulos gráficos menores (p. ej. «No Signal» en la imagen del móvil y logotipos de Nicaea), conservados a propósito o pendientes.
- Las ayudas largas de la parte inferior de la pantalla se desplazan como en el original: verlas cortadas en un momento dado es normal.

La traducción y la revisión se han hecho con asistencia de modelos de IA; no se atribuye una revisión humana independiente.

## Descarga

En **[Releases](../../releases)**:

1. `desu2rb-es-v1.0.1.xdelta`: el parche de la ROM. **Lo necesita todo el mundo.**
2. `desu2rb-es-v1.0.1-actualizacion.zip`: la carpeta `luma` para consola (y su equivalente para Azahar). Solo hace falta si tienes instalada la actualización 1.1, pero no hace daño ponerla aunque no la tengas.

- SHA-256 del XDELTA: `44e29bb5382a7f2abf8a764b60c55b0539b9555af1e4a24961f22b035df84883`
- SHA-256 del ZIP: `81367acff3cd6c2647dbfb1ba22d88cbc9bcab7b49ac235c38a27ee5b2660782`

## Versión necesaria

| Dato | Valor |
|---|---|
| Edición | América (USA), juego base sin otros parches |
| Código de producto | `CTR-P-ADXE` |
| Title ID | `0004000000159500` |
| ROM usada | `Shin Megami Tensei - Devil Survivor 2 - Record Breaker (USA).3ds` (descifrada) |
| Tamaño | 4.294.967.296 bytes |
| MD5 | `872b26825246bc314edbab32c8779bd6` |
| SHA-256 | `d623197901e0befaa91205e9092a6593240b3ce5e138e9089bea428883028b2c` |

El **XDELTA exige esta ROM exacta** (la del juego base, aunque luego tengas instalada la actualización 1.1). No es compatible con las ediciones europea ni japonesa ni se ha verificado con otros mods.

## Cómo aplicar el parche

1. Comprueba que tu ROM tiene el tamaño y las huellas de arriba:

   ```bash
   md5sum "Shin Megami Tensei - Devil Survivor 2 - Record Breaker (USA).3ds"      # Linux
   md5 "Shin Megami Tensei - Devil Survivor 2 - Record Breaker (USA).3ds"         # macOS
   CertUtil -hashfile "Shin Megami Tensei - Devil Survivor 2 - Record Breaker (USA).3ds" MD5   # Windows
   ```

2. Aplica el parche con [Delta Patcher](https://github.com/marco-calautti/DeltaPatcher/releases) o con:

   ```bash
   xdelta3 -d -s "Shin Megami Tensei - Devil Survivor 2 - Record Breaker (USA).3ds" desu2rb-es-v1.0.1.xdelta "Shin Megami Tensei - Devil Survivor 2 - Record Breaker (ES).3ds"
   ```

3. La ROM resultante ocupa **4.294.967.296 bytes**, MD5 `a718bcb01598b1be2591099df1213b3b` y SHA-256 `3120324c55be03fe2a2f39c4edd8ac006e3d1700fd4fb0e25ac9691aa7cad23f`. Ya incluye el arreglo de SpotPass de la actualización 1.1.
4. Ábrela en Azahar (o conviértela al formato que use tu consola). No cargues estados rápidos creados con otra versión del parche; las partidas guardadas del juego sí sirven.

### Si tienes instalada la actualización 1.1

Cuando la actualización oficial 1.1 está instalada, la consola usa su ejecutable en lugar del de la ROM y verías los **menús y correos en inglés** y **huecos detrás de las letras con tilde**. No hace falta desinstalarla:

- **Consola con Luma3DS:** extrae el ZIP y copia la carpeta `luma` a la raíz de la tarjeta SD (debe quedar `luma/titles/0004000000159500/`). Después, enciende la consola manteniendo **SELECT**, activa **Enable game patching** y guarda. Puedes copiar esta carpeta aunque no tengas la actualización: no cambia nada.
- **Azahar con la actualización instalada:** clic derecho sobre el juego → **Open Mods Location** y copia allí los dos ficheros de la carpeta `azahar-con-actualizacion` del ZIP. Sin la actualización no hace falta.

## Cambios

### v1.0.1 — 2026-10-25

- Compatible con la actualización oficial 1.1: con ella instalada, los menús, los correos de Nicaea y las tildes ya salen bien (carpeta `luma` en el ZIP). Gracias a Bulkhead28 por el aviso.
- La ROM parcheada lleva ahora el ejecutable de la 1.1 traducido, con su arreglo de SpotPass.
- Mismo texto y gráficos que la 1.0. Si ya aplicaste la 1.0: sin la actualización no necesitas cambiar nada; con la actualización basta con añadir la carpeta del ZIP (no hace falta volver a parchear la ROM).

### v1.0 — 2026-10-23

- Primera versión pública: guion, interfaz, tablas de datos y rótulos gráficos en castellano.

## Créditos y aviso

Proyecto de **johanderohan / Parches en Castellano**. Juego y materiales originales de **ATLUS** y **SEGA**. Traducción de aficionados sin relación oficial con ellos.

Herramientas: utilidades propias de extracción y reinserción, [Azahar](https://github.com/azahar-emu/azahar), [3dstool](https://github.com/dnasdw/3dstool) y xdelta3. Las letras castellanas reutilizan la fuente del juego; algunos rótulos gráficos usan además letras de la fuente libre Fira Sans (licencia SIL OFL).

El repositorio contiene solo este README; el parche está en Releases. No se publican ROMs, partidas ni el guion extraído. Si encuentras un problema, abre una incidencia indicando versión del parche, emulador o consola y una captura.
