# Shin Megami Tensei: Devil Survivor 2 Record Breaker — Traducción al castellano

[![Invítame a un café en Ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/johanderohan)

Ficha del proyecto, capturas y más traducciones al castellano en **[Parches en Castellano](https://parchesencastellano.com/traducciones/nintendo-3ds/shin-megami-tensei-devil-survivor-2-record-breaker)**.

Traducción al **español de España** de *Shin Megami Tensei: Devil Survivor 2 Record Breaker* (Nintendo 3DS, Atlus, 2015), que nunca salió en español. Se ha hecho sobre la **edición americana en inglés**; no es una traducción directa del japonés.

Se distribuye como parche **XDELTA** para crear una ROM `.3ds` ya traducida. Necesitas tu propia copia del juego: la descarga no incluye ninguna ROM.

## Estado

Versión **1.0**: guion completo, interfaz, tablas de datos y rótulos gráficos.

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
- **Pendiente:** no se han jugado la fusión, el compendio, la subasta, el sistema de Destino ni los días posteriores al primero; falta una partida completa hasta los finales y la prueba en consola física. No se certifican todas las ventanas ni rutas.
- Siguen en inglés algunos rótulos gráficos menores (p. ej. «No Signal» en la imagen del móvil y logotipos de Nicaea), conservados a propósito o pendientes.
- Las ayudas largas de la parte inferior de la pantalla se desplazan como en el original: verlas cortadas en un momento dado es normal.

La traducción y la revisión se han hecho con asistencia de modelos de IA; no se atribuye una revisión humana independiente.

## Descarga

En **[Releases](../../releases)**: `desu2rb-es-v1.0.xdelta`.

- SHA-256 del XDELTA: `319705c887eb353e0b1ddef26b960084ae9aa242ba6c8f38f4b9e17f2eaff07b`

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

El **XDELTA exige esta ROM exacta**. No es compatible con las ediciones europea ni japonesa y no se ha verificado con actualizaciones u otros mods.

## Cómo aplicar el parche

1. Comprueba que tu ROM tiene el tamaño y las huellas de arriba:

   ```bash
   md5sum "Shin Megami Tensei - Devil Survivor 2 - Record Breaker (USA).3ds"      # Linux
   md5 "Shin Megami Tensei - Devil Survivor 2 - Record Breaker (USA).3ds"         # macOS
   CertUtil -hashfile "Shin Megami Tensei - Devil Survivor 2 - Record Breaker (USA).3ds" MD5   # Windows
   ```

2. Aplica el parche con [Delta Patcher](https://github.com/marco-calautti/DeltaPatcher/releases) o con:

   ```bash
   xdelta3 -d -s "Shin Megami Tensei - Devil Survivor 2 - Record Breaker (USA).3ds" desu2rb-es-v1.0.xdelta "Shin Megami Tensei - Devil Survivor 2 - Record Breaker (ES).3ds"
   ```

3. La ROM resultante ocupa **4.294.967.296 bytes**, MD5 `13e150ab747a0bbcc292b7af241a6464` y SHA-256 `712b4e56ebd8938fb89607da13025d4bd61298bdc777158e854de2bd9127422a`.
4. Ábrela en Azahar (o conviértela al formato que use tu consola). No cargues estados rápidos creados con otra versión del parche; las partidas guardadas del juego sí sirven.

## Cambios

### v1.0 — 2026-10-23

- Primera versión pública: guion, interfaz, tablas de datos y rótulos gráficos en castellano.

## Créditos y aviso

Proyecto de **johanderohan / Parches en Castellano**. Juego y materiales originales de **ATLUS** y **SEGA**. Traducción de aficionados sin relación oficial con ellos.

Herramientas: utilidades propias de extracción y reinserción, [Azahar](https://github.com/azahar-emu/azahar), [3dstool](https://github.com/dnasdw/3dstool) y xdelta3. Las letras castellanas reutilizan la fuente del juego; algunos rótulos gráficos usan además letras de la fuente libre Fira Sans (licencia SIL OFL).

El repositorio contiene solo este README; el parche está en Releases. No se publican ROMs, partidas ni el guion extraído. Si encuentras un problema, abre una incidencia indicando versión del parche, emulador o consola y una captura.
