# Simplified Payment Verification

Simplified Payment Verification (‘verificación simplificada de pagos’), también conocido como **SPV**, es un sistema de verificación de transacciones que permite a los usuarios de billeteras ligeras, es decir, que no corren nodos completos, tener acceso al historial de transacciones y poder verificar que determinadas transacciones fueron efectivamente confirmadas y agregadas por los mineros a la cadena de bloques.

Descrita originalmente en la sección 8 del _whitepaper_, SPV es una de las herramientas más útiles para poder obtener certeza acerca del historial de transacciones.

## Funcionamiento paso a paso

La billetera del usuario mantiene una copia de los encabezados de todos los bloques, verificando que sea siempre la cadena con mayor prueba de trabajo. El encabezado es una sección especial del bloque que mantiene, entre otra información, la raíz del árbol de Merkle de ese bloque, es decir, una prueba criptográfica de todas las transacciones que están incluidas en ese bloque. El encabezado ocupa 80 bytes de espacio y la raíz del árbol de Merkle ocupa solamente 32 bytes de espacio. Mantener una copia de los encabezados de todos los bloques requiere a 4,2 megabytes de almacenamiento por año aproximadamente.

Gracias a esta prueba criptográfica, el usuario que solicita verificar la autenticidad de una transacción puede garantizar con certeza que una transacción ha sido incluida dentro de un bloque y que, siendo que posteriormente la red ha construido nuevos bloques sobre este, ha sido considerada como válida por la red.

## Limitaciones

Este sistema, si bien está descrito en el documento original de Bitcoin, tiene algunas limitaciones, las cuales han sido mitigadas a lo largo del tiempo.

Un posible ataque es que el nodo al cual el usuario se conecta le indique que no existe la transacción que está solicitando, incluso aunque esta sí exista. Para evitar este inconveniente, las billeteras que utilizan esta tecnología realizan múltiples conexiones a diferentes servidores SPV, con el fin de aumentar las probabilidades de que al menos uno de ellos sea honesto. Los servidores que hubieren mentido pueden ser baneados, lo cual, aplicado masivamente en todas las billeteras, desincentivaría su uso y consiguientemente la utilidad de correr nodos SPV maliciosos. Dado que las ventajas para un atacante son escasas, es muy raro encontrar nodos que escondan parte del historial de transacciones a los usuarios que lo solicitan, salvo que sea por un problema de límite de cuotas o un error de configuración.

Otra desventaja de este sistema es una disminución en la privacidad del usuario, ya que estaría revelando los servidores cuáles son las transacciones en las que se encuentra interesado y por tanto aumentando las posibilidades de que esos servidores rastreen monedas individuales vinculadas al usuario. Varias de las soluciones propuestas este problema tienen que ver con hacer múltiples pedidos a los servidores, con el fin de obtener información acerca de diversas transacciones no relacionadas entre ellas, y después descartar localmente aquellas que no le interesen al usuario. Otra forma de mitigarlo es utilizar tecnologías que anonimicen el origen de la petición, como por ejemplo Tor.
