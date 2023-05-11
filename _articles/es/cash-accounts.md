---
layout: es/post
title: Qué son las Cash Accounts
author: Leo Beltran
date: 2023-01-01
image: cash-accounts.jpg
lead:
categories: uncategorized
id: cashaccounts
---

**Cash Accounts** es un sistema de alias descentralizado, que remplaza las tradicionales direcciones de Bitcoin Cash por una alternativa mucho más simple de recordar y permanente. En esencia, funcionan como un formato alternativo de direcciones que simplifica el intercambio de información requerido para el envío de dinero entre los usuarios.

Una Cash Account sirve para remplazar una dirección como esta `qpv9zu8xfh8p58pcp94qhen7x2mtwc76yytg7nv4zp` por algo más simple en el formato `<USERNAME>#<NUMBER>`.

Pongamos un ejemplo. Supongamos que Satoshi tiene la siguiente dirección: `qpv9zu8xfh8p58pcp94qhen7x2mtwc76yytg7nv4zp`. La Cash Account correspondiente es: `Satoshi#99344`. Por lo tanto, si un usuario quisiera enviarle dinero, en lugar de copiar o escanear la dirección, podría realizar un pago a `Satoshi#99344` desde su billetera y automáticamente Satoshi recibiría sus BCH en la dirección original.

La principal desventaja de este sistema es que, al asociarse el alias a una única dirección, todos los pagos que se envíen a la misma Cash Account pueden ser vinculados. Esto puede ser mitigado con el uso de tecnologías de privacidad, como **CashFusion**.

## Cómo funcionan las Cash Accounts

Cash Accounts es un sistema descentralizado y no depende de ninguna autoridad emitiendo certificados o nombres de usuario, sino que se utiliza la cadena de bloques para dejar asentado las Cash Accounts de forma abierta.

Para registrar una Cash Account, se genera una transacción especial que contiene el alias deseado por el usuario y la dirección a la que asociar dicho alias. Todas las Cash Accounts constan de una segunda parte numérica, que corresponde a la altura del bloque en el que se confirma esta transacción inicial de registro.

De esta manera, al momento de realizar el pago, la billetera accede a esta transacción especial y verifica, usando los mecanismos de seguridad de Bitcoin Cash, a qué dirección está asociada la Cash Account.

## Cómo generar una Cash Account

Cualquier usuario puede generar tantas Cash Accounts como desee. El único costo real es el de la transacción de registro, la cual es extremadamente barata debido a los bajos costos de operación de Bitcoin Cash.

Para hacerlo, pueden seguirse los pasos explicados en esta sección.

### Desde Electron Cash

Para generar una Cash Account en Electron Cash, hace falta tener algo de balance en Bitcoin Cash.

Lo primero es ir a la pestaña **Receive**, para obtener una dirección nueva.

<div>
  <img src="/assets/images/cash-account-1.png" class="img-fluid rounded mx-auto my-4 border d-block">
</div>

Debajo del campo **Receiving address**, se encuentra otro que dice **Cash Account**. Haciendo clic en el ícono verde de la etiqueta, a la derecha, se abrirá una nueva ventana, donde se ofrecerá registrar una nueva Cash Account.

<div>
  <img src="/assets/images/cash-account-2.png" class="img-fluid rounded mx-auto my-4 border d-block">
</div>

Luego de tipear el alias deseado hay que cliquear en **Proceed to Send Tab**.

<div>
  <img src="/assets/images/cash-account-3.png" class="img-fluid rounded mx-auto my-4 border d-block">
</div>

En la siguiente ventana se avisa que se deberá verificar que la transacción esté correcta.

<div>
  <img src="/assets/images/cash-account-4.png" class="img-fluid rounded mx-auto my-4 border d-block">
</div>

Para registrar la transacción, se hará clic en **Send**, completando el envío.

Una vez que la transacción esté confirmada, lo que demora alrededor de diez minutos, la cuenta se encontrará creada y otros usuarios podrán enviar dinero a esa dirección usando el alias de Cash Account.

### Desde CashAccount.info

## Billeteras compatibles

Actualmente, las únicas billeteras compatibles con Cash Accounts son **Electron Cash**, **Zapit** y **Paytaca**.

## Consideraciones de privacidad

### BIP-47

Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

### RPA

Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
