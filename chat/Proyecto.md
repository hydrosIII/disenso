
Sistema de mensajería segura para Organizaciones Civiles de Protección de Derechos Humanos y Libertad de expresión.

## Aqupi tenemos que documentar todo lo que ha sido reportado, del caso del espionaje y poner citas a los documentos de CITIZEN lab y otros.

El el ámbito de los derechos humanos es indispensable contar con un sistema de mensajería segura para asegurar la no intercepción de las comunicaciones por terceras personas. Además de contar con un mayor nivel de control y seguridad. Esto involucra varios retos tecnológicos y organizativos  cuando se plantea el despliegue de un sistema de comunicación seguro. 

El objetivo final del proyecto es conseguir un sistema de comunicación en chat multiplataforma que sea similar a los usados en otros servicios comerciales como son WhatsApp o Skype, dependiendo de las necesidades de la organización.


## Aquí tenemos que justificar, las fases humanas del proyecto de seguridad. 

Fases del proyecto:

Fase de reconocimiento:

Esta fase será implementada para conocer las necesidades de la organización y trabajar en un diseño técnico que se adecuado al tamaño, visión a largo plazo, y el propósito que la organización de Derechos Humanos tenga del sistema de comunicación.

Fase de implementación:

Es sobretodo una fase técnica en donde se van a tener instalados y puestos a puntos los servicios tecnológicos que van a constituir el sistema de comunicación de acuerdo a  la información obtenida en la anterior fase. 

Fase de pruebas y retroalimentación:

Esta fase es una fase técnico-organizativa del proyecto, en donde se implementan una serie de pruebas, para probar que el sistema de comunicación sea el adecuado. Se hace la presentación y capacitación básica del sistema de comunicación y se reciben las críticas de los miembros de la organización. 

Fase de reingeniería:

Se implementan las mejoras o modificaciones que en la medida de lo posible sugieran los miembros de la organización.

Fase de capacitación

Es la fase final del proyecto, en donde nos aseguramos de capacitar a todo el personal tanto el uso  tecnológico del sistema de comunicación, como en la capacitación en seguridad digital a nivel protocolario y personal. Haciendo que sea integral la formación de la implementación del sistema de comunicación.

## aquí va toda la investigación que estamos haciendo. Justificando los pors y contras de la solucion de chat seguro. 

Propuesta tecnológica.

Se propone la siguiente arquitectura. El corazón del sistema de comunicaciones será un servidor  XMPP para la tranmisión de mensajes de voz, video y texto.

XMPP es un estandard internacional reconocido por la IETF (Internet Engineering Task Force
), sobre las transmisiones de video, audio y chat por internet. Es un estandárd abierto y reconocido internacionalmente  como uno de los protocolos a ser usados globalmente en internet. Actualmente es usado en varios servicios de comunicación como son Google Talk y el chat de Facebook.

Este servidor se sugiere que este en un país que tenga un estandard alto de cumplimiento a los derechos humanos. Greenhost es un buen proveedor.

# Estas son las medidas que se van a tomar para proteger el servidor.

Arquitectura del servidor.

Sistema Operativo Debian. 
Debian es una fundación en Alemania, que provee una de las distribuciones Linux mas viejas y conocidas del mundo. Esta organización es responsable de proyectos que apoyan la libertad de expresión como FreedomBox. Asimismo la estabilidad y seguridad de su sistema operativo son como pocos, gracias a los estándares abiertos y la estructura organizativa de la organización.

Las medidas de seguridad digital a nivel tecnológico que serán implementadas son:
-El hardening del kernel, logrando que el sistema operativo del servidor sea resistente a  ciberataques.
-Simplicidad de los servicios, por lo que el servidor contará solo con el servicio exclusivo de XMPP, con el fin de simplificar la arquitectura atendiendo a los principios para la seguridad digital. 
 Asegurando así la disponibilidad y seguridad de la información dentro del servidor. 
- Hardening y auditoría previa del sistema operativo. Además de tomar las medidas de seguridad convencionales, como la aplicación de parches de seguridad, o la instalación de un firewall.

## Medidas de protección de los clientes.
Arquitectura de los clientes:

Se instalará un cliente en cada una de los sistemas operativos usados por los miembros de la organización, atendiendo a los sistemas de computadoras personales, y los de los teléfonos inteligentes, asegurándose la interoperabilidad de los clientes.

Los clientes, serán auditados, para asegurar que no tengan fallos graves de seguridad en cuanto al código. 

También se asegurará la privacidad de las comunicaciones, usando cifrado End To End o cliente a cliente. Para lograr que el servidor sirva como un simple transmisor de comunicaciones y no queden guardados registros en el caso de un ataque cibernético.  


## Hay que agregar las consideraciones de cada uno de los cifrados probados (OTR, OMEMO y TLS simple)

Seguridad en la organización.

Las medidas de seguridad a nivel protocolar, será la implementación y capacitación del personal de la organización en el uso correcto del sistema. Así como la concientización de posibles puntos de fuga de información. 

Alguna otra medida especial de seguridad requerida por la organización que sea específica.


Consideraciones adicionales. 

El sistema propuesto puede servir a nivel técnico para aumentar las capacidades de la organización para realizar su trabajo. Asimismo, puede extenderse para  manejar una buena cantidad de personal sin necesidad de expandir la infraestructura por lo que podría ser usado en conjunto como un sistema seguro para otras organizaciones. Además de que como todo software de internet es susceptible de ser usado internacionalmente, dependiendo más de la capacidad organizativa para cuidar las buenas prácticas de seguridad.
