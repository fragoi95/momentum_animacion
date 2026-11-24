# Conservación del momentum — simulador entre paredes

**Francisco Goitia** · francisco.goitia@upc.edu

Aplicación docente de movimiento unidimensional: dos esferas colisionan entre sí y rebotan contra dos paredes fijas. Interfaz clara, con controles mínimos para introducir masa y velocidad inicial.

## Abrir la aplicación

- **Online:** https://fragoi95.github.io/momentum_animacion/ (si GitHub Pages está activado).
- **Sin internet:** descargar `index.html` y abrirlo directamente con Chrome o Edge.

No depende de bibliotecas externas.

## Controles

- Masa y velocidad inicial de las esferas A y B.
- Iniciar, pausar y reiniciar la animación.
- Velocidad de reproducción 0,5×, 1× o 2×.
- Lectura en tiempo real de momento lineal de A y B, momento de las dos esferas y energía cinética total.

## Modelo físico

- Se considera movimiento unidimensional horizontal, sin rozamiento.
- Todos los choques entre esferas son perfectamente elásticos, con `e=1`.
- Las paredes se consideran inmóviles, con rebote perfectamente elástico.
- En un choque entre esferas se conserva el momento lineal y la energía cinética del par.
- **Al impactar una esfera contra una pared, la pared ejerce un impulso externo sobre las esferas.** Por tanto, el momento de las dos esferas no se conserva a través de ese impacto. Si se incluye la pared y su soporte en el sistema, el impulso tiene la correspondiente reacción externa.

Los tamaños dibujados de las esferas son iguales independientemente de sus masas, para facilitar la comparación.

## GitHub Pages

En Settings → Pages seleccionar Deploy from a branch, rama main y carpeta /(root). Los cambios de `index.html` se publican automáticamente.
