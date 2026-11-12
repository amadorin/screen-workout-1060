# training1060

Segundo campo de datos Connect IQ del repo, con otro app id (no pisa a "Zona Potencia 3s"). Pantalla completa para Edge 1050, 1060 y Edge 850. El nombre dice 1060, pero se compila y prueba para el 1050.

Instalar: copia `releases/training1060-edge1050.prg` (o `-edge850.prg` / `-edge1060.prg`) a `GARMIN/Apps` del Edge y ponlo en una pantalla de datos de un solo campo.

## Qué trae
- Arriba, pestañas POTENCIA / VELOC / FC: toca una para cambiar el número grande.
- Número grande, barra de zona con el objetivo del paso del entrenamiento (semáforo verde/ámbar/rojo) y media lap.
- Barra de páginas con flechas y puntos (toca la mitad izquierda o derecha de la zona de abajo): RIDE, PASOS, ANÁLISIS, CUERPO.
  - RIDE: FC, tiempo o cuenta atrás del paso, velocidad, distancia, cadencia, desnivel.
  - PASOS: paso actual, siguiente y los últimos 3 terminados (duración, rango, media y si cumpliste).
  - ANÁLISIS: gráfico de 40 s con banda objetivo, IF, TSS, NP y media.
  - CUERPO: FC, FC media y máxima, calorías, potencia media y máxima.
- Tarjeta del siguiente paso en los últimos 8 s con cuenta atrás.
- Aviso al terminar cada paso, tema claro/oscuro, ajuste de FTP en el Edge.

## Límites
- La API solo da el paso actual y el siguiente. No hay lista completa ni "paso 8/11": el campo cuenta los pasos y guarda los terminados.
- No hay datos de comida, bebida, temperatura corporal ni HSI en el API de Connect IQ.
- Sin probar en el Edge todavía.

## Edge 850

Pantalla táctil de 420x600 (la del 1050 es 480x800). Mismo diseño escalado; como las fuentes miden lo mismo en píxeles, en el 850 se baja un escalón de fuente en todos los textos para que quepan en las casillas más pequeñas. Compila para el 850 (datafield 128 KB, API 6.0); sin probar en el aparato.
