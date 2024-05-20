
Maquinas de Soporte Vectorial:

Se pueden hablar como "máximo margen"

Condiciones del SVM:
B es proporcional de la distancia del origen

Ambos tienen el mismo símbolo, es decir que se expresan a través de su multiplicación de forma positiva.

lambda = multiplicador de Lagrange

Se incorporan las optimizaciones en el índice lagrangiana

Problema dual: otro problema de optimización

Vector Suporte, cuando X esta en 0

Si X es vector soporte alfa o lambda = 0

Para todos los vectores soporte alfa/lambda es = 0

Las que están en el borde, son las que afectan la optimización.

La optimización depende de las muestras que están en el borde.

Como puedo permitir que algunas muestras "violen" el márgen:

Se agrega una "ayudita" un chi, que entrega la diferencia de esa muestra para que ese valor entre a conjunto

Esto se denomina como: "Margen suave: Variables de holgura"

Se "acota" con phi llamado "kernels"


![[./Recording 20240506114729.webm|Recording 20240506114729]]



