Certificacion de Cableado Estructurado

image alt

Descripción general

Este repositorio tiene información sobre un laboratorio que prueba redes UTP. Se hicieron pruebas en varios puntos de red con herramientas especiales para ver si funcionaban bien y cumplían con los estándares requeridos.

Objetivos

Ejecutar pruebas de certificación en puntos de red físicos para asegurarnos de que funcionen correctamente. Verificar que todo cumpla con los estándares TIA/EIA-568, que son importantes para garantizar la calidad de nuestra red. Documentar los resultados de estas pruebas utilizando Git y Markdown, para que podamos seguir el progreso y revisar los resultados de manera clara y organizada.

Contenido

parametros.md: Esto es donde se explican las definiciones técnicas  
equipo.md: Aquí se describen las funciones de la certificadora  
pruebas.md: En este archivo se presentan los resultados y el análisis de las pruebas  

Desarrollo

Se eligieron varios puntos de la red en el laboratorio para hacer pruebas de certificación. Se comprobó que el cableado estuviera en buen estado, que las conexiones fueran correctas, que no hubiera interferencias y que la conectividad funcionara bien.

Fotos de los cables usados para la certificadora

Estas fotos demuestran que los cables se encuentran en perfecto estado para su uso en la certificación del enlace

![cables usados para la certificadora 1](cables usados para la certificadora 1.png)  
![cables usados para la certificadora 2](cables usados para la certificadora 2.png)  
![cables usados para la certificadora 3](cables usados para la certificadora 3.png)  

Fotos de los puntos certificados

En las siguientes fotos se puede observar los puntos que decidimos certificar los cuales fueron analizados anteriormente para garantizar que hubiera conexión entre el rack y el punto elegido, también se pueden observar características como los metros totales del enlace, el larga de cada cable que lo compone y su algún cable no llega o que esta cruzado.

![Fotos de los puntos certificados 1](Fotos de los puntos certificados 1.png)  
![Fotos de los puntos certificados 2](Fotos de los puntos certificados 2.png)  
![Fotos de los puntos certificados 3](Fotos de los puntos certificados 3.png)  
![Fotos de los puntos certificados 4](Fotos de los puntos certificados 4.png)  

Informe de Revisión

Estos datos fueron tomados con un tester normal para verificar que los puntos fueran los mismos que tenían etiquetados y ver cuales fallas poseían para posteriormente verificarlas en la certificadora

Datos tomados:

-Tomo N.º 12 Los números 1, 5 y 8 no registran marca.

-Tomo N.º 11  
Todos los elementos funcionan correctamente.

-Tomo N.º 9  
Se detecta una falla en el cable número 5. Los demás cables se encuentran en buen estado. Sin embargo, los pares 1, 2, 3 y 6 están cruzados.

Estos fueron los datos de los puntos verificados.

Fotos de los patch panel

Un dato a tener en cuenta en una certificación es la categoría que se maneja en el enlace puesto que podría llegar a generar algunos problemas a la hora ya sea de certificar o de usar el enlace.

![Fotos de los patch panel](Fotos de los patch panel.jpeg)

En la foto se puede apreciar que el patch panel es de categoría 5e al igual que los cables que usamos para la certificación, sin embargo, los cables que estaban detrás del mismo y asumimos que en todos los enlaces es de categoría 6 la cual es mucho mejor de lo que manejan estos patch panel. Si bien no es un problema grave esto podría generar problemas a la hora de tener múltiples puntos funcionando a la vez ya que limitaría mucho la conexión del laboratorio.

Switch

En el switch se muestra la actividad de link (en este caso en el puerto 7) y el dúplex en el mismo puerto, lo que significa que el puerto correspondiente tiene conexión bidireccional (Full dúplex) dependiendo del color

Link/activity: muestra si se tiene conexión en el puerto

• Naranja: conexión de 10M  
• Verde: conexión de 100M  

Dúplex: muestra el tipo de conexión correspondiente indicado si la luz está encendida o apagada

• Encendida: La conexión es Full Dúplex osea bidireccional  
• Apagada: Si el puerto sale apagado pero su Link/activty esta encendido significa que es conexión tipo half dúplex  

![Panel Switch](Panel Switch.png)

Glosario Técnico

Glosario con definiciones de conceptos comúnmente vistos en telecomunicaciones

Ancho de banda: Cantidad máxima de datos que pueden transmitirse por un enlace en un tiempo determinado, generalmente medido en Mbps o Gbps.

Atenuación: Pérdida de señal a medida que viaja por el cable; aumenta con la distancia.

Diafonía (Crosstalk): Interferencia entre pares de cables dentro de un mismo cable, lo que puede afectar la calidad de la señal.

Normas de cableado estructurado: Conjunto de estándares (como TIA/EIA) que regulan la instalación y certificación de redes.

TIA/EIA-568: Norma que define cómo deben instalarse y certificarse los sistemas de cableado estructurado.

RJ-45: Conector estándar utilizado en cables de red Ethernet.

Patch cord: Cable corto que conecta el patch panel con el switch o un equipo final.

Canal de comunicación: Ruta completa que sigue la señal, incluyendo cables, conectores y dispositivos intermedios.

Topología de red: Forma en que están organizados los dispositivos y conexiones en una red.

Latencia: Tiempo que tarda un paquete de datos en viajar de un punto a otro.

Interferencia electromagnética (EMI): Perturbación causada por campos eléctricos o magnéticos que afecta la señal en los cables.

Interferencia de radiofrecuencia (RFI): Tipo de interferencia causada por señales de radio que pueden afectar el rendimiento del cableado.

Blindaje (STP/FTP): Protección adicional en los cables para reducir interferencias:

• UTP: sin blindaje  
• STP/FTP: con blindaje  

UTP (Unshielded Twisted Pair): Tipo de cable de par trenzado sin protección contra interferencias externas.

Mapa de cableado (Wiremap): Resultado que muestra el orden y conexión de los pares dentro del cable.

Open (abierto): Falla donde un cable está cortado o no hace contacto.

Short (corto circuito): Falla donde dos conductores hacen contacto indebido.

Split pair: Error donde los cables están conectados en los pines correctos pero no en los pares correctos, generando interferencia.

Margen de error: Valor que indica qué tan cerca está un enlace de fallar respecto al estándar.

Certificación PASS/FAIL: Resultado de la certificadora indicando si el enlace cumple (PASS) o no (FAIL) con los estándares.

Frecuencia de operación: Rango de frecuencias en el que trabaja el cable, relacionado con su categoría.

Backbone: Parte principal de la red que conecta diferentes segmentos o áreas.

Punto de consolidación: Lugar intermedio donde se agrupan conexiones antes de llegar al destino final.

Canal vs enlace permanente:

• Enlace permanente: cableado fijo dentro de la instalación  
• Canal: incluye patch cords y conexiones finales  

Identificación de fallas:

Proceso de localizar problemas específicos en el cableado o dispositivos.
