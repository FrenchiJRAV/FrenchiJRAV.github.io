---
layout: "post"
---

###Conceptualización y creación de modeles 3D

El proceso para obtener un objeto 3D es más complicado de lo que uno pensaría inicialmente. No se trata simplemente de crear una forma básica y deformarlo hasta que obtengamos lo que deseamos. Personalmente tengo un proceso con el que me siento cómodo trabajando, este tipo de procesos son variados, y los conocemos principalmente como “pipelines” de trabajo, que nos ayudan a optimizar nuestro rendimiento.
Bien, ahora les describiré como funciona mi pipeline personal. Esto no significa que sea el mejor que exista o les recomiendo seguirlos ustedes mismos, solamente es para ejemplificar mi método de trabajo.

*	Definir el ambiente que se busca crear: esto es muy importante debido a que el tipo de ambiento que buscamos construir va a delimitar los tipos de objetos que usamos, y de estos mismos, que forma tomaran.

* Investigar el tema seleccionado y obtener referencias a este: si por ejemplo seleccionamos un ambiente medieval es conveniente buscar referencias fotográficas de edificios medievales, ya sean monasterios, castillos, o una taberna.

![Bit 01](\images\MonasterioA.jpg)   

![Bit 02](\images\MonasterioB.jpg)   
https://www.google.com/search?q=monasterio+medieval&client=firefox-b-d&source=lnms&tbm=isch&sa=X&ved=0ahUKEwjN26zkhYPhAhVEIqwKHZ_oCUQQ_AUIDigB&biw=1920&bih=966#imgrc=wjqm0M1d0H94yM:


*	Creación de la forma básica del modelo: Iniciamos con una forma simple tal que un cuadrado para empezar el proceso de modelación de nuestra pieza, esto nos sirve para obtener un apercibido muy básico de lo que buscamos crear, como se muestra en la imagen siguiente.

 ![Bit 03](\images\Catedral02.png)   

*	High-Poly: En este caso este paso puede ser innecesario para personas que se enfocan en modelos “low-poly”. Ya que tenemos una forma low-poly definida, podemos empezar a trabajar lo que se conoce como “high-poly” haciendo referencia a la alta cantidad de caras y tris que un modelo o escena tiene. Tengo que especificar que esto no es el último paso, todavía falta. La siguiente imagen muestra un modelo de la imagen previa trabajado a más alto detalla, pues también se empezó a trabajar el interior.

 ![Bit 04](\images\Catedral03.png)   

*	Optimización y Re-topología: Ya que tengamos un nivel de detalle con el que estemos cómodos, debemos optimizar los modeles vía cabo un proceso que llamamos re-topología. En la imagen siguiente estoy haciendo uso de un cubo deformado con una cantidad menor de polígonos que el muro detallado. Lo que se debe realizar es tener el mapeo de los “UV” y realizar una transferencia de mapas entre ambos modelos. En el cual el modelo de menor cantidad de polígonos va a simular el detalle del modelo con más amplia cantidad de polígonos.

 ![Bit 05](\images\Catedral04.png)   

*	Texturizado: Después de haber hecho la re-topología de un modelo, tenemos un modelo de bajos polígonos con alto detalle, lo único que queda es empezar a elegir el tipo de material que tendrá el modelo y la textura que tendrá.

![Bit 06](\images\Shaders.png)
 https://www.google.com/search?biw=1920&bih=969&tbm=isch&sa=1&ei=eBWLXNj-FYKOsQXIqb24DQ&q=texturizado+de+un+modelo+shader&oq=texturizado+de+un+modelo+shader&gs_l=img.3...12589.13837..14082...0.0..0.129.745.2j5......1....1..gws-wiz-img.AxxWFsWvdX0#imgrc=b6mBgZPLMjRO1M:

 ![Bit 07](\images\Substance.jpg)
https://www.google.com/search?biw=1920&bih=969&tbm=isch&sa=1&ei=eBWLXNj-FYKOsQXIqb24DQ&q=texturizado+de+un+modelo+shader&oq=texturizado+de+un+modelo+shader&gs_l=img.3...12589.13837..14082...0.0..0.129.745.2j5......1....1..gws-wiz-img.AxxWFsWvdX0#imgrc=XDjn2EPjVv-v_M:

*	Colocación en escena: Finalmente estamos listo para poner nuestro modelo en donde lo queremos, ya sea en solitario o dentro de una escena compuesta, por ejemplo si solamente buscamos tener un “preview” en donde nadie podría interactuar con el escenario se puede crear el ambiento dentro de Maya, ubicar la cámara en un ángulo que muestre de manera adecuada la escena y obtener un render.
Otra opción si lo que se busca es una interacción por parte de una persona, recomiendo hacer uso de varios motores de juego, por ejemplo Unity o Unreal Engine, en donde se podrá jugar más fondo con diferentes opciones, por ejemplo luces y sombras, lo que nos permitirá crear un ambiente más inmersivo e interactuable con nuestros jugadores.

![Bit 08](\images\EngineBuild.jpg)
 https://www.google.com/search?biw=1920&bih=969&tbm=isch&sa=1&ei=UBaLXLbSOcbwsQWS0pPIBg&q=unreal+engine+lighting&oq=unreal+engine+lig&gs_l=img.1.0.0i19j0i8i30i19l2.36473.38471..39537...0.0..0.258.721.0j3j1......1....1..gws-wiz-img.......0j0i67j0i30.DygfpivWAq4#imgrc=7nE6BaTGWuorWM:

Bueno espero que este paso a paso de la conceptualización y creación de modelos 3D les haya sido de ayuda en sus proyectos, como bien decía al inicio de mi explicación hay varias maneras de trabajar, y lo que les acabo de explicar no es la única, conozco personas que usan programas diferentes, por lo que el orden y los procesos que deben realizar son diferentes, y hasta en algunos casos innecesarios, pero realmente lo que les explique, en todos los pipelines y programas encontraremos similitudes, por más básicas que parecieran.
