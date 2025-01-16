# Andres Molina González
# Testing en Producción

## 1. Evaluación inicial de estándares y navegación

El proyecto elegido es de mi compañero Angel. https://animangadatahub.netlify.app/ Que es una de las mas completas.

### ¿Cuáles no cumplen con las pautas de usabilidad?  
A pesar de que la página cumple con los estándares mencionados, no satisface completamente algunas pautas de usabilidad:  
- **Tiempos de carga elevados** en ciertos recursos, lo que puede dificultar la interacción inicial para usuarios con conexiones más lentas.  
- **Elementos interactivos** que no siempre son intuitivos para todos los perfiles de usuarios, lo que puede complicar la experiencia en algunos casos.

### ¿Cómo es la facilidad de navegación del sitio web con diferentes periféricos?  
- **Ratón**: La navegación con ratón es excelente. Los enlaces y botones son claramente visibles y accesibles.  
- **Teclado**: La navegación con teclado funciona correctamente. Se pueden recorrer los elementos interactivos usando la tecla **Tab**, y no se detectaron problemas de accesibilidad básicos.   

 
El uso de estándares en el desarrollo web es esencial para garantizar la accesibilidad, el rendimiento y la experiencia del usuario. Esta página muestra un buen nivel de cumplimiento en estos aspectos y facilita la navegación con diferentes periféricos, salvo el detalle de los tiempos de carga elevados. Resolver este punto permitirá optimizar la experiencia y mejorar la interacción en dispositivos y redes menos rápidas.

## **Webpagetest**
### Móvil Chrome 

![alt text](image-1.png)

La primera prueba la realice en Chrome con un emulador de Motorola.

![Imagen donde a](image.png)

De primera mano nos muestra lo mas importante.

Velocidad de carga: El informe señala que la página no tiene un mal rendimiento, pero hay áreas a optimizar, como las solicitudes bloqueantes y el tiempo de renderizado del contenido principal.

Usabilidad: Se identifican problemas críticos, como una lenta interactividad inicial y tres problemas de accesibilidad. Esto evidencia la necesidad de seguir estándares en el desarrollo para evitar retrasos y problemas para usuarios con discapacidades.

Resiliencia: Aunque no hay fallas de seguridad, se mencionan dependencias de terceros que podrían comprometer la estabilidad de la página.

![alt text](image-3.png)

Esta imagen muestra el análisis técnico detallado de la carga del sitio web, dividido en tres áreas:

Waterfall: Representa todas las solicitudes de recursos realizadas (HTML, CSS, JavaScript, imágenes y fuentes). El desglose por tiempos de espera, conexión y renderizado permite identificar cuellos de botella.

Captura de pantalla: Refleja el estado final del sitio una vez completamente cargado. Este elemento asegura que el diseño y contenido son consistentes en diferentes dispositivos.

Gráficos de contenido: Proporcionan un desglose porcentual de los recursos descargados, destacando que JavaScript ocupa el 22.8% del tráfico total. Esto sugiere áreas de optimización para mejorar la velocidad de carga. Lo que mas consume son las imagenes con un 47,9%. 


![alt text](image-2.png)


En esta imagen se detalla el proceso de carga del sitio en intervalos específicos:

Filmstrip: Muestra cómo la página progresa desde el inicio hasta estar completamente cargada . Esto permite identificar tiempos muertos o problemas en la visualización inicial.

Waterfall detallado: Incluye todas las solicitudes realizadas, destacando los tiempos de espera y ejecución. Los gráficos de CPU y ancho de banda revelan picos en el procesamiento y la importancia de optimizar fuentes e imágenes.

Evaluación de interactividad: El desglose temporal identifica problemas que retrasan la experiencia del usuario, como la carga de scripts externos.

### Escritorio Mozilla Firefox

![alt text](image-4.png)

Ahora lo hacemos en un escritorio normal con el Firefox

![alt text](image-7.png)

Como anteriormente la velocidad de carga y la usabilidad es muy parecida. Lo unico que cambia es la resiliencia.

Resiliencia: ¡Se ve genial! Este sitio no tenía solicitudes de terceros que bloquearan la visualización y que pudieran ser un punto único de falla. No tenía problemas de seguridad.

![alt text](image-5.png)

Esta vez tardo 1 segundo y medio menos que anteriormente. Es decir que por el dispositivo o por el navegador se funciona mejor la página web.

![alt text](image-6.png)

Como anteriormente podemos ver el Waterfall que es lo que he mostrado anteriormente, los gráficos proporcionan un desglose porcentual de los recursos descargados, destacando que las imagenes ocupa el 64,1% del tráfico total. Esto sugiere áreas de optimización para mejorar la velocidad de carga.

## PageSpeed Insights
### Home
#### Movil
![alt text](image-8.png)
El home en el movil tiene un rendimiento medio malo con la primera carga en 5 segundos, y el maximo en cargá tardo 8,4 segundos 
#### Escritorio
![alt text](image-9.png)
En escritorio tuvo un rendimiento bueno con la mayor tardanza en 1,4 segundos.
### Listado
#### Movil
![alt text](image-13.png)
El listado en el movil ha ido un poco mejor que el de home, pero aun asi no esta del todo bien todavia.
#### Escritorio
![alt text](image-14.png)
El listado en el escritorio esta muy bien tiene
### Producto
#### Movil
![alt text](image-18.png)
En el producto en el movil tiene un mal rendimiento de carga y puede ser tedioso para los usuarios.
#### Escritorio
![alt text](image-11.png)
En cambio en el escritorio puede ser muy bueno porque tiene un buen rendimiento.

## Optimización con Lighthouse
Con la extension Lighthouse me da estos resuultados.
![alt text](image-17.png)

![alt text](image-19.png)

Tiene una gran carga de elementos y tarda en cargar completanente.

![alt text](image-21.png)
tiene una buena accesibilidad pero tiene dos pequeños fallos faciles de solucionar.