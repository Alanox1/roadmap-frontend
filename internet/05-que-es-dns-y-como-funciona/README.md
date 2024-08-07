# ¿Qué es el DNS y cómo funciona?

El Sistema de Nombres de Dominio (DNS) es una tecnología esencial para el funcionamiento de Internet, y se puede comparar con una guía telefónica. Su principal función es traducir nombres de dominio fáciles de recordar, como www.google.com, en direcciones IP numéricas que las computadoras utilizan para identificar y comunicarse con otros dispositivos en la red.

Imagina que quieres llamar a un amigo, pero solo conoces su nombre y no su número de teléfono. De manera similar, cuando escribes un nombre de dominio en tu navegador, este envía una solicitud a un servidor DNS para obtener la dirección IP correspondiente. El servidor DNS actúa como una guía telefónica, buscando en sus registros el "número de teléfono" (dirección IP) asociado al "nombre" (dominio) que proporcionaste.

El servidor DNS primero revisa su caché para ver si ya tiene la dirección IP del dominio solicitado. Si no la tiene, inicia una serie de consultas para encontrarla. Primero, consulta a uno de los servidores raíz del DNS, que tienen información sobre dónde encontrar los servidores que manejan dominios de nivel superior, como .com o .org. El servidor raíz responde con la dirección de un servidor de nivel superior (TLD) adecuado. Luego, el servidor DNS consulta a este servidor TLD, que responde con la dirección de un servidor autoritativo para el dominio específico, en este caso, google.com.

El servidor autoritativo es el que finalmente tiene la información definitiva sobre la dirección IP del dominio solicitado. El servidor DNS consulta a este servidor autoritativo y recibe la dirección IP correspondiente, que luego devuelve a tu navegador. Con esta dirección IP, tu navegador puede establecer una conexión directa con el servidor web de google.com y cargar la página solicitada.

Este proceso ocurre en fracciones de segundo y es transparente para el usuario. El DNS permite una navegación web más amigable y eficiente al permitirnos usar nombres fáciles de recordar en lugar de largas y complicadas direcciones IP numéricas. Además, el DNS es escalable y redundante, lo que significa que puede manejar grandes volúmenes de tráfico y sigue funcionando incluso si algunos servidores fallan, garantizando la disponibilidad y confiabilidad del servicio de resolución de nombres en Internet.

## Páginas que me sirvieron: 

- [Cloudflare](https://www.cloudflare.com/es-es/learning/dns/what-is-dns/#:~:text=El%20DNS%20traduce%20los%20nombres,equipos%20pueden%20usar%20para%20encontrarlo.) 
- [NeoAttack](https://neoattack.com/neowiki/dns/) 
