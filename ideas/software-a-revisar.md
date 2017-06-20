# Principios:

No reinventar la rueda. Usar software y tecnología que se nutra de comunidades, OSC's y empresas que han sido 
probadas y estén bien establecidas. Además de siempre intentar usar software estandár e intentar no hacer cambios específicos en los desarrollos que no se puedan poner en el proyecto principal. Con esto nos aseguramos de poder ofrecer una amplia 
variedad de servicios. Cuando sea necesario hacer modificaciones al software o adaptaciones se tiene que evaluar el 
costo-beneficio y si es posible devolver estas contribuciones a su desarrollo principal.

## Proyectos de software a revisar para servicios e ideas que me parecen interesantes y con las que me identifico.

- Ushahidi. 

Este software ha sido usado en Kenya para el monitoreo de elecciones y además el monitoreo de desastres naturales. 
Actualmente esta siendo usado para el proyecto rutasdelamemoria.org. Es un software de geolocalización y mapeo.

- XMPP sus protocolos y redes. 


XMPP como protocolo se usa desde chats seguros, telefonía VOIP, aplicaciones de video straeming. Hasta en las redes 
sociales federadas. La última vez que chequé a red Mastodont era la más popular. 

- Redes sociales descentralizadas. 

En lo personal no les veo mucho futuro debido a los gigantes de la tecnología han centralizado las redes 
sociodigitales, pero quizá habría que evaluar por caso. Mastodont creo que está creciendo y hay otra llamada 
Quitter. Que yo sepa ninguna es viable todavia. 

- Odoo y Tryton.

Odoo ahora ya está bastante separado del proeycto Tryton, pero en un ERP que es comunitario y tiene algunos módulos 
para ONGS también. Además esta siendo cada vez más implementado en empresas. He trabajado con odoo 3 años.

https://www.odoo.com/

Odoo hoy también incluye e-commerce.

Hay una fundación que produce módulos gratuitos. 

https://odoo-community.org/

Tryton es usado sobretodo en hospitales. 

http://health.gnu.org/

- El proyecto Kolibri, es un proyecto de software educacional que intenta llevar conetenidos educaciones a lugares 
con poco acceso a internet.

https://learningequality.org/kolibri/

- Owncloud y similares. 

https://owncloud.org/

Es un Software que sustituye a Dropbox. También lo he usado.

https://cryptpad.fr/

Sofware para almacenar cosas de manera cifrada.

- CMS

 Aquí pueden ser desde Wordpress y otros para instalar blogs, sin emabrgo esta área ya esta muy automatizada. Pero siempre se puede vender el diseño de blogs y cosas que van más por lo artístico. O ofreciendo por ejemplo servicios de seguridad alrededor de las páginas. 

- Paginas seguras. 

Guthub pages ofrece hosting gratuito y seguro para muchas páginas web. Está limitado por que no ofrece https. Pero 
ofrecer este tipo de servicio a ONGs con bajo presupuesto se me hace una buena idea. La limitación es que son páginas estáticas. 
Software como Jekyll hace posible ahcer blogs pero solo a usuarios técnicos. 

- Servidores de radio y podcat para tranmisión en vivo de voz y video.

Para medios de comunicación, por ejemplo mediagoblin.


## Software de infraaestructura.


- Docker y similares. 

Docker y otros proyectos autoamizatizan el manejo de servidores y aplicaciones dentro de ellos haciendolos mas 
seguros, la desventaja es que aún no está tan probado y es relativamente nuevo. Pero es una manera de lograr 
desarrollos que consistan en sumar las partes de un sistema de manera inteligente y sobretodo repetible.
Llevo probándolo unos meses, pero por ahora no he tenido oportunidad de probarlo con algo serio. 

Este proyecto ya tiene Red Hat Atomic y distros como CoreOS que se centran en meter contenedores me parece que se puede integrar 
perfectamente con ofrecer microservicios especializados y seguros.

- Debian

Se manejar bien Debian en servidores. Otros linux como Centos/RedHAt no los manejo al mismo nivel pero lo hago. También en 
escritorio. Lo interesante son las implementaciones de LUKS (cifrado entero de disco) para escritorio que hacen de Linux
+ LUKS un producto a ofrecer. 

- Alpine linux. 

 Es una distro linux para seguridad tambien en servidores. Me gusta. Actualmente ando checando que tan bien funciona con docker.
 
 - Arch linux
 
 Lo uso diario.
 
 - Proxmox 
 
 Es debian con LXc y KVM, consecuentemente he aprendido sobre virtualización.También he trabajado sobre VMWARE que es mas 
 empresarial y propietario, pero visto desde lejos son parecidos.
 
 - Bases de datos. 
 
 Al final he aprendido operaciones básica de administración de base de datos. Mysql y Postgres han sido las que más he usado, 
 aunque he llegado a manejar Oracle. No soy fan. En todo caso soy familiar con como se usan, su estructura y alto de migración de estas bases. 

## Servicios empresariales de infraestructura.

Todos los servicios que se deriven de la revisión y/o instalación de software arriba citado, pueden ser ofrecidos 
de manera segura a empresas. Estos constarían sobretodos de servicios de infraestructura.

Por ejemplo:

Yo uso Proxmox que es un servidor de virtualización, para probar aplicaciones, por lo que se podría ofrecer para un 
servicio empresarial, por ejemplo de virtualización de aplicaciones ya existentes en algunas empresas. En todo caso 
los servicios derivados de los de arriba se pueden ir ofreciendo. 

También uso bastantes redes y ahora trabajo son software como OPENVPN y otro tipo de servicios además de 
distribuciones enteras como es PFsense que es para routeo de paquetes y seguridad de redes. 

En resumen servicios empresariales:

- Servicios de virtualización y contenirización  de aplicaciones. Usando Proxmox, docker, LXC y KVM entre otras 
tecnologías de contenedores.
- Servicios de configuración de Redes. 
- Servidores de archivos y NAS. Open Source como FreeNAS.


Todos estos conocimientos han nacido con base en las cosas que se van ofrecieno como servicios mas especializados 
como es el caso del chat seguro.
