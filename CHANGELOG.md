# Olfix Tuner — Changelog

## [3.4.0] - 2026-04-15
### Novedades
- Metrónomo: nueva pestaña ♩ METRO junto a Guitarra y Voz
- Display BPM estilo 7 segmentos con el mismo diseño retro del afinador
- Tap tempo: golpeás el ritmo y la app calcula el BPM automáticamente
- Botones +/- con click sostenido para ajuste rápido de tempo
- Compás configurable: 2/4, 3/4, 4/4, 5/4, 6/8, 7/8
- Subdivisiones: negras, corcheas, tresillos y semicorcheas
- Indicadores LED sincronizados con el pulso
- Modo práctica: sube el tempo automáticamente cada N compases hasta el BPM objetivo
- El nombre del tempo (Andante, Allegro, etc.) se muestra en tiempo real

## [3.2.0] - 2026-04-13
### Mejoras
- Corrección de octava en modo voz: el detector ya no salta una octava cuando YIN se engancha en un sub-armónico o primer armónico de la voz. La frecuencia detectada se valida contra la lectura estable anterior en una ventana de 200 ms; si el ratio es ≈0.5 o ≈2.0 se corrige automáticamente. El modo guitarra no se ve afectado.

## [3.1.0] - 2026-04-03
### Novedades
- Detección más rápida y confiable: buffer 2048 con solapamiento y filtro de probabilidad
- El medidor LED ahora usa el mismo suavizado que el osciloscopio para mayor estabilidad visual

### Mejoras
- El diapasón se aplica en todos los filtros y en el resaltado de cuerdas, evitando desalineaciones con A≠440 Hz
- Ruido y frecuencias de cuerdas se muestran con textos localizables desde recursos

### Correcciones
- Vibración compatible con API 21+ usando getSystemService seguro según versión

## [3.0.0] - 2026-03-02
### Mejoras
- Noise gate ajustado y nuevo filtrado por cuerda para afinación más precisa y cómoda

## [2.9] - 2026-04-01
### Novedades
- Modo landscape: layout rack horizontal al girar el dispositivo
- Opción en Ajustes para activar/desactivar la rotación automática
- Changelog movido a archivo `assets/changelog.txt` para facilitar edición

### Mejoras
- Header compacto en landscape con botón de micrófono integrado
- Presets y cuerdas en fila horizontal compacta en landscape
- Banner publicitario presente en ambas orientaciones

## [2.8] - 2026-03-31
### Novedades
- Indicador visual de calibración: spinner animado y botón deshabilitado mientras el noise gate se calibra
- Sistema de actualizaciones corregido: la descarga ahora usa la carpeta privada de la app y verifica el estado antes de instalar

### Mejoras
- Indicador de afinación más suave y estable: suavizado aumentado, historial de pitch más largo
- Osciloscopio siempre en movimiento: animación suave hacia el centro cuando no hay señal
- Nota fantasma reemplazada por texto moderno con glow, compatible con cifrado latino y sostenidos sin desplazamiento

## [2.7] - 2026-03-29
### Novedades
- Panel retro LED: nuevo diseño completo de la pantalla principal con medidor de 31 LEDs rojo/ámbar/verde
- Osciloscopio con nota fantasma: la nota detectada aparece detrás de la onda de afinación
- Flechas funcionales: indican si hay que subir o bajar la cuerda para afinar
- Los 3 LEDs centrales se ponen verdes solo cuando la afinación es perfecta
- Cifrado latino restaurado: compatible con el nuevo diseño retro
- Banner publicitario reservado en el pie de pantalla para implementación futura de AdMob

### Mejoras
- Noise gate más preciso: calibración automática al inicio con botón de recalibración manual
- Sensibilidad de detección mejorada: la señal se mantiene activa 500ms después de que la nota decae
- Selector AUTO/MANUAL reubicado a la izquierda del osciloscopio
- Presets de afinación reubicados a la derecha del osciloscopio

## [2.6] - 2026-03-27
### Novedades
- Rediseño completo de la pantalla principal con estética retro de panel LED de los 80s
- Display de nota detectada estilo 7 segmentos con glow
- Medidor de cents con barra de 31 LEDs de colores
- Gama cromática integrada dentro del panel de medición
- Indicador de cuerdas activas dentro del panel LED

### Correcciones
- El indicador de afinación ya no se congela al cambiar de nota
- La calibración del noise gate ahora funciona correctamente al iniciar la app

## [2.5] - 2026-03-25
### Novedades
- Noise gate automático al iniciar: la app mide el ruido ambiente y calibra sola
- Botón para recalibrar el noise gate manualmente desde la pantalla principal
- Nuevo diseño del header con logo OLFIX TUNER

### Correcciones
- Fix en el tildado visual de cuerdas afinadas

## [2.4] - 2026-03-23
### Mejoras
- Botones Guitarra/Voz rediseñados con nuevo estilo visual
- Textos más grandes y legibles en toda la interfaz
- Gráfico de trayectoria mejorado: más fluido y visible
- Efecto visual en el botón de ajustes

### Correcciones
- Sistema de actualizaciones corregido: instalación más confiable

## [2.3] - 2026-03-21
### Novedades
- Gráfico de trayectoria mejorado: línea continua sin cortes, más gruesa y visible
- Botón de donación PayPal agregado en ajustes

## [2.2] - 2026-03-19
### Novedades
- Botón para pausar y reanudar el micrófono desde la pantalla principal
- Sistema de actualizaciones mejorado: descarga e instala automáticamente

### Correcciones
- El sonido de confirmación ya no interfiere con la afinación
- El tema claro es ahora el predeterminado al instalar la app
- Los Hz de las cuerdas se actualizan correctamente al cambiar la frecuencia base

## [2.1] - 2026-03-18
### Novedades
- Sistema de actualizaciones automáticas con descarga guiada
- Modo manual de afinación mejorado
- Banner "¡Listo para tocar!" rediseñado

## [2.0] - 2026-03-15
### Novedades
- Ajustes operativos: frecuencia base funcional, diapasón reproduce la frecuencia elegida
- Tema claro/oscuro persiste entre sesiones
- Modo manual: bloqueá una cuerda específica para afinar sin interferencias
- Al afinar una cuerda por 1 segundo se marca en verde con ✓
- Banner "¡Listo para tocar!" cuando las 6 cuerdas están afinadas

## [1.8] - 2026-03-10
### Correcciones
- Cambios de modo claro/oscuro ya no rompen la UI
- Al volver de ajustes, la pantalla principal se refresca correctamente

## [1.7] - 2026-03-08
### Novedades
- Opciones para vibración/sonido al afinar
- Notación americana/latina conmutables

## [1.6] - 2026-03-06
### Novedades
- Nuevo ícono de la app
- Switches de ajustes con estados claros

## [1.5] - 2026-03-04
### Novedades
- Pantalla de ajustes accesible desde el ícono de tuerca

## [1.4] - 2026-03-02
### Novedades
- Nuevo indicador de afinación con cuadro que se centra al afinar

## [1.3] - 2026-02-29
### Correcciones
- Detección de notas correcta en todas las cuerdas

## [1.2] - 2026-02-27
### Mejoras
- Detección de notas más estable y precisa
- La pantalla se mantiene encendida durante el uso

## [1.1] - 2026-02-25
### Novedades
- Gráfico de trayectoria del tono, modos Guitarra y Voz, afinaciones predefinidas, nivel de ruido

## [1.0] - 2026-02-20
### Novedades
- Primera versión de Olfix Tuner
