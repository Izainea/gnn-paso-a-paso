# Cómo aprende una red neuronal de grafos

Explicación interactiva, en español, del entrenamiento de una red neuronal de grafos (GCN de dos capas) para clasificación de nodos.

El ejemplo es un problema de detección de fraude: ocho cuentas bancarias, las transferencias entre ellas y solo dos cuentas revisadas. La pregunta es en qué orden revisar las demás. Los datos son inventados.

## Qué contiene

Una sola página, `index.html`, organizada como un tablero: a la izquierda la red de cuentas, que se entrena en el navegador; a la derecha doce paneles que se recorren en orden.

1. El problema
2. Por qué no basta la tabla
3. El problema escrito como matrices
4. Qué se aprende y qué no
5. Paso hacia adelante
6. La pérdida
7. Paso hacia atrás, con comprobación numérica del gradiente
8. Actualización, orden de revisión y el ciclo en PyTorch Geometric
9. Capas, campo receptivo, sobresuavizado y sobrecompresión
10. Un problema donde la respuesta está lejos y el paso de mensajes falla
11. Walk Attention: atención directa sobre los nodos a k saltos, con la evidencia y sus límites
12. Dudas frecuentes

Las matrices que aparecen en los paneles son las del modelo que se está entrenando y cambian con cada paso.

## Cómo usarla

Abrir `index.html` en un navegador. Las flechas del teclado cambian de panel. Las fórmulas se dibujan con KaTeX desde un CDN, así que necesitan conexión; la parte interactiva funciona sin ella.

No hay dependencias que instalar ni paso de compilación.
