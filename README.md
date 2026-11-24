# Conservación de la cantidad de movimiento · Simulador interactivo

Aplicación docente de **Francisco Goitia** · francisco.goitia@upc.edu.

## Ejecutar

- **En línea:** [GitHub Pages](https://fragoi95.github.io/momentum_animacion/) (una vez habilitado en el repositorio).
- **Sin conexión:** descarga `index.html` y ábrelo en Chrome, Edge o Firefox. No se requieren bibliotecas, servidores ni conexión a internet.

## Contenido

Simula un **choque frontal unidimensional entre dos esferas** sobre una pista ideal, sin rozamiento y sin fuerzas externas durante el choque. Es una introducción deliberadamente más simple que un péndulo de Newton, para separar la conservación de la cantidad de movimiento de la conversión entre energía gravitatoria y cinética.

Se pueden modificar las masas `m_A`, `m_B` (0,2–10 kg), las velocidades iniciales `u_A`, `u_B` (−5 a 5 m/s) y el coeficiente de restitución `e` (0–1). Incluye ejemplos preestablecidos, reproducción y pausa, velocidades de reproducción, retroceso a antes/después del impacto y barra temporal. Calcula las velocidades finales y los balances de momento lineal y energía cinética.

El modelo usa la conservación de cantidad de movimiento y la relación de restitución:

```text
p = mA*uA + mB*uB
vA = (p - mB*e*(uA-uB)) / (mA+mB)
vB = (p + mA*e*(uA-uB)) / (mA+mB)
```

Las ecuaciones de choque se aplican únicamente si `uA > uB` (A comienza a la izquierda de B y lo alcanza). Cuando no hay contacto, ambas mantienen sus velocidades. El instante de impacto y las posiciones se calculan analíticamente para evitar errores numéricos de integración.

Para `e = 1` se conserva también la energía cinética. Para `e < 1` existe disipación energética, y cuando `e = 0` las dos esferas continúan con una misma velocidad inmediatamente después del choque, sin representar explícitamente la deformación de contacto. Los radios dibujados varían aproximadamente con la raíz cúbica de la masa para mejorar la lectura; no representan un material con densidad prefijada.

## Publicación en GitHub Pages

En **Settings → Pages → Build and deployment**, selecciona `Deploy from a branch`, rama `main` y carpeta `/(root)`, y guarda. La dirección será <https://fragoi95.github.io/momentum_animacion/> una vez completada la publicación.