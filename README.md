Primer Parcial Conmutación y teletrafico 


<img width="583" height="194" alt="imagen" src="https://github.com/user-attachments/assets/b06eaa64-f69d-4b1d-bee1-4da957a704d9" />

La latencia es un proceso que habla de cuanto tarda en milisegundos un determinado paquete en ir y regresar dentro de una determinada red, el jitter es la diferencia en tiempo en relación de los paquetes nos habla de la relación de tiempo con la cual llega cada paquete, en términos de funcionalidad en una comparación ambos escenarios crean un ambiente de degradación en un sistema de telecomunicaciones ya que una latencia alta genera una caída inmediata de la voip mientras que un problema en el jitter generara una conexión interferida donde se esucharia la comunicación entrecortada, en términos de cual de estos dos factores afectan mas una comunicación la latencia generaría un inconveniente mas pronunciado ya que generara la perdida inmediata del canal de comunicación. 

<img width="583" height="121" alt="imagen" src="https://github.com/user-attachments/assets/e27e0436-a6ff-47ad-a3b2-d86954fd22ab" />

Durante un proceso de transmisión de videos, video llamadas o transmisión de información en forma de video UDP siempre será uno de los mejores medios ya que la diferencia entre UDP y TCP es que UDP no espera la confirmación de la recepción de la información si no que simplemente continua adelante en caso de TCP siempre se espera la confirmación de la recepción de paquete lo cual a nivel de video genera una falencia ya que al perder un frame genera una congelación en el video hasta no obtener el frame faltante en cambio a nivel de UDP no se espera esta confirmación se continua adelante dándole continuidad al video sin interferir con la continuidad del mismo, aunque TCP tendrá un mayor control de perdida de paquetes UDP será el indicado para eventos en vivo o transmisión de videos. 

<img width="588" height="102" alt="imagen" src="https://github.com/user-attachments/assets/20097ae1-1b04-4f66-8809-316ab58b74d0" />

Al ejecutar este comando podemos observar como en cmd nos muestra lo siguiente  

<img width="472" height="424" alt="imagen" src="https://github.com/user-attachments/assets/42150509-c773-48eb-9983-6e18c92ca895" />

Donde podremos observar como este comando nos muestra un proceso de traducción de direcciones ip en direcciones mac lo cual permite saber si las direcciones están asociadas de formas correctas también permite observar protocolos dinámicos o estáticos, es un proceso que trabaja en la capa de acceso a la red del grupo de tcp. 

<img width="472" height="57" alt="imagen" src="https://github.com/user-attachments/assets/404f9857-c389-4504-9f58-dbec7f7a980f" />

SNMPv2c y SNMPv3 Son sistemas de gestión de la red administran diferentes tipos de equipos la diferencia fundamental es el aspecto de seguridad, ya que en SNMPv2c es un protocolo que no tiene seguridad y en caso de que la red sea intervenida se puede observar toda la trama sin cifrar, mientras que SNMPv3 es un protocolo con cifrado y seguridad incorporada que agrega un gran factor de seguridad a la red. 
 
Normalmente SNMPv2c es un protocolo que al llevar a la practica puede tener falencias muy grandes a nivel de seguridad, este protocolo es altamente utilizado para realizar pruebas, lo cual se puede realizar en un ambiente controlado lo cual no agregara vulnerabilidades a la red. 

OID y MIB: un OID (Object Identifier) es un identificador único de un objeto gestionable en la red, como el contador de bytes recibidos en una interfaz. La MIB (Management Information Base) es el “diccionario” que define todos los OID disponibles, qué representan y cómo leerlos o modificarlos. Cada OID está definido dentro de una MIB, es decir, la MIB es la guía y el OID es la entrada específica que querés consultar.

Operaciones SNMP: para consultar la cantidad de bytes que ha recibido una interfaz se usa Get, porque permite leer el valor exacto del OID en ese momento. Set sirve para modificar valores y Trap es solo una notificación automática del dispositivo cuando ocurre un evento (por ejemplo, enlace caído), por eso no sirve para consultas puntuales: un Trap no garantiza que obtengas el dato cuando lo necesitás.

<img width="853" height="285" alt="imagen" src="https://github.com/user-attachments/assets/82f2533d-42a0-4184-bc1c-4400cfb2fed0" />

a) Cabecera Ethernet  
En la cabecera Ethernet encontramos el campo Destino, que representa la dirección física del dispositivo que debe recibir la trama, y el campo Origen, que identifica al equipo que la envía. Ambos son esenciales para que la comunicación se mantenga dentro de la red local. El campo Tipo, con el valor 0x0800, nos indica que el contenido transportado corresponde a un paquete IPv4, lo que permite a los dispositivos interpretar correctamente la información y encaminarla hacia el protocolo adecuado.

b) Cabecera IPv4  
En la cabecera IPv4, el campo Protocolo señala qué protocolo de transporte se está utilizando, siendo el valor 6 equivalente a TCP, mientras que el campo TTL define el número máximo de saltos que puede realizar el paquete antes de ser descartado. Este último es crucial porque evita que los paquetes queden atrapados en bucles de enrutamiento, lo que generaría congestión y degradación en la red. En términos de funcionalidad, el TTL asegura que la comunicación se mantenga estable y que los recursos de la red no se saturen por tráfico inútil.

c) Cabecera TCP  
En la cabecera TCP, los flags ACK y PSH cumplen funciones específicas: el primero confirma la recepción de datos previos, mientras que el segundo fuerza la entrega inmediata de la información a la aplicación sin esperar a llenar el buffer. El Puerto Destino 80 nos habla directamente del servicio al que se intenta acceder, en este caso el protocolo HTTP, que es el estándar para la comunicación web. En términos prácticos, esto significa que el cliente está solicitando un recurso en un servidor web, como una página o archivo.

d) Uso de IPv6  
Si este mismo paquete se enviara bajo IPv6, la cabecera IPv6 reemplazaría a la de IPv4. Una mejora notable sería la simplificación en su procesamiento por parte de los routers, ya que la cabecera IPv6 es más ligera y eficiente, eliminando campos opcionales y manteniendo un formato fijo. Esto genera un entorno más estable y rápido para el tráfico de red, especialmente en sistemas de telecomunicaciones que requieren alta disponibilidad. Además, IPv6 ofrece un espacio de direcciones mucho mayor, lo que garantiza la continuidad del crecimiento de internet sin las limitaciones de IPv4.

<img width="842" height="268" alt="imagen" src="https://github.com/user-attachments/assets/1574694c-da05-40e5-9d7f-e3bb4c2cc11a" />

Ejecutando proceso en linux 

<img width="748" height="332" alt="Captura desde 2026-03-09 17-38-36" src="https://github.com/user-attachments/assets/7f4eb4d6-e9ee-4fd0-bd15-f9189739e695" />

Cuando se ejecuta el comando pathping desde la consola de Windows, lo que se obtiene es una combinación de la información que daría un ping y un tracert. El ping nos habla de la latencia y de la pérdida de paquetes hacia un destino específico, mientras que el tracert nos muestra la ruta completa que siguen los paquetes a través de los diferentes saltos de la red. Pathping une ambos escenarios: primero descubre la ruta como lo hace tracert y luego mide la latencia y la pérdida de paquetes en cada uno de los nodos, lo que permite identificar con precisión dónde se degrada la comunicación.

El proceso que sigue pathping para obtener sus resultados se divide en dos fases. En la primera, envía paquetes con valores crecientes de TTL para descubrir cada salto de la ruta, igual que lo haría tracert. En la segunda, realiza múltiples envíos de paquetes a cada uno de esos saltos durante un tiempo determinado, recopilando estadísticas de latencia y pérdida de paquetes. Con ello genera un informe acumulado que muestra en qué punto exacto de la red se produce la degradación.

En términos de funcionalidad, esto significa que pathping no solo nos dice si hay respuesta o cuál es la ruta, sino que nos muestra con detalle dónde se encuentra el problema. En un sistema de telecomunicaciones, esta diferencia es crítica: mientras ping y tracert ofrecen información parcial, pathping entrega un diagnóstico completo que permite localizar el origen de la falla, ya sea un router intermedio con pérdida de paquetes o un tramo de la red con latencia elevada.

Desarrollo del siguiente punto 

<img width="845" height="259" alt="imagen" src="https://github.com/user-attachments/assets/5825d671-3565-49b0-8e53-bbc39c89c7ab" />

se realiza la instalación del paquete requerido 

<img width="805" height="122" alt="imagen" src="https://github.com/user-attachments/assets/90292aa5-f016-4215-bfd6-55129aca07e0" />

Lo que hace este comando es recorrer (“caminar”) todo el árbol MIB del router y mostrar la información que el dispositivo expone. En palabras simples, es como pedirle al router que nos muestre todos sus datos de estado, por ejemplo el tráfico de las interfaces, si están activas o apagadas y si han tenido errores.

Cuando el router envía un mensaje llamado “authenticationFailure trap”, significa que alguien intentó entrar con una clave o comunidad equivocada. Es como si el router dijera: “me están intentando consultar, pero no tienen permiso”. Este aviso es útil porque nos alerta de intentos de acceso indebido o de errores de configuración.

La ventaja de recibir un Trap frente a estar consultando constantemente al router con polling es que el Trap llega justo en el momento en que ocurre el evento, sin necesidad de estar preguntando todo el tiempo. Esto ahorra recursos en la red y permite reaccionar más rápido. Dicho de manera sencilla, el Trap convierte la gestión en algo proactivo: el router avisa cuando pasa algo, mientras que el polling obliga a estar vigilando de manera continua, lo cual puede ser más pesado y menos eficiente.

<img width="845" height="217" alt="imagen" src="https://github.com/user-attachments/assets/217eecc4-3630-486e-8df7-49cc3379d3da" />

a) Verificación de conectividad básica  
El primer paso para comprobar si tu equipo puede hablar con los servidores de GitHub es usar el comando:

<img width="813" height="308" alt="imagen" src="https://github.com/user-attachments/assets/840c0fd2-3a0f-4ef4-9b1c-4f955148fe83" />

Este comando envía paquetes ICMP y espera respuesta. En términos de modelo OSI, lo que está verificando es la capa de red, porque se asegura de que exista conectividad IP. El protocolo que utiliza es ICMP, que es el encargado de dar mensajes de control y prueba dentro de la red.

b) Resolución de nombres  
Tu equipo no conoce directamente la dirección IP de github.com. Lo que hace es preguntar a un servidor DNS para que traduzca el nombre en una dirección IP. Este proceso se llama resolución de nombres y utiliza el protocolo DNS, que pertenece a la capa de aplicación del modelo OSI. Si la resolución fallara, el comando que se usaría para diagnosticarlo manualmente sería:

<img width="661" height="165" alt="imagen" src="https://github.com/user-attachments/assets/22590bea-5071-49cc-b50c-0299fc91af84" />

Estos comandos muestran qué dirección IP devuelve el servidor DNS y permiten confirmar si el problema está en la traducción del nombre.

c) Latencia alta y variable  
Si el ping es exitoso pero muestra tiempos muy altos y cambiantes, las métricas de teletráfico afectadas son:

    Latencia, porque los paquetes tardan mucho en llegar y regresar.

    Jitter, porque la variación entre los tiempos de respuesta es irregular.


Cuando yo ejecuto git push origin main, lo que realmente está pasando es que Git necesita hablar con GitHub usando HTTPS. Pero antes de que se envíe nada, se abre una conexión confiable gracias a TCP, que es el protocolo de la capa de transporte. TCP es como ese amigo que se asegura de que todo llegue completo y en orden, sin que nada se pierda en el camino.

Lo primero que ocurre es el famoso three-way handshake, que yo lo imagino como un saludo entre dos personas. Mi equipo le dice al servidor: “oye, quiero hablar contigo” (SYN). El servidor responde: “te escucho y estoy listo” (SYN-ACK). Y yo confirmo: “perfecto, ya estamos conectados” (ACK). Con ese intercambio tan simple, la conexión queda lista para que Git empiece a mandar mis datos.

Si en ese momento quisiera ver en vivo cómo se están enviando esos segmentos TCP, abriría Wireshark o usaría tcpdump en la terminal. Con un filtro como tcpdump host <IP_de_GitHub> puedo enfocarme solo en el tráfico que va y viene hacia GitHub, sin que se mezcle con todo lo demás que circula en mi red. Es como poner una lupa sobre esa conversación específica.

En la cabecera TCP de esa conexión, el puerto destino casi siempre es el 443, porque Git usa HTTPS. El puerto origen, en cambio, es uno aleatorio que mi sistema asigna en ese momento para iniciar la comunicación. Y todo esto lo gestiona la capa de transporte, que es la que organiza qué aplicación está hablando y se asegura de que los datos lleguen al proceso correcto.

Al final, cuando yo digo “git push”, no es solo subir archivos: detrás hay un saludo de tres pasos, una conexión segura y un flujo de datos que puedo observar si quiero. Es como ver cómo se abre la puerta, se da la mano y luego empieza la conversación entre mi equipo y GitHub.

<img width="843" height="431" alt="imagen" src="https://github.com/user-attachments/assets/da60694b-8dd9-4900-9013-41c8f3d8c731" />

Cuando yo ejecuto el git push, lo que realmente ocurre es que mis datos —los archivos, el mensaje del commit, todo— empiezan a transformarse capa por capa antes de salir de mi computadora. En la capa de aplicación esos datos son simplemente información que Git prepara para enviar. Al bajar a la capa de transporte, esa información se convierte en segmentos TCP, que ya incluyen detalles como los puertos de origen y destino. Luego, en la capa de red, esos segmentos se encapsulan en paquetes IP, que llevan las direcciones de origen y destino para que puedan viajar por la red. Finalmente, en la capa de enlace, esos paquetes se transforman en tramas Ethernet, que son las que realmente salen por mi tarjeta de red hacia el primer router. Es como si cada capa le fuera poniendo su propia caja y etiqueta al contenido, hasta que queda listo para viajar físicamente.

Mientras esos paquetes IP van saltando de router en router hasta llegar a los servidores de GitHub, puede pasar que alguno de esos routers esté congestionado. Si eso ocurre y empieza a descartar paquetes, mi git push se vería afectado porque los datos no llegarían completos. Aquí es donde TCP demuestra su confiabilidad: detecta la pérdida y activa mecanismos como la retransmisión y el control de congestión, ajustando la velocidad de envío para no saturar más la red. Si yo quisiera identificar en qué salto se están perdiendo los paquetes, usaría un comando como mtr en Linux, que me muestra en tiempo real dónde exactamente se produce la pérdida.

En la cabecera IP hay un detalle muy importante: el campo TTL (Time To Live). Este valor se va reduciendo en cada salto que hace el paquete. Si llega a cero, el paquete se descarta. De esta forma se evita que un paquete quede dando vueltas indefinidamente en la red por un error de enrutamiento. Es como ponerle un contador de vida útil: si no llega a destino en cierto número de saltos, se elimina para no congestionar la red.

<img width="843" height="393" alt="imagen" src="https://github.com/user-attachments/assets/e5b0f91b-f6e3-4621-998b-52786ce1cdd8" />

Cuando yo termino de hacer el git push, los datos llegan al servidor de GitHub, se procesan y lo primero que ocurre es que el servidor me envía una confirmación de que todo salió bien. Esa confirmación viaja en forma de un mensaje TCP de tipo ACK, que es el que me asegura que los datos fueron recibidos correctamente. Aquí se conecta directamente con el concepto de fiabilidad: aunque en la red puedan perderse paquetes, TCP se encarga de retransmitirlos y de confirmar cada entrega, de modo que yo nunca me quedo con la duda de si mi commit llegó o no. Es como tener un recibo firmado de que la información fue entregada.

Una vez que el push ha terminado, la conexión no se corta de golpe, sino que se cierra de manera ordenada. TCP utiliza un proceso de cierre que también es un intercambio de mensajes: primero uno de los extremos envía un FIN para decir “ya terminé”, el otro responde con un ACK confirmando que entendió, y luego envía su propio FIN para cerrar su lado de la comunicación. Finalmente, el primer extremo devuelve otro ACK y la conexión queda cerrada. Es como despedirse educadamente: “ya terminé”, “ok, entendido”, “yo también terminé”, “perfecto, adiós”.

Si yo fuera administrador de red y quisiera monitorear el tráfico que generó mi push, lo haría a través de SNMP en el router de salida. Allí podría observar métricas como los bytes transmitidos y recibidos, el número de paquetes descartados, o incluso la utilización de la interfaz. Esas métricas me darían una idea clara de cómo se comportó la red durante la operación. Y si necesitara que esas consultas estuvieran cifradas para mayor seguridad, usaría SNMPv3



