
# Sistema de mensajería segura para Organizaciones Civiles de Protección de Derechos Humanos y Libertad de expresión.

En el contexto de espeionaje que se vive hoy día en el internet  en contra de periodistas y activistas de distintas organizaciones de derechos humanos que ha sido comprobado por varias organizaciones como R3D, y Citizen Labs, la importancia de las telecomunicaciones digitales seguras se vuelve una cuestión crucial en el quehacer diario de periodistas y defensores de derechos humanos. Es indispensable contar con aplicaciones digitales de mensajería segura para asegurar la no intercepción de las comunicaciones por terceros. Es necesario asimismo que este sistema de mensajería sea auditable y que se encuentre en manos de la organización.Esto involucra varios retos tecnológicos y organizativos  cuando se plantea el despliegue de un sistema de comunicación seguro. 

En este caso se desarrolla una propuesta de un sistema de mensajera seguro, sus pros y sus contras. El objetivo final del proyecto es conseguir un sistema de comunicación en chat multiplataforma que sea similar a los usados en otros servicios comerciales como son WhatsApp o Telegram. Adaptándolo a las necesidades de comunicación y seguridad de la organización. 


## Fases del proyecto:

- Fase de reconocimiento (2 semana):

Esta fase será implementada para conocer las necesidades de la organización y trabajar en un diseño técnico que se adecuado al tamaño, visión a largo plazo, y el propósito que la organización de Derechos Humanos tenga del sistema de comunicación. Sorebtodo identificar el nivel de vulenrabilidad de la organización. así como la sensibilidad de la información manejada por la organización. Por lo que se pedirán datos básicos, en cuanto al número de integrantes de la organización, los equipos de computo manejados, los celulares, y las prácticas de uso de la tencología. 

 - Fase de implementación y pruebas ( 3 semanas):

Es sobretodo una fase técnica en donde se van a tener instalados y puestos a puntos los servicios tecnológicos que van a constituir el sistema de comunicación de acuerdo a  la información obtenida en la anterior fase. Se va a mostrar el prototipo del sistema de comunicación para la evaluación de este mismo desde el punto de vista del personal de la organización, dirigido a ver la usabilidad del mismo y la utilidad en el quehacer diario de la organización. Asimismo se estará abierto a las críticas que se le pudan hacer al sistema de mensajería.

- Fase de reingeniería ( varia dependiendo de las críticas y los desarrollos recopilados durante la anterior fase):

Se implementan las mejoras o modificaciones técnicas que en la medida de lo posible sugieran los miembros de la organización.

- Fase de capacitación ( de 2 a 3 semanas)

Es la fase final del proyecto, en donde nos aseguramos de capacitar a todo el personal tanto el uso  tecnológico del sistema de comunicación, como en la capacitación en seguridad digital a nivel protocolario y personal. Haciendo que sea integral la formación de la implementación del sistema de comunicación. El objetivo es integrar prácticas de autodefensa digital dentro de la organización. 


## Propuesta tecnológica.

Se propone la siguiente arquitectura. El corazón del sistema de comunicaciones será un servidor  XMPP para la tranmisión de 
mensajes de texto y voz, as como imagenes. XMPP es un estandard internacional reconocido por la IETF (Internet Engineering Task 
Force), sobre las transmisiones de video, audio y chat por internet. Es un estandárd abierto y reconocido internacionalmente  
como uno de los protocolos a ser usados globalmente en internet. Actualmente es usado en varios servicios de comunicación como 
son Google Talk y el chat de Facebook. El nivel de seguridad de este estandar es máximo ya que lleva en uso ms de 10 años y se ha 
establecido como uno de los protocolos estandard de intenret junto con el http, el protocolo usado para la transmisión de 
información desde el navegador web.

La implementación de un servidor que maneje las comunicaciones internas por chat de la organizacin tiene el objetivo de evitar la 
centralización de servicios de terceros como puede ser WhatsApp, además de asegurar que los datos sensibles permanezcan bajo 
control, legal y práctico de la organización. Para ello se sugieren las suguientes medidas:

- Contratar un servidor en un país que tenga un estandard alto de cumplimiento a los derechos humanos. Además de que el proveedor 
debe tener experiencia en el hosteo de ONGs dedicadas al activismo en derechos humanos. 

- Definir las responsabilidades de la persona que posea la entrada a los datos del servidor.

## Servidor XMPP.

- Sistema Operativo Debian. 

Debian es una fundación en Alemania, que provee una de las distribuciones Linux mas viejas y conocidas del mundo. Esta 
organización es responsable de proyectos que apoyan la libertad de expresión como FreedomBox. Asimismo la estabilidad y seguridad 
de su sistema operativo son como pocos, gracias a los estándares abiertos y la estructura organizativa de la organización.

Las medidas de seguridad digital a nivel tecnológico que serán implementadas son:

-El hardening del kernel, logrando que el sistema operativo del servidor sea resistente a  ciberataques.
-Simplicidad de los servicios, por lo que el servidor contará solo con el servicio exclusivo de XMPP, con el fin de simplificar 
la arquitectura atendiendo a los principios para la seguridad digital. 
 Asegurando así la disponibilidad y seguridad de la información dentro del servidor. 
- Hardening y auditoría previa del sistema operativo. Además de tomar las medidas de seguridad convencionales, como la aplicación 
de parches de seguridad a nivel informático.
- La implementación de una arquitectura dentro del servidor que asegure que los datos sensibles no sean facilmente accesibles ni 
modificables por parte de terceras personas. 
- Protección ante ataques de denegación de servicio, y otro tipo de ataques informáticos.
- Realización de pruebas de intrusión hacia el servidor. 

Todas estas medidas serán adecuadamente documentadas y entregadas a la organización con el objetivo de que se pueda asegurar la 
fiabilidad del servicio.

- Prosody como servidor XMPP.

Un servidor minimalista diseñado para organizaciones pequeñas. El minimalismo contribuye también ala seguridad digital. Se usarán en todo momento certificados SSL.

Estos requisitos pueden variar dependiendo del proyecto y de acuerdo a la información recolectada y los requerimientos de la organizaición.

## Clientes ( Aplicaciones para celulares y Escritorio)

Arquitectura de los clientes:

Se instalará un cliente en cada una de los sistemas operativos usados por los miembros de la organización, atendiendo a los 
sistemas de computadoras personales, y los de los teléfonos inteligentes, asegurándose la interoperabilidad de los clientes.
Se usará la aplicación de Android Conversations. 

También se asegurará la privacidad de las comunicaciones, usando cifrado End To End o cliente a cliente. Para lograr que el 
servidor sirva como un simple transmisor de comunicaciones y no queden guardados registros en el caso de un ataque cibernético. 
Este cifrado es equivalente al que ofrecen servicios como Telegram con el chat seguro y WhatsAPP con la implementación del 
cifrado seguro. 

Asimismo se capacitará al personal de la organización en el uso de estos cifrados,a saber OTR y OMEMO. 

Para los clientes en dispositivos Android se usará Conversations. Mientras que para clientes en equipos de Escritorios Gnu/linux y Windows se usar el cliente Gajim. No se recomienda el uso de dispotivos IOS por sus estándares de seguridad, sin embargo de haberlos se propondrá una solución para estos. 

Estos requisitos pueden variar dependiendo del proyecto y de acuerdo a la información recolectada y los requerimientos de la organización.

### Seguridad de la información transmitida.

Toda la información entre clientes y servidor viene cifrada por TLS el estandar de cifrado de internet (equivalente al https). Adicionalmente están disponibles otros dos tipos de cifrado END to END, es decir que la información va cifrada desde que el dispositivo de una persona lo envia, hasta que el dispositivo de laotra persona lo recibe. Esto tiene como consecuencia, que en el servidor no se guardan datos.

### Desventajas y ventajas en cuanto a la seguridad digital del sistema de mensajera propuesto.
    
#### Desventajas

    - Clientes no sincronizados cuando usen cifrado OTR. ( Es el caso por ejemplo de los chats secretos de Telegram que solo se 
    pueden tener en un solo dispositivo)
    - La disponibilidad del servidor determina la disponibilidadl de servicio
    - 0 days en el protocolo XMPP o el servidor XMPP. ( Este procolo tiene más de 10 años en funcionamiento y es auditado por la IETF   
    por lo que se espera que este no  sea un riesgo importante, además de que en todo caso tambin serían vulnerables las aplicaciones como Signal, Telegram o WhatsAPP)

#### Ventajas.

    - Cifrado cliente a cliente con OMEMO, el mismo cifrado usado por Signal y WhatsAPP.
    - Control sobre el servidor.
    - La Base de datos permanece bajo jurisdicción de la organización
    - El Control de la información  se queda en la organización.
    - Auditable en caso de duda.
    - Se pueden fincar responsabilidades legales, si se tiene evidencia de hackeo.
    - Se define un círculo de confianza dentro de la organización con las personas que tienen acceso a la información.

### Seguridad en la organización.

Las medidas de seguridad a nivel protocolar, será la implementación y capacitación del personal no solamente en el uso del 
sistema, sino en la introducción a la autodefensa digital, por medio de incidir en las practicas tencologicas de la organización, 
así como crear conciencia en cuanto a la prevención de ataques cibernéticos. A

### Consideraciones adicionales. 

El sistema  de mensajería propuesto puede servir a nivel técnico para aumentar las capacidades de la organización para realizar 
su trabajo, sin que se ceda el control de las comunicaciones a terceros. Asimismo, puede extenderse para manejar una buena 
cantidad de personal sin necesidad de expandir la infraestructura. Los servidores XMPP pueden ser extendidos incluso para manjear 
audio y tranmisión de video. Por lo que contar con una infraestructura de comunicación sólida, puede extender las capacidades de 
la organización a largo plazo.


## Bibliografía.

Internet Engineering Task Force, https://www.ietf.org/
XMPP, https://xmpp.org/
Electronic Frontier Foundation, Secure Messaging scorecard, https://www.eff.org/secure-messaging-scorecard, 13 junio 2017
EFF, Surveillance self Defense, https://ssd.eff.org/ consultado 13 junio 2017
