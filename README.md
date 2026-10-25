# Shin Megami Tensei: Devil Survivor 2 Record Breaker — Traducción al castellano

[![Invítame a un café en Ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/johanderohan)

Ficha del proyecto, capturas y más traducciones al castellano en **[Parches en Castellano](https://parchesencastellano.com/traducciones/nintendo-3ds/shin-megami-tensei-devil-survivor-2-record-breaker)**.

Traducción al **español de España** de *Shin Megami Tensei: Devil Survivor 2 Record Breaker* (Nintendo 3DS, Atlus, 2015), que nunca salió en español. Se ha hecho sobre la **edición americana en inglés**; no es una traducción directa del japonés.

Se distribuye como parche **XDELTA** para crear una ROM `.3ds` ya traducida, más unas pequeñas carpetas para consola por si ves los menús en inglés (p. ej. con la **actualización 1.1** del juego instalada). Necesitas tu propia copia del juego: la descarga no incluye ninguna ROM.

## Estado

Versión **1.0.4**: guion completo, interfaz, tablas de datos y rótulos gráficos, compatible con el juego **con o sin la actualización oficial 1.1**, y con el **DLC** de las 6 batallas descargables traducido.

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
- **Consola real (New 2DS XL con Luma3DS 13.4):** juego original instalado, con y sin la actualización 1.1, más la carpeta `luma`: arranca, menús, avisos, cabecera y diálogos en castellano. Ahí se descubrió que, con un `code.ips`, Luma usa el ejecutable de la ROM base aunque haya actualización, y por eso la v1.0.3 usa una sola carpeta.
- **Pendiente:** no se han jugado la fusión, el compendio, la subasta, el sistema de Destino ni los días posteriores al primero; falta una partida completa hasta los finales y la prueba en consola física. No se certifican todas las ventanas ni rutas.
- Siguen en inglés algunos rótulos gráficos menores (p. ej. «No Signal» en la imagen del móvil y logotipos de Nicaea), conservados a propósito o pendientes.
- Las ayudas largas de la parte inferior de la pantalla se desplazan como en el original: verlas cortadas en un momento dado es normal.

La traducción y la revisión se han hecho con asistencia de modelos de IA; no se atribuye una revisión humana independiente.

## Descarga

En **[Releases](../../releases)** (versión 1.0.5):

| Fichero | Para qué | SHA-256 |
|---|---|---|
| `desu2rb-es-v1.0.5.xdelta` | Parche de la ROM. **Siempre.** | `64d6298af7d17f5e3378b20eb6a0faa59381a36436385d1661cf000a4b9a17f3` |
| `desu2rb-es-v1.0.5-consola.zip` | Carpeta `luma` (opción C) y carpeta de Azahar (opción A) | `c09cf9eb186175fb08de55f9eb1554921a883acd7aae08e8d543bbac2f418f73` |
| `desu2rb-es-v1.0.5-actualizacion-1.1-godmode9.xdelta` | Actualización 1.1 traducida, CIA descifrada con GodMode9 (opción D) | `1160b43ac091baf85fd6a21062c99943e4434634e93fd2c65c351c08d9790a10` |
| `desu2rb-es-v1.0.5-actualizacion-1.1-batch.xdelta` | Ídem, CIA descifrada con Batch CIA 3DS Decryptor (opción D) | `193a1ce13c793c1593dd5fb8925e21dd0aea1be11cb1d6da3d7c1243f95dd25a` |
| `desu2rb-es-v1.0.5-dlc-godmode9.xdelta` | DLC traducido, CIA descifrada con GodMode9 (opción E) | `e3963336792e65ed3624a2c08f932fadc77f4f712babd2c7da3d1c742e8e711e` |
| `desu2rb-es-v1.0.5-dlc-batch.xdelta` | Ídem, CIA descifrada con Batch CIA 3DS Decryptor (opción E) | `10cff1a26890c3c4de688f2f333f4b4bdbd99da22362cde6fb0d59e94d27edd8` |

**Dos formas de descifrar una CIA, dos parches.** GodMode9 (*CIA image options → Decrypt file*) descifra la CIA tal cual: el resultado tiene siempre el mismo MD5. [Batch CIA 3DS Decryptor Redux](https://github.com/xxmichibxx/Batch-CIA-3DS-Decryptor-Redux) (Windows; responde **No** a convertir en CCI) la vuelve a montar con un ticket aleatorio: su MD5 cambia cada vez que se usa, así que no hay MD5 que comprobar. Su parche ignora esos datos y sirve para cualquier ejecución. Los dos parches dan la misma CIA traducida; si la CIA de origen no es la correcta, xdelta da un error en lugar de crear una CIA rota.

## Versión necesaria

| Dato | Valor |
|---|---|
| Edición | América (USA), ROM `.3ds` descifrada del juego base |
| Código de producto / Title ID | `CTR-P-ADXE` / `0004000000159500` |
| Tamaño | 4.294.967.296 bytes |
| MD5 | `872b26825246bc314edbab32c8779bd6` |
| SHA-256 | `d623197901e0befaa91205e9092a6593240b3ce5e138e9089bea428883028b2c` |

No vale para las ediciones europea ni japonesa.

## Instalación

### Paso común: parchear la ROM

1. Comprueba el MD5 de tu ROM (`md5sum`, `md5` o `CertUtil -hashfile … MD5` en Windows).
2. Aplica `desu2rb-es-v1.0.5.xdelta` con [Delta Patcher](https://github.com/marco-calautti/DeltaPatcher/releases) o con
   `xdelta3 -d -s "ROM original.3ds" desu2rb-es-v1.0.5.xdelta "ROM traducida.3ds"`.
3. La ROM traducida debe tener MD5 `13e150ab747a0bbcc292b7af241a6464` (la misma que la v1.0).

Después, elige **una** opción:

### A. Emulador (Azahar)

1. Abre la ROM traducida. Listo.
2. Solo si instalaste en Azahar la actualización 1.1 y ves menús en inglés: clic derecho en el juego → **Open Mods Location** y copia ahí los dos ficheros de `azahar-con-actualizacion-1.1` (del ZIP).

### B. Consola sin la actualización 1.1

1. Instala o carga la ROM traducida como siempre (por ejemplo, conviértela en CIA e instálala con FBI).
2. Listo: todo sale en castellano.

### C. Consola con la actualización 1.1 instalada (recomendado)

Síntoma: menús y correos en inglés y huecos tras las letras con tilde. No hace falta desinstalar la actualización.

1. Extrae `desu2rb-es-v1.0.5-consola.zip`.
2. Copia la carpeta `luma` de dentro de `consola` a la raíz de la SD. Debe quedar `luma/titles/0004000000159500/code.ips` y `exheader.bin` (sustituye los de versiones anteriores).
3. Enciende con **SELECT** pulsado, activa **Enable game patching** y guarda.
4. Arranca el juego: todo en castellano. En el título no saldrá «Ver. 1.1»; es normal (Luma usa el ejecutable de la ROM, que es el traducido).

Si parcheaste la ROM con la v1.0.1 o la v1.0.2, vuelve a parchearla con la v1.0.5 antes de usar esta carpeta; si no, el juego se cuelga al arrancar. La v1.0 vale tal cual.

### D. Consola con la actualización 1.1 traducida (avanzado)

Para mantener la 1.1 (lleva un arreglo de SpotPass) sin la carpeta de Luma.

1. Consigue la CIA de la actualización 1.1 (`0004000E00159500 … (v1.1.0) (U)`, 2.752.768 bytes; cifrada, MD5 `32835fc9d87b7d27cb36e4ffda98397e`) o vuelca con GodMode9 la que tengas instalada.
2. Descífrala:
   - **GodMode9** (*CIA image options → Decrypt file*): debe quedar con SHA-256 `457a23cd1e4cd81efac563ba638b4b83ca75a97b67347850bb023b4f2de580ae`. Usa `desu2rb-es-v1.0.5-actualizacion-1.1-godmode9.xdelta`.
   - **Batch CIA 3DS Decryptor**: su MD5 varía; usa `desu2rb-es-v1.0.5-actualizacion-1.1-batch.xdelta`.
3. Aplica el parche (Delta Patcher o xdelta3). El resultado, con cualquiera de los dos, tiene SHA-256 `4a2dddbf438c5451d0be48430894b16eae86f6a703f21fca6799a1d4602ec07e`.
4. Instálala con FBI encima de la oficial.
5. No uses a la vez la carpeta de la opción C: con un `code.ips` presente, Luma ignora la actualización.

Esta opción no se ha probado aún en una consola real.

### E. DLC: las 6 batallas descargables

Traduce los combates, los correos de Nicaea y el menú de las 6 batallas («Macca a la fuga», «Que crezcan los demonios», «Adicionetario», «¡Habilidades en liquidación!», «La pelea de principiantes» y «Rescate del demonio perdido»).

1. Consigue la CIA del DLC completo (`0004008C00159500 … (v0.1.0) (W)`, los 6 contenidos, 240.192 bytes; cifrada, MD5 `3a428e61f06e4aea1748b75aa757f869`).
2. Descífrala:
   - **GodMode9** (*CIA image options → Decrypt file*): debe quedar con SHA-256 `438ac694100b9c13243815496a4eb1399a66deeb909d3f02144c707e0c2fa858`. Usa `desu2rb-es-v1.0.5-dlc-godmode9.xdelta`.
   - **Batch CIA 3DS Decryptor**: su MD5 varía; usa `desu2rb-es-v1.0.5-dlc-batch.xdelta`.
3. Aplica el parche (Delta Patcher o xdelta3). El resultado, con cualquiera de los dos, tiene SHA-256 `71e56a251b254ee51aa96601deb78444fecf52edb6d32ed745322b493d96f573`.
4. Instálala con FBI (o en Azahar: *File → Install CIA*).

El DLC traducido no se ha probado aún en una consola ni en emulador: está comprobado por hashes y relectura de los ficheros. Falta ver en pantalla si el menú de DLC muestra bien las tildes.

## Cambios

### v1.0.5 — 2026-10-25

- Parches para la actualización 1.1 y el DLC también para quien descifre la CIA con Batch CIA 3DS Decryptor (rehace la CIA con un ticket aleatorio y su MD5 cambia en cada uso). Probados con los programas de esa herramienta: varias ejecuciones dan la misma CIA traducida que la opción de GodMode9.
- Mismo parche de ROM, carpeta de consola y traducción que la v1.0.4.

### v1.0.4 — 2026-10-25

- DLC traducido: las 6 batallas descargables (combates, correos de Nicaea y menú), con un parche aparte.
- Mismo parche de ROM, carpeta de consola y actualización que la v1.0.3.

### v1.0.3 — 2026-10-25

- Una sola carpeta `luma` para consola, válida con o sin la actualización 1.1: se ha comprobado en una consola real que, si hay un `code.ips`, Luma usa el ejecutable de la ROM base y no el de la actualización, así que la carpeta lleva el parche de la 1.0 y la ROM vuelve a ser la de la v1.0. Ya no hay que mirar el título.
- Nuevo parche opcional para tener la actualización oficial 1.1 traducida, sin Luma.

### v1.0.2 — 2026-10-25

- Arreglado el cuelgue al arrancar en consola con la carpeta `luma` de la 1.0.1 cuando el juego usa el ejecutable original (1.0): ahora hay una carpeta para cada versión, y se elige mirando si el título pone «Ver. 1.1». Gracias a Bulkhead28 por probarlo en consola.
- Mismo parche de ROM, texto y gráficos que la 1.0.1.

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
