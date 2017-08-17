---
title: Comunicándote Con Otros
date: "2017-02-01T19:20:04-07:00"
---

# Comunicándote Con Otros

Las redes de telecomunicación y el Internet han hecho la comunicación con otros mas fácil que nunca, sin embargo, han hecho la vigilancia mas prevalente en la historia de la humanidad. Sin tomar pasos extras para proteger tu privacidad, cada llamada telefónica, cada mensaje de texto, email, mensaje instantáneo, llamada de voz sobre IP (VoIP), video charla, y mensaje en la red social podrían ser vulnerables a la escucha secreta.

Muchas veces la mejor manera de comunicarte con otros es en persona, sin involucrar computadoras o teléfonos. Sin embargo, ello no es siempre posible. Si necesitas proteger el contenido de tu comunicación, el otro medio preferido para comunicarte a través de una red es el uso del cifrado de punto-a-punto (“end-to-end encryption”)

### ¿Cómo Trabaja el Cifrado de Punto-a-Punto?

Cuando dos personas quieren comunicarse de manera segura (por ejemplo, Akiko y Boris) ambos necesitan generar una llave de cifrado. Antes que Akiko envíe un mensaje a Boris, ella cifra su mensaje con la llave de Boris; así solo Boris podrá descifrarlo. De esta forma, lo que Akiko hará es enviar el mensaje ya cifrado vía Internet. Si alguien está escuchando a escondidas a Akiko y Boris-- inclusive sí el atacante tiene acceso a los servicios que Akiko está usando para enviar sus mensajes (tales como su cuenta de email)--los atacantes sólo podrán ver la información cifrada y no podrán leer el mensaje. Cuando Boris reciba el mensaje, él debe de usar su llave de cifrado para descifrar el mensaje y hacerlo legible.

El cifrado de punto-a-punto involucra algunos esfuerzos adicionales, pero éstos son la única manera para que el usuario puede verificar la seguridad de sus comunicaciones sin tener que confiar en la plataforma que ambos están usando. Algunos servicios como Skype dicen que ofrecen al público servicios de cifrado de punto-a-punto cuando en la realidad ellos no los ofrecen. Para que un cifrado de punto-a-punto sea seguro, los usuarios deben poder verificar que la llave cifrada, a la que ellos están enviando el mensaje cifrado, pertenece a la persona que ellos creen le pertenece. Si el software no lleva esa funcionalidad construida dentro de si mismo, entonces cualquier mensaje cifrado podría ser interceptado por el mismo proveedor de servicio, de hecho ellos estan obligados hacerlo, por ejemplo si el gobierno se lo requiere.

Puedes leer el reporte de La Fundación de Libertad de Prensa (Freedom of the Press Foundation's whitepaper), Encryption Works para detalles e instrucciones de como usar cifrado de punto-a-punto para proteger mensajes instantáneos y email. Asegúrate de mirar también los siguientes módulos de SSD:

 * Una Introducción a la Criptografía de Llave Pública y PGP

 * Cómo Usar OTR para PC

 * Cómo Usar OTR para Mac

### Llamada de Voz

Cuando haces una llamada desde un teléfono fijo o desde un móvil, tu llamada no es cifrada de punto-a-punto. Si estás usando un teléfono móvil, tu llamada puede ser cifrada (de forma débil) entre tu equipo y las torres de telefonía celular. Sin embargo, como la comunicación está viajando a través de las redes telefónicas, las mismas se hacen vulnerables a interceptaciones por parte de la compañía telefónica, del mismo modo que es vulnerable frente a cualquiera otra rama del gobierno, organización, o institución que tenga poder sobre la compañía. La manera mas fácil de asegurarte que tienes el sistema de cifrado de punto-a-punto en una conversación de voz, es usando en su lugar, el sistema VoIP (Voz-sobre-el Protócolo de Internet).

<aside class="warning">
¡Ten cuidado! Los proveedores mas populares de VoIP, tales como Skype y Google Hangouts, ofrecen transporte de cifrado que los atacantes que vigilan a escondidas no pueden oír, pero los mismos proveedores tienen la capacidad técnica de escuchar la conversación. Dependiendo de tu modelo de amenaza, esto podría ser o no un problema.
</aside>

Algunos de los servicios que ofrecen cifrado de punto-a-punto de llamadas VoIP incluyen:

 * WhatsApp
 * Signal
 * Jitsi 
 * Silent Phone
 * Zphone

Para poder tener una conversación VoIP cifrada de punto-a-punto, ambos lados tienen que usar el mismo software o software compatible.

### Mensajes de Texto
Los mensajes de texto estándar no permiten el cifrado de punto a punto. Si quieres enviar mensajes cifrados desde tu teléfono, piensa en utilizar un programa de mensajería instantánea cifrada en vez de mensajes de texto.

Algunos de estos servicios de mensajería cifrada de punto a punto utilizan su propio protocolo. Por eso, por ejemplo, los usuarios de Signal sobre Android e iOS pueden chatear con seguridad con otras personas que utilizan esos programas. ChatSecure es una aplicación para móviles que encripta conversaciones con OTR sobre cualquier red que utilice XMPP, lo que implica que puedes elegir entre una variedad de servicios de mensajería instantánea independientes.

### Mensajes Instantáneos

Los mensajes “Off-the-record", comúnmente llamado OTR, es un protócolo de cifrado de punto-a-punto para conversaciones de textos en tiempo real (al momento), el cual puedes usar sobre una variedad de servicios.

Algunas de las plataformas que incorporan OTR con mensajes instantáneos incluyen:

 * Pidgin (para Windows or Linux)
 * Adium (para OS X)
 * ChatSecure (para iPhone y Android)
 * Jitsi (Linux, Windows, Mac OS)

### Email

La mayoría de los proveedores de email proporcionan una forma de acceso a tu email usando un navegador de web, tales como Firefox o Chrome. De estos proveedores, la mayoría apoyan los protócolos HTTPS, o transporte de cifrado en capa (“transport-layer encryption”). Puedes saber si tu proveedor de email soporta HTTPS si ingresas a tu Webmail y el URL (en la parte superior de tu navegador) comienza con las letras “HTTPS” en vez de “HTTP” (por ejemplo: https://mail.google.com).

Si tu proveedor permite HTTPS, pero no lo hace por defecto, trata de reemplazar HTTP con HTTPS en la URL , y actualiza la página. Si quieres estar seguro que siempre estás usando HTTPS en los sitios donde HTTPS esté disponible, baja el HTTPS Everywhere, un “plug-in” para el navegador de Firefox o Chrome.

Algunos proveedores de webmail que usan HTTPS de manera estándar incluyen:

 * Gmail
 * Riseup
 * Yahoo

Algunos de los proveedores de webmail que le dan la opción de escoger el uso de HTTPS de manera estándar en sus ajustes. El servicio mas popular que todavía lo ofrece es Hotmail.

¿Qué hace el protócolo de transporte de cifrado en capa (“transport-layer encryption”)? y ¿por qué podrías necesitar éste? HTTPS, es también denominado SSL o TLS, éste cifra tu comunicación, y de esa manera no puede ser leída por otras personas en tu red. Estos pueden incluir otras personas usando el mismo Wi-Fi en un aeropuerto o en un café, las otras personas en tu oficina o escuela, el administrador en tu ISP, crackers malignos, gobiernos, e oficiales del órden público.

Un atacante puede fácilmente interceptar y leer las comunicaciones que envias sobre tu navegador web, incluyendo las páginas web que visitas y el contenido de tus emails, entradas de blog, y mensajes si usas HTTP en vez de HTTPS.

HTTPS es el nivel mas básico de cifrado para tu navegador que le podríamos recomendar a todo el mundo. Es tan básico como el ponerse el cinturón de seguridad cuando manejas.

Pero hay algunas cosas que el HTTPS no hace. Cuando envías un email usando HTTPS, tu proveedor de email también recibe una copia descifrada de tu comunicación. El gobierno y las fuerzas del orden público podrían tener acceso a esta información con una orden judicial, o una citación. En los Estados Unidos, la mayoría de proveedores de email tienen una política de privacidad que dice que ellos te notificaran cuando reciban una solicitud del gobierno para recolectar tus datos, siempre y cuando ellos estén legalmente permitidos, pero estas políticas son estrictamente voluntarias, y en mucho de los casos, los proveedores están legalmente impedidos de informarles a los usuarios sobre la petición de información.

Algunos proveedores de email, tales como Google, Yahoo, y Microsoft, publican un reporte de transparencia, detallando el número de solicitudes por parte del gobierno para obtener información de sus usuarios, que país hizo la solicitud, y cuántas veces la compañía ha obedecido a las solicitudes, entregándoles la información.

Si tu modelo de amenaza incluye algún gobierno o fuerza de orden público o tienes otras razones de querer estar seguro que tu proveedor de servicios de email no entregará tu información a una tercera persona, quizás quieras considerar usar cifrado de punto-a-punto para tus comunicaciones de email.

PGP (o Pretty Good Privacy/Privacidad Muy Buena) es el estandar de seguridad de punto-a-punto para tu email. Usado correctamente, éste ofrece una protección muy fuerte para sus comunicaciones. Para detalles e instrucciones de cómo instalar y usar PGP para cifrar tu email, vea esta sección:

 * Como Usar PGP para Mac OS X
 * Como Usar PGP para Windows
 * Como Usar PGP para Linux

### ¿Qué es lo que un Cifrado de Punto-a-Punto No Hace?

El cifrado de punto-a-punto solo protege el contenido de tu comunicación, no la veracidad de la misma. Este no protege tus metadata, la cual es otra cosa, incluyendo el asunto de tu email, o con quien te está comunicando y cuando.

<aside class="warning">
Los metadatos puede revelar información extremadamente sensible sobre tí inclusive cuando el contenido de tu comunicación se mantiene privada.
</aside>

Los metadatos de tus llamadas telefónicas pueden proporcionar información muy íntima y sensible. Por ejemplo:

Ellos pueden saber que llamaste a un servicio de sexo telefónico a las 2:24 am y habló por 18 minutos, pero no pueden saber que conversaste.
Ellos pueden saber que llamaste a una línea de prevención de suicidio desde el Puente Golden Gate, pero el tópico de la conversación se mantiene en secreto.
Ellos pueden saber que llamaste a un servicio de prueba para VIH, después a tu doctor, después a tu seguro de salud a la misma hora. Pero ellos no pueden saber que discutiste.
Ellos saben que recibiste una llamada desde la oficina local de la Asociación Nacional del Rifle (o su acrónimo en inglés NRA) mientras que ellos desarrollaban tu campaña sobre la legislatura de armas, y llamaste a tu senador y a tus representantes en el congreso inmediatamente después, pero el contenido de esas llamadas se mantienen privadas frente a la intrusión del gobierno.
Ellos saben que llamaste a un ginecólogo, hablaste por media hora, y luego llamaste a la oficina local de Planificación Familiar, pero nadie sabe que conversaste.
Si estás llamando desde un celular, la información de tu localidad es metadatos. En el 2009, el político del Partido Verde en Alemania, Malte Spitz, demandó a la compañía Deutsche Telekom para forzarlos a que le entreguen los metadatos de tu teléfono por un período de seis meses, la cual hizo público en un periódico alemán. La visualización resultante demuestra en detalles la historia de los movimientos de Spitz.

El proteger tus metadatos requiere que utilices otras herramientas, por ejemplo Tor, al mismo tiempo que utilizas el cifrado de punto-a-punto.

Para un ejemplo de cómo Tor y HTTPS trabajan conjuntamente para proteger el contenido de tus comunicaciones y tus metadatos de una variedad de posibles atacantes, tal vez desee echar un vistazo a esta explicación.