# Composite - Caso práctico

### Intención

Compone objetos en estructura de árbol para representar jerarquías todo-parte. Composite permite que los clientes traten de manera uniforme objetos individuales y composición de objetos.

### Clasificación

Patrón Estructural

### Vista Estructural

![image](https://user-images.githubusercontent.com/84739791/231043978-21a88190-bb2d-484c-8dde-3ef1b6506f1a.png)

### Vista Dinámica

![image](https://user-images.githubusercontent.com/84739791/231044058-911daa5b-4da4-4fe3-ab8f-c0599d070b30.png)

### Ejemplo Real

Imaginemos un sistema de punto de venta, en el cual se le pueden vender al 
cliente una serie de productos, estos productos pueden ser simples (Leaf) o 
paquetes (Composite). El sistema permitirá crear órdenes de ventas que estarán 
compuestas por uno o muchos productos.
El precio de los productos deberá ser calculado mediante la suma del precio de 
todos los productos internos. La siguiente imagen ilustra la estructura de un 
paquete y cómo es que el precio del mismo es calculado basado en el precio de 
los productos que lo componen.

Algunos puntos importantes a tomar en cuenta:
* Un paquete es creado mediante una serie de productos simples y 
compuestos.
* No debe existir una diferencia entre la forma que tratamos un producto 
simple de uno compuesto.
* El precio de un paquete es la suma de todos los productos simples que 
contenga.
* El sistema deberá mostrar el total de la orden y los productos que 
contiene.

![image](https://user-images.githubusercontent.com/84739791/231044489-31c2cf98-e578-49a0-a6dc-f826b426a3c1.png)


### Solución con el patrón Composite:

Para solucionar el problema planteado, tendremos que diseñar una estructura de 
productos que nos permita crear productos simples y compuestos; con los 
productos simples no tendríamos problemas, pero los productos compuestos son 
más complicados. Para crear una estructura flexible utilizaremos el patrón de 
diseño Composite, el cual nos permitirá crear estructuras de productos 
compuestas mediante productos simples.

![image](https://user-images.githubusercontent.com/84739791/231044733-12559f6c-6daf-4555-a0c2-0a9c97bc8f12.png)

![image](https://user-images.githubusercontent.com/84739791/231044806-4f5f4fa6-cab1-4c80-bf16-816008524c92.png)


# Ejecutar Java-App 

* Cargue las Extensiones Java de VS Code correcta y completamente.
* En la clase principal de clic sobre el botón Play.

