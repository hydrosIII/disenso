# Pruebas realizadas para ofrecer el servicio de Chat Seguro.

## Clientes

El chat seguro depende de la implementación y qué tan completa es la implementación de los clientes. 

Es este caso se probaron los clientes gajim en linux.


En android se probaron los clientes Wom, Chat Secure y Conversations. Siendo Conversations el más completo.

Conversations es bueno pero tiene el defecto de que cuesta en la App Store, sin emabrgo se puede compilar ya que
existe el código fuente de manera independiente. 

Gajim, es el cliente más completo de Linux, sobre todo porque es el que soporta cifrado OMEMO, ya que lo que se busca en 
la implementación es la seguridad. Este cliente, sin emabrgo, tiene algunos errores como que no es posible agregar 
grupos de chat para que se queden de forma permanente.

## Servidores

### Ejabberd
Se probó el servidor ejabberd, el cual está construido para grandes desarrollos, ya que soporta 
caractersticas como la clusterización y la federación de servicios. Además, éste tiene una interfaz web ( que no 
es fácil de usar para el usuario final ) con la cual se pueden configurar algunas de las características del 
servidor. El servidor está escrito en Erlang, me parece que por lo asíncrono del lenguaje de programación. 

Las pruebas fueron hechas en Gnu/linux Debian 9, que es la última versión. Escogí ejabberd porque estaba dentro de 
la distribución Debian, lo que siginfica que entra dentro de las acutlaizaciones de seguridad de la misma 
distribución, algo que considero bastante importante. 

Parece ser que tiene integrada una base de datos para guardar tanto los usuarios como los mensajes. Pero soporta 
la conexión con otras bases de datos como Mysql y Postresql. En todo caso me parece que esto depende del 
tamaño de la implementación. 

### Prosody.

Este servidor es minimalista, y está diseñado para implementaciones pequeñas, no posee por ejemplo una interfaz 
web y el agregar usuarios se hace mediante comandos (una desventaja). Desconozco si existen UIs web que se puedan 
usar con este servidor para este fin. Me parece que el control de usuarios y quien usa el servidor es algo 
fundamental en este proyecto, ya que así se puede garantizar la privacidad de las conversaciones. 

Está escrito en Lua.

Este servidor también viene incluido en Debian. 

### Openfire

Este servidor promete ser fácil de configurar. No lo he checado. 


http://download.igniterealtime.org/openfire/docs/latest/documentation/install-guide.html



## Documentos a consultar para la implementación de este servicio:

### Servicios ya disponibles y sus defectos:

https://ssd.eff.org/en/module/how-use-whatsapp-android
https://www.eff.org/secure-messaging-scorecard

### El caso de Signal.

https://stackoverflow.com/questions/33699970/run-custom-textsecure-signal-server/34471995#34471995

### XMPP.

Pagína oficial:

https://xmpp.org/

Libro:
https://oriolrius.cat/blog/wp-content/uploads/2009/10/Oreilly.XMPP.The.Definitive.Guide.May.2009.pdf

### Implementaciones criptográficas.

- Omemo. 

https://es.wikipedia.org/wiki/Omemo

- OTR. ( solo funciona para chats de 2 personas)

https://es.wikipedia.org/wiki/Off_the_record_messaging

- PGP ( este si puede ser usado en chats de varias personas pero no es tan obvio de usar).
https://es.wikipedia.org/wiki/Pretty_Good_Privacy


## Seguridad de la información transmitida.

Toda la información entre clientes y servidor viene cifrada por TLS que es lo más seguro. Así que creo que no hay problema.

En el chat sin OMEMO PGP u OTR, el texto se quedan guardadas en el servidor en la base de datos.  Esto no es mucho problema ya que el servidor es seguro y está bajo control de la organización. Sim embargo, en el caso de un hackeo al servidor ( caso remoto pero posible) la info de los mensajes se podrá encontrar sin cifrar.

- soluciones. Vaciar la base de datos de mensajes, periódicamente.
- Usar OMEMO, PGP  u OTR.

Con las imagenes, como se envian aparte, se guardan en otro directorio y permanecen allí, habría que implementar cifrado.


Parece ser que conversations en Android, viene también con SQlite para guardar los datos, no sé si tenga algún protocolo para cifrar con contraseña. Esto haría más dificl el robar datos. Parece ser que chat secure sí lo tiene. Hay que analizar la estrctura de seguridad de los clientes.

